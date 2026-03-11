
## TEST 1

### Question 3

A financial services company wants to ensure that its AWS account activity meets the governance, compliance and auditing norms. As a Cloud Practitioner, which AWS service would you recommend for this use-case?

Correct answer: AWS CloudTrail

You can use CloudTrail to log, monitor and retain account activity related to actions across your AWS infrastructure. CloudTrail provides an event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command-line tools, and other AWS services.

Your answer is incorrect: AWS Config

AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources.

### Question 7

Which of the following AWS Support plans provide access to guidance, configuration, and troubleshooting of AWS interoperability with third-party software? (Select two)

Correct selection: AWS Enterprise Support, AWS Business Support

Your selection is incorrect: AWS Corporate Support, AWS Developer Support, AWS Basic Support

### Question 8

Which of the following AWS services support VPC Gateway Endpoint for a private connection from a VPC? (Select two)

Correct selection: Amazon Simple Storage Service (Amazon S3), Amazon DynamoDB

Your selection is incorrect: Amazon Elastic Compute Cloud (Amazon EC2)


A VPC endpoint enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered by AWS PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection. Instances in your VPC do not require public IP addresses to communicate with resources in the service.

A gateway endpoint is a gateway that you specify as a target for a route in your route table for traffic destined to a supported AWS service. The following AWS services are supported:

Amazon Simple Storage Service (Amazon S3) & Amazon DynamoDB

### Question 9

An organization is currently operating MySQL databases on its own on-premises servers. To reduce the operational burden of database maintenance and management, the organization wants to move to a fully managed AWS database offering.

Which migration strategy best aligns with this goal?

Correct answer: Replatform

Your answer is incorrect: Rehost

Replatforming is the most suitable strategy here. It involves moving to a cloud environment with some optimizations, such as switching from a self-managed MySQL database to a managed service like Amazon RDS for MySQL, reducing operational overhead without major changes to the application.

Rehosting involves moving applications to the cloud without making changes to the architecture. While it’s fast, it typically means continuing to manage the database yourself on Amazon EC2 or similar services—not adopting a managed service.

### Question 13

Which of the following AWS services has encryption enabled by default?

Correct answer: AWS CloudTrail Logs

AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. AWS CloudTrail can be used to record AWS API calls and other activity for your AWS account and save the recorded information to log files in an Amazon Simple Storage Service (Amazon S3) bucket that you choose.

### Question 16

Which of the following is the MOST cost-effective option to purchase an EC2 Reserved Instance (RI)?

Correct answer: Partial upfront payment option with standard 3-years term

Your answer is incorrect: No upfront payment option with standard 3-years term

Partial -> ANTECIPADO
No upfront -> PARCELADO

### Question 21

A web application stores all of its data on Amazon S3 buckets. A client has mandated that data be encrypted before sending it to Amazon S3.

Which of the following is the right technique for encrypting data as needed by the customer?

Correct answer: Enable client-side encryption using AWS encryption SDK

The act of encrypting data before sending it to Amazon S3 is termed as client-side encryption. The AWS encryption SDK is a client-side encryption library that is separate from the language–specific SDKs.

### Question 22

Which of the following are correct statements regarding the AWS Global Infrastructure? (Select two)

Your selection is correct: Each Availability Zone (AZ) consists of one or more discrete data centers

Correct selection: Each AWS Region consists of a minimum of three Availability Zones (AZ)

### Question 24

A company wants to improve the resiliency of its flagship application so it wants to move from its traditional database system to a managed AWS NoSQL database service to support active-active configuration in both the East and West US AWS regions. The active-active configuration with cross-region support is the prime criteria for any database solution that the company considers.

Which AWS database service is the right fit for this requirement?

Correct answer: Amazon DynamoDB with global tables

Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-region replication, in-memory caching, and data export tools.

### Question 26

Which of the following AWS Support plans provide access to only core checks from the AWS Trusted Advisor Best Practice Checks? (Select two)

Correct selection: AWS Developer Support, AWS Basic Support

**AWS Basic Support**

The AWS Basic Support plan only provides access to the following:

Customer Service & Communities - 24x7 access to customer service, documentation, whitepapers, and support forums. AWS Trusted Advisor - Access to the core Trusted Advisor checks and guidance to provision your resources following best practices to increase performance and improve security. AWS Health - Your Account Health Dashboard : A personalized view of the health of your AWS services, and alerts when your resources are impacted.

**AWS Developer Support**

You should use the AWS Developer Support plan if you are testing or doing early development on AWS and want the ability to get email-based technical support during business hours as well as general architectural guidance as you build and test. This plan provides access to just the core Trusted Advisor checks from the Service Quota and basic Security checks.

### Question 27Incorrect

A company needs a storage solution for a project wherein the data is accessed less frequently but needs rapid access when required. Which S3 storage class is the MOST cost-effective for the given use-case?

Correct answer: Amazon S3 Standard-Infrequent Access (S3 Standard-IA)

Amazon S3 Standard-Infrequent Access (S3 Standard-IA) is for data that is accessed less frequently, but requires rapid access when needed. S3 Standard-IA offers the high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee. This combination of low cost and high performance make S3 Standard-IA ideal for long-term storage, backups, and as a data store for disaster recovery files.

Correct option: **Amazon S3 Standard-Infrequent Access (S3 Standard-IA)**

Amazon S3 Standard-Infrequent Access (S3 Standard-IA) is for data that is accessed less frequently, but requires rapid access when needed. S3 Standard-IA offers the high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee.

Your answer is incorrect: Amazon S3 Intelligent-Tiering (S3 Intelligent-Tiering)

The Amazon S3 Intelligent-Tiering storage class is designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead. It works by storing objects in two access tiers: one tier that is optimized for frequent access and another lower-cost tier that is optimized for infrequent access. S3 Intelligent-Tiering would turn out to be costlier than S3 Standard-IA for the given use-case, so this option is not correct.

### Question 28

A company uses reserved EC2 instances across multiple units with each unit having its own AWS account. However, some of the units under-utilize their reserved instances while other units need more reserved instances. As a Cloud Practitioner, which of the following would you recommend as the most cost-optimal solution?

Correct answer: Use AWS Organizations to manage AWS accounts of all units and then share the reserved EC2 instances amongst all units

![[Pasted image 20260311085846.png]]


### Question 29

A unicorn startup is building an analytics application with support for a speech-based interface. The application will accept speech-based input from users and then convey results via speech. As a Cloud Practitioner, which solution would you recommend for the given use-case?

Correct answer: Use Amazon Transcribe to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech

Tools:
- You can use Amazon Polly to turn text into lifelike speech thereby allowing you to create applications that talk.
- Amazon Translate is used for language translation.
- You can use Amazon Transcribe to add speech-to-text capability to your applications.


### Question 46

A silicon valley based healthcare startup stores anonymized patient health data on Amazon S3. The CTO further wants to ensure that any sensitive data on S3 is discovered and identified to prevent any sensitive data leaks. As a Cloud Practitioner, which AWS service would you recommend addressing this use-case?

Correct answer: Amazon Macie

![[Pasted image 20260311090819.png]]


### Question 48

Which of the following are the advantages of cloud computing? (Select three)

Your selection is correct

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

### Question 56

Which of the following AWS services support reservations to optimize costs? (Select three)

Amazon Elastic Compute Cloud (Amazon EC2)
Amazon Relational Database Service (Amazon RDS)
Amazon DynamoDB

## TEST 2

### Question 2

Which of the following statement is correct for a Security Group and a Network Access Control List (Network ACL)?

Correct answer: Security Group acts as a firewall at the instance level whereas Network Access Control List (Network ACL) acts as a firewall at the subnet level

![[Pasted image 20260311091908.png]]

![[Pasted image 20260311091924.png]]


### Question 7

Which of the following AWS services is essential for implementing security of resources in AWS Cloud?

Correct answer: AWS Identity and Access Management (IAM)

### Question 8

A gaming company is looking at a technology/service that can deliver a consistent low-latency gameplay to ensure a great user experience for end-users in various locations.

Which AWS technology/service will provide the necessary low-latency access to the end-users?

Correct answer: AWS Local Zones 

AWS Local Zones allow you to use select AWS services, like compute and storage services, closer to more end-users, providing them very low latency access to the applications running locally.

**AWS Edge Locations** - An AWS Edge location is a site that CloudFront uses to cache copies of the content for faster delivery to users at any location.

### Question 11

Which of the following is the correct statement regarding the AWS Storage services?

Correct answer: Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is file based storage


### Question 12

Which Amazon Elastic Compute Cloud (Amazon EC2) pricing model is the most cost-effective and flexible with no requirement for a long term resource commitment or upfront payment but still guarantees that instance would not be interrupted?

Correct answer: On-demand Instance

### Question 20

A data analytics company stores its data on Amazon Simple Storage Service (Amazon S3) and wants to do SQL based analysis on this data with minimum effort. As a Cloud Practitioner, which of the following AWS services will you suggest for this use case?

Correct answer: Amazon Athena

### Question 26

Which of the following options can be used to access and manage all AWS services (Select three)?

Correct selection:
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


### Question 29

What are the different gateway types supported by AWS Storage Gateway service?

Correct answer: Tape Gateway, File Gateway and Volume Gateway

### Question 35

A company's flagship application runs on a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances. As per the new policies, the system administrators are looking for the best way to provide secure shell access to Amazon Elastic Compute Cloud (Amazon EC2) instances without opening new ports or using public IP addresses.

Which tool/service will help you achieve this requirement?

Correct answer: AWS Systems Manager Session Manager

### Question 36

An e-commerce company wants to assess its applications deployed on Amazon Elastic Compute Cloud (Amazon EC2) instances for vulnerabilities and deviations from AWS best practices. Which AWS service can be used to facilitate this?

Correct answer: Amazon Inspector

### Question 55Incorrect

Which of the following solutions can you use to connect your on-premises network with AWS Cloud (Select two)?

Correct selection:

- AWS Virtual Private Network (VPN)
- AWS Direct Connect

![[Pasted image 20260311093048.png]]


### Question 56

According to the AWS Shared Responsibility Model, which of the following are responsibilities of the customer for Amazon RDS?

Correct answer: Database encryption

### Question 58

A retail company has multiple AWS accounts for each of its departments. Which of the following AWS services can be used to set up consolidated billing and a single payment method for these AWS accounts?

Correct answer: AWS Organizations

### Question 59

AWS Compute Optimizer delivers recommendations for which of the following AWS resources? (Select two)

Your selection is correct

- Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon EC2 Auto Scaling groups
- Amazon Elastic Block Store (Amazon EBS), AWS Lambda functions

### Question 64

Which policy describes prohibited uses of the web services offered by Amazon Web Services?

Correct answer

**AWS Acceptable Use Policy**

The Acceptable Use Policy describes prohibited uses of the web services offered by Amazon Web Services, Inc. and its affiliates (the “Services”) and the website located at http://aws.amazon.com (the “AWS Site”). This policy is present at https://aws.amazon.com/aup/ and is updated on a need basis by AWS.

**AWS Trusted Advisor** - AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. 

**AWS Fair Use Policy** - This is a made-up option and has been added as a distractor.

**AWS Applicable Use Policy** - This is a made-up option and has been added as a distractor.