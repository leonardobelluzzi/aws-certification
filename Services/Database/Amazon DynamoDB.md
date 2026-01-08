## 📋 Visão Geral

Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability.

---

## 🔌 VPC Gateway Endpoint Support

⭐ **Amazon DynamoDB is one of only TWO services that support VPC Gateway Endpoint**

- ✅ [Amazon S3](../../Storage/S3.md)
- ✅ [Amazon DynamoDB](Amazon%20DynamoDB.md)

**Benefits of using VPC Gateway Endpoint for DynamoDB:**
- 🆓 **No additional cost** (Gateway Endpoints are free)
- 🔒 **Private connectivity** - Traffic doesn't leave AWS network
- 🚀 **Better performance** - Lower latency
- 💰 **Cost savings** - No NAT Gateway charges
- ✅ **Perfect for Lambda in VPC** accessing DynamoDB

**Exam Alert:** Remember that only S3 and DynamoDB support VPC Gateway Endpoint. All other AWS services use VPC Interface Endpoint (which has a cost).

For more details, see [VPC Endpoints](../../VPC%20-.md).

---


Amazon DynamoDB with global tables

Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-region replication, in-memory caching, and data export tools.

## USE CASE

A company wants to improve the resiliency of its flagship application so it wants to move from its traditional database system to a managed AWS NoSQL database service to support active-active configuration in both the East and West US AWS regions. The active-active configuration with cross-region support is the prime criteria for any database solution that the company considers.

Which AWS database service is the right fit for this requirement?

Amazon DynamoDB with global tables

## USE CASE

Which of the following AWS services support reservations to optimize costs?

**Amazon Elastic Compute Cloud (Amazon EC2)**
**Amazon DynamoDB**
**Amazon Relational Database Service (Amazon RDS)**

## USE CASE

An e-commerce company wants to store data from a recommendation engine in a database. As a Cloud Practioner, which AWS service would you recommend to provide this functionality with the LEAST operational overhead for any scale?

Amazon DynamoDB

## USE CASE 

Which of the following AWS services allows a database to have flexible schema and supports document data models?

Amazon DynamoDB

## 💰 Reserved Capacity

Services support reservations to optimize costs

## USE CASE

Which of the following entities should be used for an Amazon Elastic Compute Cloud (Amazon EC2) Instance to access a DynamoDB table?

IAM role