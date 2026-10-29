An Amazon Machine Image (AMI) provides the information required to launch an instance. You must specify an Amazon Machine Image (AMI) when you launch an instance.

An Amazon Machine Image (AMI) includes the following:

One or more Amazon Elastic Block Store (Amazon EBS) snapshots, or, for instance store backed AMIs, a template for the root volume of the instance (for example, an operating system, an application server, and applications).

Launch permissions that control which AWS accounts can use the Amazon Machine Image (AMI) to launch instances.

A block device mapping that specifies the volumes to attach to the instance when it's launched.


![[Pasted image 20250930200224.png]]

## USE CASE

A company based in Sydney hosts its application on an Amazon Elastic Compute Cloud (Amazon EC2) instance in ap-southeast-2. They would like to deploy the same Amazon EC2 instances in eu-south-1. Which of the following AWS entities can address this use case?

Amazon Machine Image (AMI)