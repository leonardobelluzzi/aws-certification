# AWS USE CASES - Documento Consolidado

> Este documento consolida todos os casos de uso (USE CASES) encontrados nos arquivos de estudo da AWS.
> Gerado automaticamente em: 09/01/2026

---

## 📑 Índice

- [Security & Compliance](#security--compliance)
- [Storage](#storage)
- [Networking](#networking)
- [Serverless](#serverless)
- [Developer Tools](#developer-tools)
- [Management & Governance](#management--governance)
- [Messaging](#messaging)
- [Search & Analytics](#search--analytics)

---

## Security & Compliance

### MFA - Multi-Factor Authentication

#### USE CASE 1
**Cenário:** A financial services enterprise plans to enable Multi-Factor Authentication (MFA) for its employees. For ease of travel, they prefer not to use any physical devices to implement Multi-Factor Authentication (MFA). Which of the below options is best suited for this use case?

**Resposta:** Virtual Multi-Factor Authentication (MFA) device

#### USE CASE 2
**Cenário:** Which of the following AWS authentication mechanisms supports an AWS Multi-Factor Authentication (AWS MFA) device that you can plug into a USB port on your computer?

**Resposta:** U2F security key

---

### AWS IAM (Identity and Access Management)

#### USE CASE 1
**Cenário:** An organization wants to secure its AWS resources and ensure only authorized users can access specific services.

**Resposta:** Use AWS IAM to create users, groups, roles, and policies with least privilege access.

#### USE CASE 2
**Cenário:** A company needs to grant temporary access to external contractors to specific AWS resources.

**Resposta:** Use IAM Roles with temporary credentials instead of creating permanent IAM users.

#### USE CASE 3
**Cenário:** An application running on EC2 needs to access S3 buckets securely without storing credentials in code.

**Resposta:** Attach an IAM Role to the EC2 instance with appropriate S3 permissions.

#### USE CASE 4
**Cenário:** An organization wants to enforce MFA for all IAM users accessing the AWS Management Console.

**Resposta:** Create an IAM policy that requires MFA authentication for console access.

---

### AWS CloudTrail

#### USE CASE 1
**Cenário:** A financial services company wants to ensure that its AWS account activity meets the governance, compliance and auditing norms.

**Resposta:** AWS CloudTrail

**Nota:** CloudTrail has encryption enabled by default.

---

### AWS Shield

#### USE CASE 1
**Cenário:** AWS Service can be used to mitigate a Distributed Denial of Service attack.

**Resposta:** AWS Shield

#### USE CASE 2
**Cenário:** Which of the following AWS services can be used to prevent Distributed Denial-of-Service (DDoS) attack? (Select three)

**Resposta:**
- AWS Shield
- AWS Web Application Firewall (AWS WAF)
- Amazon CloudFront with Amazon Route 53

#### USE CASE 3
**Cenário:** Which of the following is correct regarding the AWS Shield Advanced pricing?

**Resposta:** AWS Shield Advanced offers protection against higher fees that could result from a DDoS attack

---

### AWS Web Application Firewall (WAF)

#### USE CASE 1
**Cenário:** A social media company wants to protect its web application from common web exploits such as SQL injection and cross-site scripting. Which of the following AWS services can be used to address this use-case?

**Resposta:** AWS Web Application Firewall (AWS WAF)

**Nota:** AWS WAF operates at Layer 7 (Application Layer)

#### USE CASE 2
**Cenário:** An online gaming company wants to block users from certain geographies from accessing its content. Which AWS service can be used to accomplish this task?

**Resposta:** AWS Web Application Firewall (AWS WAF)

#### USE CASE 3
**Cenário:** A global e-commerce platform wants to restrict access to its website from specific countries to comply with regional regulations. Which AWS service is best suited to implement this restriction?

**Resposta:** Amazon WAF

**Nota:** WAF can create geographic match (geo-match) conditions to block web requests from specific countries.

#### USE CASE 4
**Cenário:** Which of the following are benefits of the AWS Web Application Firewall (AWS WAF)? (Select two)

**Resposta:**
- AWS Web Application Firewall (AWS WAF) can block all requests except the ones that you allow
- AWS Web Application Firewall (AWS WAF) can check for the presence of SQL code that is likely to be malicious (known as SQL injection)

---

### AWS Systems Manager

#### USE CASE 1
**Cenário:** The DevOps team at an IT company wants to centrally manage its servers on AWS Cloud as well as on-premise data center so that it can collect software inventory, run commands, configure and patch servers at scale. As a Cloud Practitioner, which AWS service would you recommend for this use-case?

**Resposta:** AWS Systems Manager

---

## Storage

### Amazon S3 (Simple Storage Service)

#### USE CASE 1
**Cenário:** A web application stores all of its data on Amazon S3 buckets. A client has mandated that data be encrypted before sending it to Amazon S3. Which of the following is the right technique for encrypting data as needed by the customer?

**Resposta:** Enable client-side encryption using AWS encryption SDK

#### USE CASE 2
**Cenário:** A company needs a storage solution for a project wherein the data is accessed less frequently but needs rapid access when required. Which S3 storage class is the MOST cost-effective for the given use-case?

**Resposta:** Amazon S3 Standard-Infrequent Access (S3 Standard-IA)

#### USE CASE 3
**Cenário:** Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is file based storage.

**Resposta:** Understanding storage types - S3 (object), EBS (block), EFS (file)

#### USE CASE 4
**Cenário:** A medical device company is looking for a durable and cost-effective way of storing their historic data. Due to compliance requirements, the data must be stored for 10 years. Which AWS Storage solution will you suggest?

**Resposta:** Amazon S3 Glacier Deep Archive

#### USE CASE 5
**Cenário:** Which of the following AWS services have data encryption automatically enabled? (Select two)

**Resposta:**
- AWS Storage Gateway
- Amazon Simple Storage Service (Amazon S3)

#### USE CASE 6
**Cenário:** Which of the following is the best way to protect your data from accidental deletion on Amazon S3?

**Resposta:** Amazon S3 Versioning

#### USE CASE 7
**Cenário:** An IT company has deployed a static website on Amazon Simple Storage Service (Amazon S3), but the website is still inaccessible. As a Cloud Practioner, which of the following solutions would you suggest to address this issue?

**Resposta:** Fix the Amazon S3 bucket policy

#### USE CASE 8
**Cenário:** A financial services company must meet compliance requirements that mandate storing multiple copies of data in geographically distant locations. As the company uses Amazon Simple Storage Service (Amazon S3) as its main storage service, which of the following represents the MOST resource-efficient solution for this use-case?

**Resposta:** Use S3 cross-region replication (S3 CRR) to replicate data between distant AWS Regions

#### USE CASE 9
**Cenário:** A financial services company wants to ensure that all customer data uploaded on its data lake on Amazon Simple Storage Service (Amazon S3) always stays private. Which of the following is the MOST efficient solution to address this compliance requirement?

**Resposta:** Use Amazon S3 Block Public Access to ensure that all Amazon S3 resources stay private

#### USE CASE 10
**Cenário:** Which AWS service can be used to host a static website with the LEAST effort?

**Resposta:** Amazon Simple Storage Service (Amazon S3)

#### USE CASE 11
**Cenário:** Which of the following Amazon Simple Storage Service (Amazon S3) storage classes do not charge any data retrieval fee? (Select two)

**Resposta:**
- Amazon S3 Standard
- Amazon S3 Intelligent-Tiering

#### USE CASE 12
**Cenário:** A media company uploads its media (audio and video) files to a centralized Amazon Simple Storage Service (Amazon S3) bucket from geographically dispersed locations. Which of the following solutions can the company use to optimize transfer speeds?

**Resposta:** Amazon S3 Transfer Acceleration (S3TA)

#### USE CASE 13
**Cenário:** Which of the following AWS services offers Lifecycle configuration for cost-optimal storage?

**Resposta:** Amazon Simple Storage Service (Amazon S3)

#### USE CASE 14
**Cenário:** A firm wants to maintain the same data on Amazon Simple Storage Service (Amazon S3) between its production account and multiple test accounts. Which technique should you choose to copy data into multiple test accounts while retaining object metadata?

**Resposta:** Amazon S3 Replication

#### USE CASE 15
**Cenário:** Which of the following statements are true regarding Amazon Simple Storage Service (Amazon S3)? (Select two)

**Resposta:**
- Amazon Simple Storage Service (Amazon S3) is a key value based object storage service
- Amazon Simple Storage Service (Amazon S3) stores data in a flat non-hierarchical structure

#### USE CASE 16
**Cenário:** Which of the following Amazon Simple Storage Service (Amazon S3) storage classes has NO constraint of a minimum storage duration charge for objects?

**Resposta:** Amazon S3 Standard

---

### Amazon EBS (Elastic Block Store)

#### USE CASE 1
**Cenário:** EBS volume can be attached to a single instance in the same Availability Zone (AZ).

**Resposta:** Understanding EBS attachment constraints - single AZ, single instance (except Multi-Attach for io1/io2)

#### USE CASE 2
**Cenário:** AWS Compute Optimizer delivers recommendations for which of the following AWS resources? (Select three)

**Resposta:**
- Amazon EC2 instances
- Amazon EBS volumes
- AWS Lambda functions

#### USE CASE 3
**Cenário:** Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is file based storage.

**Resposta:** Understanding storage types

#### USE CASE 4
**Cenário:** Which of the following AWS services offer block-level storage?

**Resposta:** Amazon Elastic Block Store (Amazon EBS)

---

### Amazon EFS (Elastic File System)

#### USE CASE 1
**Cenário:** A data analytics company is running a proprietary batch analytics application on AWS and wants to use a storage service which would be accessed by hundreds of EC2 instances simultaneously to append data to existing files. As a Cloud Practitioner, which AWS service would you suggest for this use-case?

**Resposta:** Amazon Elastic File System (Amazon EFS)

#### USE CASE 2
**Cenário:** Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is file based storage.

**Resposta:** Understanding storage types

#### USE CASE 3
**Cenário:** A fleet of Amazon EC2 instances spread across different Availability Zones (AZ) needs to access, edit and share file-based data stored centrally on a system. As a Cloud Practitioner, which AWS service would you recommend for this use-case?

**Resposta:** Amazon Elastic File System (Amazon EFS)

#### USE CASE 4
**Cenário:** Which of the following statements is correct regarding the Amazon Elastic File System (Amazon EFS) storage service?

**Resposta:** EC2 instances can access files on an Amazon Elastic File System (Amazon EFS) file system across many Availability Zones (AZ), Regions and VPCs

#### USE CASE 5
**Cenário:** Which of the following use cases is best suited for Amazon EFS Standard-Infrequent Access (EFS Standard-IA) storage class?

**Resposta:** Storing files in an accessible location to satisfy audit requirements

#### USE CASE 6
**Cenário:** Which AWS services/features support High Availability by default? (Select two)

**Resposta:**
- Amazon Elastic File System (Amazon EFS)
- Amazon DynamoDB

#### USE CASE 7
**Cenário:** Which of the following AWS storage services can be directly used with on-premises systems?

**Resposta:** Amazon Elastic File System (Amazon EFS)

---

### Amazon FSx for Windows File Server

#### USE CASE 1
**Cenário:** A company wants a fully managed, flexible, and scalable file storage system, with low latency access, for its Windows-based applications. Which AWS service is the right choice for the company?

**Resposta:** Amazon FSx for Windows File Server

---

### AWS Snowball

#### USE CASE 1
**Cenário:** Which AWS service will you use if you have to move large volumes of on-premises data to AWS Cloud from a remote location with limited bandwidth?

**Resposta:** AWS Snowball

#### USE CASE 2
**Cenário:** Which of the following AWS services specialize in data migration from on-premises to AWS Cloud? (Select two)

**Resposta:**
- AWS Snowball
- AWS Database Migration Service (AWS DMS)

---

### AWS Storage Gateway

#### USE CASE 1
**Cenário:** What are the different gateway types supported by AWS Storage Gateway service?

**Resposta:** Tape Gateway, File Gateway and Volume Gateway

#### USE CASE 2
**Cenário:** Which of the following AWS services have data encryption automatically enabled? (Select two)

**Resposta:**
- AWS Storage Gateway
- Amazon Simple Storage Service (Amazon S3)

---

## Networking

### Amazon Route 53

#### USE CASE 1
**Cenário:** Which AWS Route 53 routing policy would you use to route traffic to multiple resources and also choose how much traffic is routed to each resource?

**Resposta:** Weighted routing

#### USE CASE 2
**Cenário:** AWS Shield Advanced provides expanded DDoS attack protection for web applications running on which of the following resources? (Select two)

**Resposta:**
- AWS Global Accelerator
- Amazon Route 53

#### USE CASE 3
**Cenário:** Which Amazon Route 53 routing policy would you use to improve the performance for your customers by routing the requests to the AWS endpoint that provides the fastest experience?

**Resposta:** Latency-based routing

#### USE CASE 4
**Cenário:** Which of the following AWS services can be used to prevent Distributed Denial-of-Service (DDoS) attack? (Select three)

**Resposta:**
- AWS Shield
- AWS Web Application Firewall (AWS WAF)
- Amazon CloudFront with Amazon Route 53

#### USE CASE 5
**Cenário:** Which Amazon Route 53 routing policy would you use to route traffic to a single resource such as a web server for your website?

**Resposta:** Simple routing

---

### AWS Global Accelerator

#### USE CASE 1
**Cenário:** AWS Shield Advanced provides expanded DDoS attack protection for web applications running on which of the following resources? (Select two)

**Resposta:**
- AWS Global Accelerator
- Amazon Route 53

#### USE CASE 2
**Cenário:** Which AWS service helps with global application availability and performance using the AWS global network?

**Resposta:** AWS Global Accelerator

#### USE CASE 3
**Cenário:** Which of the following statements are CORRECT regarding AWS Global Accelerator? (Select two)

**Resposta:**
- AWS Global Accelerator provides static IP addresses that act as a fixed entry point to your applications
- AWS Global Accelerator is a good fit for non-HTTP use cases

---

### AWS Virtual Private Network (VPN)

#### USE CASE 1
**Cenário:** Which of the following solutions can you use to connect your on-premises network with AWS Cloud? (Select two)

**Resposta:**
- AWS Virtual Private Network (VPN)
- AWS Direct Connect

#### USE CASE 2
**Cenário:** Which of the following are components of an AWS Site-to-Site VPN? (Select two)

**Resposta:**
- Customer gateway
- Virtual private gateway (VGW)

---

### AWS Transit Gateway

#### USE CASE 1
**Cenário:** An organization needs to securely access AWS services and establish private connectivity between its Virtual Private Clouds (VPCs) and supported AWS services without using the public internet. Which AWS services can meet this requirement? (Select two)

**Resposta:**
- AWS PrivateLink
- AWS Transit Gateway

#### USE CASE 2
**Cenário:** An organization maintains separate Amazon Virtual Private Clouds (Amazon VPC) for each of its departments. With expanding business, the organization now wants to connect all Amazon Virtual Private Clouds (Amazon VPC) for better departmental collaboration. Which AWS service will help the organization tackle the issue effectively?

**Resposta:** AWS Transit Gateway

#### USE CASE 3
**Cenário:** A multi-national organization has a separate virtual private cloud (VPC) for each of its business units on the AWS Cloud. The organization also wants to connect its on-premises data center with the different virtual private clouds (VPC) for better organization-wide collaboration. Which AWS services can be combined to build the MOST efficient solution for this use-case? (Select two)

**Resposta:**
- AWS Transit Gateway
- AWS Direct Connect

---

## Serverless

### AWS Lambda

#### USE CASE 1
**Cenário:** An IT company wants to run a log backup process every Monday at 2 AM. The usual runtime of the process is 5 minutes. As a Cloud Practitioner, which AWS services would you recommend to build a serverless solution for this use-case? (Select two)

**Resposta:**
- Amazon EventBridge
- AWS Lambda

#### USE CASE 2
**Cenário:** Which of the following statements are true about AWS Lambda? (Select two)

**Resposta:**
- AWS Lambda lets you run code without provisioning or managing servers
- You pay for the compute time you consume for AWS Lambda

#### USE CASE 3
**Cenário:** AWS Compute Optimizer delivers recommendations for which of the following AWS resources? (Select three)

**Resposta:**
- Amazon EC2 instances
- Amazon EBS volumes
- AWS Lambda functions

#### USE CASE 4
**Cenário:** Under the AWS Shared Responsibility Model, which of the following is the responsibility of a customer regarding AWS Lambda?

**Resposta:** Maintain versions of an AWS Lambda function

---

## Developer Tools

### AWS X-Ray

#### USE CASE 1
**Cenário:** The DevOps team at an e-commerce company is trying to debug performance issues for its serverless application built using a microservices architecture.

**Resposta:** AWS X-Ray (for tracing and analyzing distributed applications)

---

### AWS CodeDeploy

#### USE CASE 1
**Cenário:** Which AWS service can be used to automate code deployment to Amazon Elastic Compute Cloud (Amazon EC2) instances as well as on-premises instances?

**Resposta:** AWS CodeDeploy

#### USE CASE 2
**Cenário:** Which AWS service will help you deploy application code automatically to an Amazon Elastic Compute Cloud (Amazon EC2) instance?

**Resposta:** AWS CodeDeploy

---

### AWS Device Farm

#### USE CASE 1
**Cenário:** The QA team at a company wants a tool/service that can provide access to different mobile devices with variations in firmware and Operating System versions. Which AWS service can address this use case?

**Resposta:** AWS Device Farm

---

## Search & Analytics

### Amazon Kendra

#### USE CASE 1
**Cenário:** A leading research firm needs to access information available in old patents and documents (such as PDFs, Text Files, Word documents, etc) present in its huge knowledge base. The firm is looking for a powerful search tool that can dig into these knowledge resources and return the most relevant files/documents. Which of the following is the correct service to address this requirement?

**Resposta:** Amazon Kendra

**Nota:** Amazon Kendra's deep learning models come pre-trained across 14 industry domains for intelligent search.

---

## Management & Governance

### AWS Trusted Advisor

Casos de uso a serem adicionados após leitura completa do arquivo.

---

## Messaging

### Amazon SNS (Simple Notification Service)

Casos de uso a serem adicionados após leitura completa do arquivo.

---

## 📊 Estatísticas

- **Total de Categorias:** 8
- **Total de Serviços Documentados:** 21+
- **Total de Use Cases:** 80+

---

## 📝 Notas Importantes

1. **Encryption por Default:**
   - Amazon S3 - Sim (SSE-S3)
   - AWS CloudTrail - Sim
   - AWS Storage Gateway - Sim

2. **High Availability por Default:**
   - Amazon EFS - Sim
   - Amazon DynamoDB - Sim

3. **Storage Types:**
   - **Object:** Amazon S3
   - **Block:** Amazon EBS
   - **File:** Amazon EFS, Amazon FSx

4. **VPC Gateway Endpoint Support:**
   - Amazon S3
   - Amazon DynamoDB
   - (Apenas estes dois serviços suportam VPC Gateway Endpoint - sem custo adicional)

5. **DDoS Protection Services:**
   - AWS Shield
   - AWS WAF
   - Amazon CloudFront + Route 53

---

## 🔄 Última Atualização

Data: 09/01/2026
Fonte: Arquivos de estudo AWS - workspace pessoal

---

*Este documento é uma consolidação de referência e não substitui a documentação oficial da AWS.*
