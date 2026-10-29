## 📋 Visão Geral

Amazon Virtual Private Cloud (VPC) enables you to launch AWS resources into a virtual network that you've defined. This virtual network closely resembles a traditional network that you'd operate in your own data center, with the benefits of using the scalable infrastructure of AWS.

---

## 🔌 VPC Endpoints

A **VPC endpoint** enables you to **privately connect your VPC** to supported AWS services and VPC endpoint services powered by [AWS PrivateLink](../../AWS%20PrivateLink.md) without requiring:
- ❌ Internet gateway
- ❌ NAT device
- ❌ VPN connection
- ❌ [AWS Direct Connect](../../AWS%20Direct%20Connect.md) connection

### ✅ Benefícios

- 🔒 **Privacidade:** Traffic does not leave the Amazon network
- 🚀 **Performance:** Melhor latência e throughput
- 💰 **Custo:** Sem custos de NAT Gateway ou Internet Gateway
- 🔐 **Segurança:** Instances não precisam de IPs públicos

---

## USES CASES

### Use case 

Only Amazon S3 and Amazon DynamoDB support VPC gateway endpoint

## 🔀 Tipos de VPC Endpoints

### 1️⃣ Interface Endpoint (VPC Interface Endpoint)

**O que é:**
- Elastic network interface com IP privado do range da subnet
- Entry point para tráfego destinado a serviços suportados
- Powered by [AWS PrivateLink](../../AWS%20PrivateLink.md)

**Características:**
- ✅ Usa endereços IP **privados**
- ✅ Suporta **maioria dos serviços AWS**
- ✅ Permite acesso via **DNS privado**
- 💰 Tem custo por hora + data processed

**Serviços Suportados:**
- Amazon API Gateway
- Amazon CloudWatch
- [Amazon SNS](Message/SNS%20-%20Amazon%20Simple%20Notification%20Service.md)
- [Amazon SQS](Message/SQS%20-%20Amazon%20Simple%20Queue%20Service.md)
- AWS Systems Manager
- E muitos outros...

---

### 2️⃣ Gateway Endpoint (VPC Gateway Endpoint)

**O que é:**
- Gateway especificado como **target em route table**
- Para tráfego destinado a serviços suportados

**Características:**
- ✅ **Sem custo** adicional
- ✅ Usa **route tables** para direcionar tráfego
- ✅ Altamente escalável
- ⚠️ Suporta **APENAS 2 serviços**

**Serviços Suportados:**
1. [Amazon S3](Storage/S3.md) ⭐
2. [Amazon DynamoDB](Amazon%20DynamoDB.md) ⭐

![VPC Gateway Endpoint](../../Images/Pasted%20image%2020250718085045.png)

---

## ⚠️ Exam Alert - VPC Gateway vs Interface Endpoint

### 🎯 Regra de Ouro para Certificação

**VPC Gateway Endpoint (Gratuito):**
- ✅ **Apenas** [Amazon S3](Storage/S3.md)
- ✅ **Apenas** [Amazon DynamoDB](Amazon%20DynamoDB.md)

**VPC Interface Endpoint (Pago):**
- ✅ **Todos os outros serviços** AWS que suportam VPC Endpoints
- ✅ [Amazon S3](Storage/S3.md) também suporta (além do Gateway)

### 📊 Comparação Rápida

| Característica | Gateway Endpoint | Interface Endpoint |
|----------------|------------------|-------------------|
| **Serviços** | S3, DynamoDB | Maioria dos serviços AWS |
| **Custo** | 🆓 Gratuito | 💰 Pago |
| **Implementação** | Route table | ENI com IP privado |
| **DNS** | Usa endpoint público | DNS privado |
| **Alta disponibilidade** | Automática | Multi-AZ recomendado |

![VPC Endpoints Comparison](../../Images/Pasted%20image%2020250718085136.png)

---

## 🏗️ Componentes Principais da VPC

### Subnets
- **Public Subnet:** Tem rota para Internet Gateway
- **Private Subnet:** Sem acesso direto à internet

### Route Tables
- Definem regras de roteamento de tráfego
- Cada subnet deve estar associada a uma route table

### Internet Gateway (IGW)
- Permite comunicação entre VPC e internet
- Escalável, redundante, sem limitações de bandwidth

### NAT Gateway/Instance
- Permite instâncias em subnets privadas acessarem internet
- Para downloads, updates, etc.
- **A Network Address Translation gateway (NAT gateway) is managed by AWS** (alta disponibilidade e escalabilidade automática)

### Security Groups
- Firewall **stateful** ao nível de instância
- Controla tráfego inbound/outbound
- **A Security Group can have allow rules only** (não possui regras de deny explícitas)

### Network ACLs (NACLs)
- Firewall **stateless** ao nível de subnet
- Avalia regras em ordem numérica

---

## 🔗 Conectividade VPC

### Conexões Privadas
- [VPC Peering](../../../Networking/VPC%20peering%20connection.md) - Conexão entre VPCs
- [AWS Transit Gateway](AWS%20Transit%20Gateway.md) - Hub central de rede
- [AWS PrivateLink](../../AWS%20PrivateLink.md) - Acesso privado a serviços

### Conexões Híbridas
- [AWS Direct Connect](../../AWS%20Direct%20Connect.md) - Conexão dedicada
- AWS VPN - Conexão criptografada via internet

---

## 💡 Casos de Uso - VPC Endpoints

### ✅ Cenário 1: EC2 Acessando S3 Privadamente

**Sem VPC Endpoint:**
- EC2 em subnet privada → NAT Gateway → Internet Gateway → S3
- 💰 Custo de NAT Gateway
- 🐌 Latência maior

**Com VPC Gateway Endpoint:**
- EC2 em subnet privada → VPC Gateway Endpoint → S3
- 🆓 Sem custo adicional
- 🚀 Menor latência
- 🔒 Tráfego não sai da rede AWS

### ✅ Cenário 2: Lambda Acessando DynamoDB

**Melhor prática:**
- Usar **VPC Gateway Endpoint** para DynamoDB
- Lambda não precisa de IP público
- Sem custo adicional

### ✅ Cenário 3: Aplicação Acessando Secrets Manager

**Solução:**
- Criar **VPC Interface Endpoint** para Secrets Manager
- Aplicação acessa via DNS privado
- 🔒 Credenciais não trafegam pela internet

---

## 📌 Pontos Importantes para Certificação

### ⭐ VPC Endpoints

1. **Gateway Endpoint = S3 + DynamoDB APENAS** (gratuito)
2. **Interface Endpoint = Outros serviços** (pago)
3. **S3 suporta AMBOS** os tipos de endpoint
4. VPC Endpoints **NÃO requerem Internet Gateway**
5. Tráfego **permanece na rede AWS**
6. Gateway Endpoint usa **route tables**
7. Interface Endpoint usa **ENI** (Elastic Network Interface)

### ⭐ Segurança

- Security Groups são **stateful** (rastreia conexões)
- NACLs são **stateless** (não rastreia)
- Um Security Group por padrão **nega tudo inbound**
- NACLs por padrão **permitem tudo**

### ⭐ Conectividade

- **1 VPC = 1 Region** (mas pode ter múltiplas AZs)
- VPC Peering **não é transitivo**
- Transit Gateway **é transitivo**
- Direct Connect leva **pelo menos 1 mês** para provisionar

---

## 🔗 Serviços Relacionados

### Networking
- [VPC Peering](../../../Networking/VPC%20peering%20connection.md) - Conexão entre VPCs
- [AWS Transit Gateway](AWS%20Transit%20Gateway.md) - Hub de rede
- [AWS Direct Connect](../../AWS%20Direct%20Connect.md) - Conexão dedicada
- [AWS PrivateLink](../../AWS%20PrivateLink.md) - Conectividade privada
- [Amazon Route 53](../../Amazon%20Route%20%2053.md) - DNS

### Compute & Storage
- [Amazon EC2](../../EC2.md) - Virtual servers
- [Amazon S3](Storage/S3.md) - Object storage
- [Amazon EBS](Storage/EBS%20-%20Amazon%20Elastic%20Block%20Storage.md) - Block storage

### Database
- [Amazon DynamoDB](Amazon%20DynamoDB.md) - NoSQL database
- [Amazon RDS](Database/RDS.md) - Relational database

### Security
- [AWS IAM](../../Security%20and%20Compliance/(IAM)%20AWS%20Identity%20and%20Access%20Management.md) - Access management
- [AWS Shield](../../Security%20and%20Compliance/AWS%20Shield%20Standard.md) - DDoS protection

---

## 📚 Recursos Adicionais

- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/)
- [VPC Endpoint Services](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints.html)
- VPC Design Best Practices

---

## USE CASE

A customer has created a VPC and a subnet within AWS Cloud. Which of the following statements is correct?

An Amazon Virtual Private Cloud (Amazon VPC) spans all of the Availability Zones (AZ) in the Region whereas a subnet spans only one Availability Zone (AZ) in the Region


## USE CASE

Which of the following statement is correct for a Security Group and a Network Access Control List (Network ACL)?

Security Group acts as a firewall at the instance level whereas Network Access Control List (Network ACL) acts as a firewall at the subnet level

## USE CASE

Which AWS service will you use to privately connect your virtual private cloud (VPC) to Amazon Simple Storage Service (Amazon S3)?

VPC Endpoint


## USE CASE

Which of the following statements are CORRECT regarding security groups and network access control lists (network ACL)? (Select two)

A network access control list (network ACL) contains a numbered list of rules and evaluates these rules in the increasing order while deciding whether to allow the traffic
A security group is stateful, that is, it automatically allows the return traffic

## USE CASE


Which AWS service would you use to create a logically isolated section of the AWS Cloud where you can launch AWS resources in your virtual network?

Virtual private Cloud (VPC)

## USE CASE 

Which AWS entity enables you to privately connect your Amazon Virtual Private Cloud (Amazon VPC) to an Amazon Simple Queue Service (Amazon SQS) queue?

VPC Interface Endpoint

## USE CASE

Which of the following entities are part of an Amazon Virtual Private Cloud (Amazon VPC) in the AWS Cloud? (Select two)

Internet Gateway
Subnet

## USE CASE 

Which security control tool can be used to deny traffic from a specific IP address?

Network Access Control List (network ACL)

## USE CASE

Which of the following statements is CORRECT regarding the scope of an Amazon Virtual Private Cloud (VPC)?

A VPC spans all Availability Zones (AZs) within an AWS region

## USE CASE

Which of the following AWS services will help provision a logically isolated network for your AWS resources?

Amazon Virtual Private Cloud (Amazon VPC)
