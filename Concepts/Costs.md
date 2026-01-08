
There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer.

![[Pasted image 20250716084410.png]]



### Data transfer between S3 and EC2 instances within the same region is not charged

There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer. In most cases, there is no charge for inbound data transfer or data transfer between other AWS services within the same region. Outbound data transfer is aggregated across services and then charged at the outbound data transfer rate.

Per AWS pricing, data transfer between S3 and EC2 instances within the same region is not charged, so there would be no data transfer charge for moving 500 GB of data from an EC2 instance to an S3 bucket in the same region.

## USE CASE

Which of the following statement is correct regarding the AWS pricing policy for data transfer charges into or out of an AWS Region?

Only outbound data transfer is charged

## USE CASE

What are the fundamental drivers of cost with AWS Cloud?

Compute, Storage and Outbound Data Transfer

## USE CASE

A startup has just moved its IT infrastructure to AWS Cloud. The CTO would like to receive detailed reports that break down the startup's AWS costs by the hour in an Amazon Simple Storage Service (Amazon S3) bucket. As a Cloud Practitioner, which AWS service would you recommend for this use-case?

AWS Cost & Usage Report (AWS CUR)

## USE CASE

Which of the following AWS services can be used to forecast your AWS account usage and costs?

AWS Cost Explorer