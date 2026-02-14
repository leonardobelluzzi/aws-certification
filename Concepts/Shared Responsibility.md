# AWS Shared Responsibility Model

## 📋 Visão Geral

Security and Compliance is a **shared responsibility** between AWS and the customer. This shared model can help relieve the customer's operational burden as AWS operates, manages and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates.

![Shared Responsibility Model](../Images/Pasted%20image%2020250716135922.png)

---

## 🏗️ Divisão de Responsabilidades

### ☁️ AWS - Responsável PELA Nuvem (Security OF the Cloud)

AWS é responsável por proteger a infraestrutura que executa todos os serviços oferecidos na AWS Cloud:

| Camada | Responsabilidade AWS |
|--------|---------------------|
| **Hardware/Infraestrutura Global** | Data centers físicos, racks, servidores |
| **Rede** | Switches, roteadores, firewalls de infraestrutura |
| **Virtualização** | Hypervisor, host operating system |
| **Segurança Física** | Acesso aos data centers, vigilância, controle ambiental |
| **Disponibilidade** | Regions, Availability Zones, Edge Locations |

**Em resumo:** AWS cuida de tudo que você **não pode acessar fisicamente**.

---

### 👤 Cliente - Responsável NA Nuvem (Security IN the Cloud)

O cliente é responsável por tudo que ele **cria e coloca** na AWS Cloud:

| Camada | Responsabilidade Cliente |
|--------|-------------------------|
| **Dados** | Dados do cliente, classificação, criptografia |
| **Aplicações** | Código da aplicação, configurações |
| **Sistema Operacional** | Patches, updates, configurações de OS |
| **Rede Virtual** | Configuração de [VPC](../Services/Technology/VPC%20-.md), Security Groups, NACLs |
| **Identity & Access** | [IAM](../Services/Security%20and%20Compliance/(IAM)%20AWS%20Identity%20and%20Access%20Management.md) users, roles, policies, MFA |
| **Criptografia** | Client-side, server-side, encryption at rest/in transit |
| **Firewall** | Security Groups, Network ACLs, WAF rules |

**Em resumo:** Cliente cuida de tudo que ele **pode configurar e controlar**.

---

## 🔄 Modelo de Responsabilidade Compartilhada

### Configuration Management

A **gestão de configuração** é uma responsabilidade compartilhada:

- **AWS:** Configura e mantém a infraestrutura subjacente
- **Cliente:** Configura os recursos que provisiona (EC2, RDS, S3, etc.)

---

## 📊 Variações por Tipo de Serviço

### IaaS - Infrastructure as a Service
**Exemplo:** [Amazon EC2](../Services/EC2.md)

Cliente tem **MAIS responsabilidade**:
- ✅ Sistema operacional
- ✅ Patches e atualizações
- ✅ Aplicações
- ✅ Configuração de rede
- ✅ Segurança de dados

### PaaS - Platform as a Service
**Exemplo:** [AWS Elastic Beanstalk](../Services/AWS%20Elastic%20Beanstalk.md)

Responsabilidade **COMPARTILHADA**:
- ✅ Cliente: Aplicação e dados
- ✅ AWS: OS, runtime, patches

### SaaS - Software as a Service
**Exemplo:** AWS Managed Services

Cliente tem **MENOS responsabilidade**:
- ✅ Principalmente dados e controle de acesso
- ✅ AWS gerencia quase tudo

---

## 🔐 Segurança por Camada

### Camadas de Responsabilidade por Serviço

| Serviço | AWS Gerencia | Cliente Gerencia |
|---------|--------------|------------------|
| [EC2](../Services/EC2.md) | Hardware, host OS, hypervisor | Guest OS, apps, dados, firewall |
| [RDS](../Services/Technology/Database/RDS.md) | Hardware, OS, DB engine patches | Dados, users, backups, encryption |
| [S3](../Services/Technology/Storage/S3.md) | Infraestrutura, durabilidade | Dados, bucket policies, encryption |
| [Lambda](../Services/Serverless/AWS%20Lambda.md) | Toda infraestrutura e runtime | Código da função, IAM roles |
| [DynamoDB](../Services/Technology/Database/NoSQL/Amazon%20DynamoDB.md) | Hardware, replicação, patches | Dados, IAM, encryption settings |

---

## 🛡️ Ferramentas para Responsabilidade do Cliente

### Security & Compliance
- [AWS IAM](../Services/Security%20and%20Compliance/(IAM)%20AWS%20Identity%20and%20Access%20Management.md) - Controle de acesso
- [AWS CloudTrail](AWS%20CloudTrail.md) - Auditoria de ações
- [AWS Config](../Management%20&%20Governance/AWS%20Config.md) - Conformidade de configuração
- [AWS Shield](../Services/Security%20and%20Compliance/AWS%20Shield%20Standard.md) - Proteção DDoS
- [AWS WAF](../Services/Security%20and%20Compliance/AWS%20Web%20Application%20Firewall%20(WAF).md) - Firewall de aplicação

### Monitoramento
- [Amazon CloudWatch](../Services/CloudWatch.md) - Logs e métricas
- [Amazon Inspector](../Services/Security%20and%20Compliance/Amazon%20Inspector.md) - Avaliação de vulnerabilidades
- [Amazon Macie](../Services/Amazon%20Macie.md) - Proteção de dados sensíveis

### Encryption
- [AWS KMS](../Services/Security%20and%20Compliance/Encrypting.md) - Key Management
- [AWS Secrets Manager](../Services/Security%20and%20Compliance/AWS%20Secrets%20Manager.md) - Gerenciamento de secrets

---

## 💡 Casos de Uso e Exemplos

### ✅ Cenário 1: EC2 Instance Comprometida

**Responsabilidade AWS:**
- ✅ Garantir segurança física do data center
- ✅ Manter hypervisor atualizado
- ✅ Isolar instâncias de outros clientes

**Responsabilidade Cliente:**
- ❌ Aplicar patches no OS da instância
- ❌ Configurar Security Groups corretamente
- ❌ Implementar antivírus/IDS se necessário
- ❌ Restringir acesso via IAM

### ✅ Cenário 2: Dados Sensíveis em S3

**Responsabilidade AWS:**
- ✅ Proteger infraestrutura de storage
- ✅ Garantir durabilidade (99.999999999%)
- ✅ Disponibilizar opções de criptografia

**Responsabilidade Cliente:**
- ❌ Ativar criptografia (SSE-S3, SSE-KMS)
- ❌ Configurar bucket policies
- ❌ Habilitar versioning
- ❌ Configurar logging com [CloudTrail](AWS%20CloudTrail.md)
- ❌ Bloquear acesso público

---

## 📌 Pontos Importantes para Certificação

### ⭐ Princípios Fundamentais

1. **AWS = Security OF the Cloud** (infraestrutura)
2. **Cliente = Security IN the Cloud** (dados e configurações)
3. **Quanto mais gerenciado o serviço, menos responsabilidade o cliente tem**
4. **Cliente SEMPRE é responsável por seus dados**
5. **IAM e criptografia são SEMPRE responsabilidade do cliente**

### 🎯 Perguntas Comuns em Provas

**P: Quem é responsável por patches do OS em EC2?**
R: Cliente ✅

**P: Quem é responsável por patches do OS em RDS?**
R: AWS ✅

**P: Quem é responsável pela segurança física dos data centers?**
R: AWS ✅

**P: Quem é responsável pela criptografia dos dados?**
R: Cliente (decidir e configurar) ✅

**P: Quem é responsável pela configuração de Security Groups?**
R: Cliente ✅

---

## 🔗 Frameworks Relacionados

- [AWS Well-Architected Framework](AWS%20Well-Architected%20Framework.md) - Pilar de Segurança
- [AWS Compliance Programs](../Services/Security%20and%20Compliance/AWS%20Artifact.md) - Certificações
- [Penetration Testing](../Security%20&%20Compliance/Penetration%20Testing.md) - Testes permitidos

---

## 📚 Recursos Oficiais

- [AWS Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)
- AWS Security Best Practices
- AWS Security Documentation

---

## USE CASE 

According to the AWS Shared Responsibility Model, which of the following are responsibilities of the customer for Amazon RDS?

Database encryption

## USE CASE

As per the AWS Shared Responsibility Model, which of the following is a responsibility of AWS from a security and compliance point of view?

Edge Location Management

## USE CASE

As per the AWS Shared Responsibility Model, which of the following is a responsibility of the customer from a security and compliance point of view?

Managing patches of the guest operating system on Amazon Elastic Compute Cloud (Amazon EC2)

**Última atualização:** 26/12/2025

## USE CASE 

Which of the following are correct statements regarding the AWS Shared Responsibility Model? (Select two)

AWS is responsible for Security 'of' the Cloud
For abstracted services like Amazon S3, AWS operates the infrastructure layer, the operating system, and platforms


## USE CASE 

According to the AWS Shared Responsibility Model, which of the following are responsibilities of the customer for AWS Identity and Access Management (AWS IAM)? (Select two)

Analyze user access patterns and review AWS Identity and Access Management (AWS IAM) permissions
Enable multi-factor authentication (MFA) on all accounts

## USE CASE

According to the AWS Shared Responsibility Model, which of the following is the responsibility of the customer?

Firewall & networking configuration of Amazon Elastic Compute Cloud (Amazon EC2)

## USE CASE

According to the AWS Shared Responsibility Model, which of the following are the responsibilities of AWS? (Select two)

Network operability
Data center security

## USE CASE

According to the AWS Shared Responsibility Model, which of the following is both the responsibility of AWS and the customer? (Select two)

Operating system (OS) configuration
Configuration management
