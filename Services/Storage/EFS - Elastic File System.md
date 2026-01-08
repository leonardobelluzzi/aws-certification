Amazon Elastic File System (Amazon EFS) is a cloud-native fully managed file system that provides simple, scalable, elastic file storage accessible from Linux instances via the NFS protocol.

![[Pasted image 20251006080616.png]]

Amazon Elastic File System (Amazon EFS) provides serverless, fully elastic file storage so that you can share file data without provisioning or managing storage capacity and performance. Amazon EFS is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files.

The service is designed to be highly scalable, highly available, and highly durable. Amazon EFS file systems store data and metadata across multiple Availability Zones (AZ) in an AWS Region. EFS file system can be mounted on instances across multiple Availability Zones (AZ).

The service is designed to be highly scalable, highly available, and highly durable. Amazon EFS offers the following file system types to meet your availability and durability needs: 

* **Regional (Recommended)** – Regional file systems (recommended) store data redundantly across multiple geographically separated Availability Zones within the same AWS Region. Storing data across multiple Availability Zones provides continuous availability to the data, even when one or more Availability Zones in an AWS Region are unavailable. 

* **One Zone** – One Zone file systems store data within a single Availability Zone. Storing data in a single Availability Zone provides continuous availability to the data. In the unlikely case of the loss or damage to all or part of the Availability Zone, however, data that is stored in these types of file systems might be lost

## EFS Standard-Infrequent Access

The Amazon EFS Standard-Infrequent Access (EFS Standard-IA) storage class reduces storage costs for files that are not accessed every day. It does this without sacrificing the high availability, high durability, elasticity, and POSIX file system access that Amazon Elastic File System (Amazon EFS) provides.

AWS recommends Amazon EFS Standard-Infrequent Access (EFS Standard-IA) storage class if you need your full dataset to be readily accessible and want to automatically save on storage costs for files that are less frequently accessed. Examples include keeping files accessible to satisfy audit requirements, performing historical analysis, or performing backup and recovery. Amazon EFS Standard-Infrequent Access (EFS Standard-IA) storage is compatible with all Amazon EFS features, and is available in all AWS Regions where Amazon EFS is available.


**EC2 instances can access files on an Amazon Elastic File System (Amazon EFS) file system across many Availability Zones (AZ), Regions and VPCs**

Amazon EFS is a regional service storing data within and across multiple Availability Zones (AZs) for high availability and durability. [Amazon EC2](../../EC2.md) instances can access your file system across AZs, regions, and [VPCs](../VPC%20-.md), while on-premises servers can access using [AWS Direct Connect](../../../AWS%20Direct%20Connect.md) or AWS VPN.

## USE CASE

A  data analytics company is running a proprietary batch analytics application on AWS and wants to use a storage service which would be accessed by hundreds of EC2 instances simultaneously to append data to existing files. As a Cloud Practitioner, which AWS service would you suggest for this use-case?

Amazon Elastic File System (Amazon EFS)

## USE CASE

Amazon Simple Storage Service (Amazon S3) is object based storage, 
Amazon Elastic Block Store (Amazon EBS) is block based storage and 
Amazon Elastic File System (Amazon EFS) is file based storage

## USE CASE

A fleet of Amazon EC2 instances spread across different Availability Zones (AZ) needs to access, edit and share file-based data stored centrally on a system. As a Cloud Practitioner, which AWS service would you recommend for this use-case?

Amazon Elastic File System (Amazon EFS)

## USE CASE

Which of the following statements is correct regarding the Amazon Elastic File System (Amazon EFS) storage service?

EC2 instances can access files on an Amazon Elastic File System (Amazon EFS) file system across many Availability Zones (AZ), Regions and VPCs

## USE CASE 

Which of the following use cases is best suited for Amazon EFS Standard-Infrequent Access (EFS Standard-IA) storage class?

Storing files in an accessible location to satisfy audit requirements

## USE CASE

Which AWS services/features support High Availability by default?

Amazon Elastic File System (Amazon EFS)
Amazon DynamoDB