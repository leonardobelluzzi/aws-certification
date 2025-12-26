# 📑 Sumário - AWS Certification Study Guide

> Índice rápido de todos os tópicos e serviços AWS documentados

---

## 🎯 Conceitos Fundamentais (14)

| Tópico | Descrição |
|--------|-----------|
| [AWS Well-Architected Framework](Concepts/AWS%20Well-Architected%20Framework.md) | 6 pilares de arquitetura |
| [AWS CAF](Concepts/AWS%20Cloud%20Adoption%20Framework%20(AWS%20CAF).md) | Framework de adoção de nuvem |
| [Cloud Computing Models](Concepts/Cloud%20Computing%20Models.md) | IaaS, PaaS, SaaS |
| [Shared Responsibility](Concepts/Shared%20Responsibility.md) | Modelo de responsabilidade |
| [Region & AZ](Concepts/Region%20&%20Availability%20Zone.md) | Infraestrutura global |
| [Auto Scaling](Concepts/Auto%20Scaling.md) | Escalabilidade automática |
| [Migration Strategy](Concepts/Migration%20strategy.md) | 7Rs de migração |
| [Six Advantages](Concepts/Six%20Advantages.md) | Vantagens da cloud |
| [AWS CloudTrail](Concepts/AWS%20CloudTrail.md) | Auditoria |
| [VPC Gateway Services](Concepts/Services%20support%20VPC%20Gateway.md) | Serviços compatíveis |
| [APN Partner Network](Concepts/APN%20Partner%20Network.md) | Rede de parceiros |
| [Support](Concepts/Suport.md) | Planos de suporte |
| [Costs](Concepts/Costs.md) | Modelos de custo |

---

## 🌐 Networking (8)

| Serviço | Função |
|---------|--------|
| [VPC](Services/Technology/VPC%20-.md) | Virtual Private Cloud |
| [VPC Peering](Networking/VPC%20peering%20connection.md) | Conexão entre VPCs |
| [Route 53](Services/Amazon%20Route%20%2053.md) | DNS e roteamento |
| [CloudFront](Services/Amazon%20CloudFront.md) | CDN global |
| [Direct Connect](Services/AWS%20Direct%20Connect.md) | Conexão dedicada |
| [PrivateLink](Services/AWS%20PrivateLink.md) | Conectividade privada |
| [Global Accelerator](Services/AWS%20Global%20Accelerator.md) | Aceleração de rede |
| [Transit Gateway](Services/Technology/AWS%20Transit%20Gateway.md) | Hub de redes |
| [S3 Transfer Acceleration](Networking/Amazon%20S3%20Transfer%20Acceleration%20(S3TA).md) | Upload acelerado |

---

## 💾 Storage (8)

| Serviço | Tipo | Caso de Uso |
|---------|------|-------------|
| [Amazon S3](Services/Technology/Storage/S3.md) | Object | Armazenamento de objetos |
| [Amazon EBS](Services/Technology/Storage/EBS%20-%20Amazon%20Elastic%20Block%20Storage.md) | Block | Volumes para EC2 |
| [Amazon EFS](Services/Technology/Storage/EFS%20-%20Elastic%20File%20System.md) | File | File system compartilhado |
| [FSx Windows](Services/Technology/Storage/FSx%20for%20Windows%20File%20Server.md) | File | Windows file server |
| [S3 File Gateway](Services/Amazon%20S3%20File%20Gateway.md) | Hybrid | Gateway para S3 |
| [AMI](Storage/Amazon%20Machine%20Image.md) | Image | Template de instância |
| [Snowball](Storage/AWS%20Snowball.md) | Physical | Migração física de dados |
| [Storage Differences](Services/Technology/Storage/Diference.md) | Comparison | Comparação de tipos |

---

## 🗄️ Database (10)

### Relacional
| Serviço | Descrição |
|---------|-----------|
| [Amazon RDS](Services/Technology/Database/RDS.md) | Banco relacional gerenciado |
| [Amazon Aurora](Services/Technology/Database/Amazon%20Aurora.md) | MySQL/PostgreSQL otimizado |

### NoSQL
| Serviço | Descrição |
|---------|-----------|
| [DynamoDB](Services/Technology/Database/NoSQL/Amazon%20DynamoDB.md) | NoSQL key-value |
| [DynamoDB Global Tables](Services/Technology/Database/NoSQL/Amazon%20DynamoDB%20with%20global%20tables.md) | Multi-região |
| [DynamoDB Overview](Services/DynamoDb.md) | Visão geral |

### Analytics
| Serviço | Descrição |
|---------|-----------|
| [Amazon Athena](Services/Technology/Database/Amazon%20Athena.md) | Query em S3 |
| [Amazon Redshift](Services/Amazon%20Redshift%20Reserved%20Nodes.md) | Data warehouse |
| [Amazon ElastiCache](Services/Technology/Database/Amazon%20ElastiCache.md) | Cache in-memory |

### Migração
| Serviço | Descrição |
|---------|-----------|
| [Database Migration Service](Database/AWS%20Database%20Migration%20Service.md) | Migração de bancos |

---

## 🔒 Security & Compliance (15)

### Identity & Access
| Serviço | Função |
|---------|--------|
| [IAM](Services/Security%20and%20Compliance/(IAM)%20AWS%20Identity%20and%20Access%20Management.md) | Gerenciamento de identidades |
| [Secrets Manager](Services/Security%20and%20Compliance/AWS%20Secrets%20Manager.md) | Gerenciamento de secrets |

### Monitoramento
| Serviço | Função |
|---------|--------|
| [CloudTrail](Services/Security%20and%20Compliance/AWS%20CloudTrail.md) | Log de API calls |
| [Amazon Inspector](Services/Security%20and%20Compliance/Amazon%20Inspector.md) | Avaliação de segurança |

### Proteção
| Serviço | Função |
|---------|--------|
| [AWS Shield](Services/Security%20and%20Compliance/AWS%20Shield%20Standard.md) | Proteção DDoS |
| [AWS WAF](Services/Security%20and%20Compliance/AWS%20Web%20Application%20Firewall%20(WAF).md) | Firewall de aplicação |
| [Encrypting](Services/Security%20and%20Compliance/Encrypting.md) | Criptografia |

### Compliance
| Recurso | Descrição |
|---------|-----------|
| [AWS Artifact](Services/Security%20and%20Compliance/AWS%20Artifact.md) | Relatórios de compliance |
| [Penetration Testing](Security%20&%20Compliance/Penetration%20Testing.md) | Testes de penetração |

### Management
| Serviço | Função |
|---------|--------|
| [Systems Manager](Services/Security%20and%20Compliance/AWS%20Systems%20Manager.md) | Gerenciamento de recursos |
| [Session Manager](Services/Security%20and%20Compliance/AWS%20Systems%20Manager%20Session%20Manager.md) | Acesso seguro |

---

## 💰 Billing & Cost Management (6)

| Serviço/Conceito | Função |
|------------------|--------|
| [AWS Billing](Billing%20&%20Cost%20Management/AWS%20Billing.md) | Faturamento |
| [Cost Explorer](Services/Billing%20and%20Pricing/AWS%20Cost%20Explorer.md) | Análise de custos |
| [AWS Budgets](Services/Billing%20and%20Pricing/AWS%20Budgets.md) | Orçamentos e alertas |
| [Pricing Calculator](Services/Billing%20and%20Pricing/Pricing%20Calculator.md) | Calculadora |
| [Reserved Instances](Services/Billing%20and%20Pricing/Services%20support%20reservations%20to%20optimize%20costs.md) | Otimização |
| [Organizations](Services/Billing%20and%20Pricing/AWS%20Organization.md) | Multi-conta |

---

## 🚀 Compute (6)

| Serviço | Tipo | Descrição |
|---------|------|-----------|
| [Amazon EC2](Services/EC2.md) | IaaS | Servidores virtuais |
| [AWS Lambda](Services/Serverless/AWS%20Lambda.md) | Serverless | Funções sem servidor |
| [Elastic Beanstalk](Services/AWS%20Elastic%20Beanstalk.md) | PaaS | Deploy de aplicações |
| [ECS](Services/ECS%20-%20Amazon%20Elastic%20Container%20Service%20-%20%20Fargate%20launch%20type.md) | Containers | Orquestração de containers |
| [ECR](Services/ECR%20-%20Amazon%20Elastic%20Container%20Registry.md) | Registry | Registro de containers |
| [ELB](Services/ELB%20-%20Elastic%20Load%20Balancing.md) | Load Balancer | Balanceamento de carga |

---

## 📨 Messaging (4)

| Serviço | Tipo | Caso de Uso |
|---------|------|-------------|
| [Amazon SNS](Services/Technology/Message/SNS%20-%20Amazon%20Simple%20Notification%20Service.md) | Pub/Sub | Notificações |
| [Amazon SQS](Services/Technology/Message/SQS%20-%20Amazon%20Simple%20Queue%20Service.md) | Queue | Filas de mensagens |
| [Amazon MQ](Services/Technology/Message/MQ%20Amazon.md) | Broker | Message broker |
| [EventBridge](Services/Serverless/Amazon%20Eventbridge.md) | Event Bus | Eventos serverless |

---

## 🤖 AI/ML & Language (5)

| Serviço | Função |
|---------|--------|
| [Amazon Polly](Services/Language/Amazon%20Polly.md) | Text-to-Speech |
| [Amazon Transcribe](Services/Language/Amazon%20Transcribe.md) | Speech-to-Text |
| [Amazon Translate](Services/Language/Amazon%20Translate.md) | Tradução automática |
| [Amazon Rekognition](Services/Amazon%20Rekognition.md) | Visão computacional |
| [Amazon Macie](Services/Amazon%20Macie.md) | Segurança de dados |

---

## 🔍 Analytics (3)

| Serviço | Função |
|---------|--------|
| [Amazon Kendra](Search%20&%20Analytics/Amazon%20Kendra.md) | Busca inteligente |
| [Amazon EMR](Services/Amazon%20EMR.md) | Big Data (Hadoop/Spark) |
| [Kinesis Data Streams](Services/Amazon%20Kinesis%20Data%20Streams.md) | Streaming de dados |

---

## 🛠️ Developer Tools (3)

| Serviço | Função |
|---------|--------|
| [CodePipeline](Developer%20Tools/AWS%20CodePipeline.md) | CI/CD pipeline |
| [CodeDeploy](Developer%20Tools/CodeDeploy.md) | Deploy automatizado |
| [Device Farm](Developer%20Tools/AWS%20Device%20Farm.md) | Testes em dispositivos |

---

## ⚙️ Management & Governance (6)

| Serviço | Função |
|---------|--------|
| [CloudFormation](Management%20&%20Governance/AWS%20CloudFormation.md) | Infrastructure as Code |
| [AWS Config](Management%20&%20Governance/AWS%20Config.md) | Auditoria de config |
| [CloudWatch](Services/CloudWatch.md) | Monitoramento |
| [Trusted Advisor](Services/AWS%20Trusted%20Advisor.md) | Recomendações |
| [Service Catalog](Services/AWS%20Service%20Catalog.md) | Catálogo de serviços |
| [Health Dashboard](Management%20&%20Governance/AWS%20Health%20Dashboard.md) | Status de saúde |

---

## 🛒 Marketplace (1)

| Recurso | Descrição |
|---------|-----------|
| [AWS Marketplace](Marketplace/AWS%20Marketplace.md) | Catálogo de soluções de terceiros |

---

## ✅ Practice & Testing (2)

| Tipo | Link |
|------|------|
| **Resultados de Testes** | [Tests Results](Tests/Tests%20results.md) |
| **Questões Práticas** | [Organization Planning](Questions/Organization%20is%20planning.md) |

---

## 📝 Daily Notes (2)

| Data | Link |
|------|------|
| 02 Set 2025 | [Daily Note](Daily%20Notes/2025-09-02.md) |
| 26 Dez 2025 | [Daily Note](Daily%20Notes/2025-12-26.md) |

---

## 📊 Resumo por Categoria

| Categoria | Quantidade | % do Total |
|-----------|------------|------------|
| 🚀 Services (Diversos) | 50 | 54% |
| 🎯 Concepts | 14 | 15% |
| 🔒 Security & Compliance | 15 | 16% |
| 🌐 Networking | 8 | 9% |
| 💾 Storage | 8 | 9% |
| 🗄️ Database | 10 | 11% |
| 💰 Billing | 6 | 6% |
| 🛠️ Developer Tools | 3 | 3% |
| ⚙️ Management | 6 | 6% |
| 🔍 Analytics | 3 | 3% |
| **TOTAL** | **93** | **100%** |

---

## 🎯 Mapa Mental de Serviços

```
AWS Cloud
│
├── Compute
│   ├── EC2 (VMs)
│   ├── Lambda (Serverless)
│   ├── ECS/ECR (Containers)
│   └── Elastic Beanstalk (PaaS)
│
├── Storage
│   ├── S3 (Object)
│   ├── EBS (Block)
│   ├── EFS (File)
│   └── Snowball (Physical)
│
├── Database
│   ├── RDS/Aurora (Relational)
│   ├── DynamoDB (NoSQL)
│   ├── ElastiCache (Cache)
│   └── Redshift (Warehouse)
│
├── Networking
│   ├── VPC (Network)
│   ├── Route 53 (DNS)
│   ├── CloudFront (CDN)
│   └── Direct Connect (Hybrid)
│
├── Security
│   ├── IAM (Access)
│   ├── CloudTrail (Audit)
│   ├── Shield/WAF (Protection)
│   └── Secrets Manager
│
├── Management
│   ├── CloudFormation (IaC)
│   ├── CloudWatch (Monitor)
│   ├── Config (Compliance)
│   └── Trusted Advisor
│
├── Analytics
│   ├── Athena (Query)
│   ├── EMR (Big Data)
│   └── Kinesis (Streaming)
│
└── AI/ML
    ├── Polly (Speech)
    ├── Rekognition (Vision)
    └── Translate (Language)
```

---

## 🔗 Navegação Rápida

### Por Frequência em Provas
🔥 **Muito Comum**
- EC2, S3, IAM, VPC, CloudWatch, Auto Scaling

⭐ **Comum**
- Lambda, RDS, DynamoDB, CloudFront, Route 53, ELB

💡 **Importante Conhecer**
- CloudFormation, SNS, SQS, CloudTrail, Cost Explorer

---

**Última atualização: 26/12/2025**

[← Voltar para README](README.md)
