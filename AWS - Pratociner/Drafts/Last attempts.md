
# 📝 AWS Cloud Practitioner - Últimas Tentativas

## 🔵 TEST 1 - Questões com Erros

### **Q3** - Governance & Auditing
**Questão:** A financial services company wants to ensure that its AWS account activity meets the governance, compliance and auditing norms. As a Cloud Practitioner, which AWS service would you recommend for this use-case?

**✅ Resposta Correta:** AWS CloudTrail

**📌 Explicação:**
You can use CloudTrail to log, monitor and retain account activity related to actions across your AWS infrastructure. CloudTrail provides an event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command-line tools, and other AWS services.

**❌ Resposta Incorreta:** AWS Config
- AWS Config is a service that enables you to assess, audit, and evaluate the **configurations** of your AWS resources (not account activity).

---

### **Q7** - AWS Support Plans (Select 2)
**Questão:** Which of the following AWS Support plans provide access to guidance, configuration, and troubleshooting of AWS interoperability with third-party software?

**✅ Respostas Corretas:**
- AWS Enterprise Support
- AWS Business Support

**❌ Seleção Incorreta:**
- AWS Corporate Support (não existe)
- AWS Developer Support
- AWS Basic Support

---

### **Q8** - VPC Gateway Endpoint (Select 2)
**Questão:** Which of the following AWS services support VPC Gateway Endpoint for a private connection from a VPC?

**✅ Respostas Corretas:**
- Amazon S3
- Amazon DynamoDB

**❌ Seleção Incorreta:** Amazon EC2

**📌 Explicação:**
A VPC endpoint enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered by AWS PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection.

**Gateway Endpoint** supports only:
- Amazon S3
- Amazon DynamoDB

---

### **Q9** - Migration Strategy
**Questão:** An organization is currently operating MySQL databases on its own on-premises servers. To reduce the operational burden of database maintenance and management, the organization wants to move to a fully managed AWS database offering. Which migration strategy best aligns with this goal?

**✅ Resposta Correta:** Replatform

**📌 Explicação:**
**Replatforming** is the most suitable strategy here. It involves moving to a cloud environment with some optimizations, such as switching from a self-managed MySQL database to a managed service like Amazon RDS for MySQL, reducing operational overhead without major changes to the application.

**❌ Resposta Incorreta:** Rehost
- **Rehosting** involves moving applications to the cloud without making changes to the architecture. While it's fast, it typically means continuing to manage the database yourself on Amazon EC2 or similar services—not adopting a managed service.

---

### **Q13** - Encryption by Default
**Questão:** Which of the following AWS services has encryption enabled by default?

**✅ Resposta Correta:** AWS CloudTrail Logs

**📌 Explicação:**
AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. AWS CloudTrail can be used to record AWS API calls and other activity for your AWS account and save the recorded information to log files in an Amazon S3 bucket that you choose. **Logs are encrypted by default.**

---

### **Q16** - Reserved Instance Cost Optimization
**Questão:** Which of the following is the MOST cost-effective option to purchase an EC2 Reserved Instance (RI)?

**✅ Resposta Correta:** Partial upfront payment option with standard 3-years term

**❌ Resposta Incorreta:** No upfront payment option with standard 3-years term

**💡 Importante:**
- **Partial upfront** = Pagamento ANTECIPADO (mais desconto)
- **No upfront** = Pagamento PARCELADO (menos desconto)

---

### **Q21** - S3 Client-Side Encryption
**Questão:** A web application stores all of its data on Amazon S3 buckets. A client has mandated that data be encrypted before sending it to Amazon S3. Which of the following is the right technique for encrypting data as needed by the customer?

**✅ Resposta Correta:** Enable client-side encryption using AWS encryption SDK

**📌 Explicação:**
The act of encrypting data **before sending it to Amazon S3** is termed as **client-side encryption**. The AWS encryption SDK is a client-side encryption library that is separate from the language–specific SDKs.

---

### **Q22** - AWS Global Infrastructure (Select 2)
**Questão:** Which of the following are correct statements regarding the AWS Global Infrastructure?

**✅ Respostas Corretas:**
- Each Availability Zone (AZ) consists of one or more discrete data centers
- Each AWS Region consists of a minimum of three Availability Zones (AZ)

---

### **Q24** - DynamoDB Active-Active
**Questão:** A company wants to improve the resiliency of its flagship application so it wants to move from its traditional database system to a managed AWS NoSQL database service to support active-active configuration in both the East and West US AWS regions. The active-active configuration with cross-region support is the prime criteria for any database solution that the company considers. Which AWS database service is the right fit for this requirement?

**✅ Resposta Correta:** Amazon DynamoDB with global tables

**📌 Explicação:**
Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, **automated multi-region replication** (global tables), in-memory caching, and data export tools.

---

### **Q26** - Trusted Advisor Core Checks (Select 2)
**Questão:** Which of the following AWS Support plans provide access to only core checks from the AWS Trusted Advisor Best Practice Checks?

**✅ Respostas Corretas:**
- AWS Developer Support
- AWS Basic Support

**📌 Explicação:**

**AWS Basic Support:**
- Customer Service & Communities - 24x7 access
- AWS Trusted Advisor - Access to **core Trusted Advisor checks** only
- AWS Health Dashboard

**AWS Developer Support:**
- Email-based technical support during business hours
- Access to just the **core Trusted Advisor checks** (Service Quota and basic Security checks)

---

### **Q27** - S3 Storage Class for Infrequent Access
**Questão:** A company needs a storage solution for a project wherein the data is accessed less frequently but needs rapid access when required. Which S3 storage class is the MOST cost-effective for the given use-case?

**✅ Resposta Correta:** Amazon S3 Standard-Infrequent Access (S3 Standard-IA)

**📌 Explicação:**
Amazon S3 Standard-IA is for data that is **accessed less frequently, but requires rapid access when needed**. S3 Standard-IA offers the high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee. This combination of low cost and high performance make S3 Standard-IA ideal for long-term storage, backups, and as a data store for disaster recovery files.

**❌ Resposta Incorreta:** Amazon S3 Intelligent-Tiering
- S3 Intelligent-Tiering automatically moves data between access tiers but would turn out to be **costlier than S3 Standard-IA** for the given use-case.

---

### **Q28** - Reserved Instances Sharing
**Questão:** A company uses reserved EC2 instances across multiple units with each unit having its own AWS account. However, some of the units under-utilize their reserved instances while other units need more reserved instances. As a Cloud Practitioner, which of the following would you recommend as the most cost-optimal solution?

**✅ Resposta Correta:** Use AWS Organizations to manage AWS accounts of all units and then share the reserved EC2 instances amongst all units

**📌 Referência Visual:**
![Reserved Instances Sharing](Pasted%20image%2020260311085846.png)


---

### **Q29** - Speech Interface Application
**Questão:** A unicorn startup is building an analytics application with support for a speech-based interface. The application will accept speech-based input from users and then convey results via speech. As a Cloud Practitioner, which solution would you recommend for the given use-case?

**✅ Resposta Correta:** Use Amazon Transcribe to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech

**💡 Ferramentas AWS:**
- **Amazon Polly** - Turn text into lifelike speech (text-to-speech)
- **Amazon Transcribe** - Add speech-to-text capability to applications
- **Amazon Translate** - Language translation (not for speech)


---

### **Q46** - Data Discovery on S3
**Questão:** A silicon valley based healthcare startup stores anonymized patient health data on Amazon S3. The CTO further wants to ensure that any sensitive data on S3 is discovered and identified to prevent any sensitive data leaks. As a Cloud Practitioner, which AWS service would you recommend addressing this use-case?

**✅ Resposta Correta:** Amazon Macie

**📌 Referência Visual:**
![Amazon Macie](Pasted%20image%2020260311090819.png)


---

### **Q48** - Cloud Computing Advantages (Select 3)
**Questão:** Which of the following are the advantages of cloud computing?

**✅ Respostas Corretas:**
- Go global in minutes and deploy applications in multiple regions around the world with just a few clicks
- Benefit from massive economies of scale
- Trade capital expense for variable expense


### Question 55

A startup wants to provision an EC2 instance for the lowest possible cost for a long-term duration but needs to make sure that the instance would never be interrupted. As a Cloud Practitioner, which of the following options would you recommend?

Correct option: **EC2 Reserved Instance (RI)**

An EC2 Reserved Instance (RI) provides you with significant savings (up to 75%) on your Amazon EC2 costs compared to On-Demand Instance pricing. A Reserved Instance (RI) is not a physical instance, but rather a billing discount applied to the use of On-Demand Instances in your account. You can purchase a Reserved Instance (RI) for a one-year or three-year commitment, with the three-year commitment offering a bigger discount. A reserved instance (RI) cannot be interrupted. So this is the correct option.

**EC2 On-Demand Instance** - An EC2 On-Demand Instance is an instance that you use on-demand. You have full control over its lifecycle — you decide when to launch, stop, hibernate, start, reboot, or terminate it. There is no long-term commitment required when you purchase On-Demand Instances. There is no upfront payment and you pay only for the seconds that your On-Demand Instances are running. The price per second for running an On-Demand Instance is fixed. On-demand instances cannot be interrupted. However, On-demand instances are not as cost-effective as Reserved instances, so this option is not correct.

**EC2 Spot Instance** - An EC2 Spot Instance is an unused EC2 instance that is available for less than the On-Demand price. Because Spot Instances enable you to request unused EC2 instances at steep discounts (up to 90%), you can lower your Amazon EC2 costs significantly. Spot Instances are well-suited for data analysis, batch jobs, background processing, and optional tasks. These can be terminated at short notice, so these are not suitable for critical workloads that need to run at a specific point in time. So this option is not correct for the given use-case.

**EC2 Dedicated Host** - An Amazon EC2 Dedicated Host allows you to use your eligible software licenses from vendors such as Microsoft and Oracle on Amazon EC2 so that you get the flexibility and cost-effectiveness of using your licenses, but with the resiliency, simplicity, and elasticity of AWS. An Amazon EC2 Dedicated Host is a physical server fully dedicated for your use, so you can help address corporate compliance requirement. It is not cost-efficient compared to an On-Demand instance. So this option is not correct.

---

### **Q56** - Services with Reservations (Select 3)
**Questão:** Which of the following AWS services support reservations to optimize costs?

**✅ Respostas Corretas:**
- Amazon EC2
- Amazon RDS
- Amazon DynamoDB

---

## 🔵 TEST 2 - Questões com Erros

### **Q2** - Security Group vs Network ACL
**Questão:** Which of the following statement is correct for a Security Group and a Network Access Control List (Network ACL)?

**✅ Resposta Correta:** Security Group acts as a firewall at the instance level whereas Network Access Control List (Network ACL) acts as a firewall at the subnet level

**📌 Referência Visual:**
![Security Group vs Network ACL - Diagram 1](Pasted%20image%2020260311091908.png)
![Security Group vs Network ACL - Diagram 2](Pasted%20image%2020260311091924.png)


---

### **Q7** - AWS Security Service
**Questão:** Which of the following AWS services is essential for implementing security of resources in AWS Cloud?

**✅ Resposta Correta:** AWS Identity and Access Management (IAM)

---

### **Q8** - Low-Latency Access
**Questão:** A gaming company is looking at a technology/service that can deliver a consistent low-latency gameplay to ensure a great user experience for end-users in various locations. Which AWS technology/service will provide the necessary low-latency access to the end-users?

**✅ Resposta Correta:** AWS Local Zones

**📌 Explicação:**
AWS Local Zones allow you to use select AWS services, like compute and storage services, **closer to more end-users**, providing them **very low latency access** to the applications running locally.

**💡 Diferença:**
- **AWS Edge Locations** - CloudFront uses edge locations to cache copies of content for faster delivery (CDN)

---

### **Q11** - AWS Storage Types
**Questão:** Which of the following is the correct statement regarding the AWS Storage services?

**✅ Resposta Correta:** Amazon S3 is object based storage, Amazon EBS is block based storage and Amazon EFS is file based storage

**💡 Resumo:**
- **Amazon S3** - Object storage
- **Amazon EBS** - Block storage
- **Amazon EFS** - File storage


---

### **Q12** - EC2 Pricing Model
**Questão:** Which Amazon EC2 pricing model is the most cost-effective and flexible with no requirement for a long term resource commitment or upfront payment but still guarantees that instance would not be interrupted?

**✅ Resposta Correta:** On-demand Instance

**📌 Características:**
- No long-term commitment
- No upfront payment
- Flexible
- **Cannot be interrupted** (unlike Spot Instances)

---

### **Q20** - SQL Analysis on S3
**Questão:** A data analytics company stores its data on Amazon S3 and wants to do SQL based analysis on this data with minimum effort. As a Cloud Practitioner, which of the following AWS services will you suggest for this use case?

**✅ Resposta Correta:** Amazon Athena

**📌 Explicação:**
Amazon Athena is an interactive query service that makes it easy to analyze data directly in Amazon S3 using standard SQL. No need to load data or set up infrastructure.

---

### **Q26** - Access and Manage AWS Services (Select 3)
**Questão:** Which of the following options can be used to access and manage all AWS services?

**✅ Respostas Corretas:**
- AWS Software Development Kit (SDK)
- AWS Management Console
- AWS Command Line Interface (AWS CLI)

### Question 27

The AWS Cloud Adoption Framework (AWS CAF) recommends four iterative and incremental cloud transformation phases. Which cloud transformation journey phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on demonstrating how the cloud will help accelerate your business outcomes?

Correct answer: Envision

The Envision phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on demonstrating how the cloud will help accelerate your business outcomes.

**Align** - The Align phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on identifying capability gaps across the six AWS CAF perspectives, identifying cross-organizational dependencies, and surfacing stakeholder concerns and challenges.

**Launch** - The Launch phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on delivering pilot initiatives in production and on demonstrating incremental business value.

**Scale** - The Scale phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on expanding production pilots and business value to desired scale and ensuring that the business benefits associated with your cloud investments are realized and sustained.


---

### **Q29** - Storage Gateway Types
**Questão:** What are the different gateway types supported by AWS Storage Gateway service?

**✅ Resposta Correta:** Tape Gateway, File Gateway and Volume Gateway

**💡 Resumo:**
- **Tape Gateway** - Virtual tape library
- **File Gateway** - File-based storage
- **Volume Gateway** - Block-based storage

---

### **Q35** - Secure Shell Access to EC2
**Questão:** A company's flagship application runs on a fleet of Amazon EC2 instances. As per the new policies, the system administrators are looking for the best way to provide secure shell access to Amazon EC2 instances without opening new ports or using public IP addresses. Which tool/service will help you achieve this requirement?

**✅ Resposta Correta:** AWS Systems Manager Session Manager

**💡 Benefícios:**
- No need to open ports (like SSH port 22)
- No need for public IP addresses
- Secure access via AWS console

---

### **Q36** - Security Assessment
**Questão:** An e-commerce company wants to assess its applications deployed on Amazon EC2 instances for vulnerabilities and deviations from AWS best practices. Which AWS service can be used to facilitate this?

**✅ Resposta Correta:** Amazon Inspector

**📌 Explicação:**
Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. It automatically assesses applications for vulnerabilities and deviations from best practices.

---

### **Q55** - On-Premises to AWS Connectivity (Select 2)
**Questão:** Which of the following solutions can you use to connect your on-premises network with AWS Cloud?

**✅ Respostas Corretas:**
- AWS Virtual Private Network (VPN)
- AWS Direct Connect

**📌 Referência Visual:**
![On-Premises Connectivity](Pasted%20image%2020260311093048.png)


---

### **Q56** - RDS Customer Responsibility
**Questão:** According to the AWS Shared Responsibility Model, which of the following are responsibilities of the customer for Amazon RDS?

**✅ Resposta Correta:** Database encryption

**📌 Explicação:**
For managed services like RDS, AWS manages the infrastructure and OS, but the customer is responsible for:
- Database encryption (at rest and in transit)
- Access control and IAM policies
- Database backup configuration
- Network access control

---

### **Q58** - Consolidated Billing
**Questão:** A retail company has multiple AWS accounts for each of its departments. Which of the following AWS services can be used to set up consolidated billing and a single payment method for these AWS accounts?

**✅ Resposta Correta:** AWS Organizations

**💡 Benefícios:**
- Consolidated billing across multiple accounts
- Single payment method
- Volume discounts
- Cost allocation and tracking

---

### **Q59** - Compute Optimizer Resources (Select 2)
**Questão:** AWS Compute Optimizer delivers recommendations for which of the following AWS resources?

**✅ Respostas Corretas:**
- Amazon EC2 instances, Amazon EC2 Auto Scaling groups
- Amazon EBS, AWS Lambda functions

---

### **Q64** - AWS Policies
**Questão:** Which policy describes prohibited uses of the web services offered by Amazon Web Services?

**✅ Resposta Correta:** AWS Acceptable Use Policy

**📌 Explicação:**
The **Acceptable Use Policy** describes prohibited uses of the web services offered by Amazon Web Services, Inc. and its affiliates. This policy is present at https://aws.amazon.com/aup/ and is updated on a need basis by AWS.

**❌ Opções Incorretas:**
- **AWS Trusted Advisor** - Online tool that provides real-time guidance for provisioning resources following AWS best practices (not a policy)
- **AWS Fair Use Policy** - Made-up option (distractor)
- **AWS Applicable Use Policy** - Made-up option (distractor)

---

## 📊 Resumo Geral

**Total de Questões Revisadas:** 31 questões

### TEST 1: 16 questões
- Governance & Security (CloudTrail, IAM, Macie)
- Storage & Databases (S3, DynamoDB, RDS)
- Cost Optimization (Reserved Instances, Organizations)
- AI/ML Services (Transcribe, Polly, Translate)
- Support Plans & Trusted Advisor

### TEST 2: 15 questões
- Security & Networking (Security Groups, VPN, Direct Connect)
- Storage Services (S3, EBS, EFS)
- Database Services (RDS responsibilities)
- Management Tools (Systems Manager, Inspector)
- AWS CAF & Best Practices
- Cost Management (Organizations, Compute Optimizer)

**🎯 Tópicos Principais:**
- AWS Security & Compliance
- Storage Solutions (S3, EBS, EFS)
- Cost Optimization Strategies
- Networking & Connectivity
- Managed Services & Shared Responsibility
- AWS Support & Governance