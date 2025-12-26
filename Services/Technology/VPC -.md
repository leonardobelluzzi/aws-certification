
## VPC Endpoint

A VPC endpoint enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered by [AWS PrivateLink](../../AWS%20PrivateLink.md) without requiring an internet gateway, NAT device, VPN connection, or [AWS Direct Connect](../../AWS%20Direct%20Connect.md) connection. Instances in your VPC do not require public IP addresses to communicate with resources in the service. Traffic between your VPC and the other service does not leave the Amazon network.

There are two types of VPC endpoints: interface endpoints and gateway endpoints.

An interface endpoint is an elastic network interface with a private IP address from the IP address range of your subnet that serves as an entry point for traffic destined to a supported service. Interface endpoints are powered by [AWS PrivateLink](../../AWS%20PrivateLink.md), a technology that enables you to privately access services by using private IP addresses.

A gateway endpoint is a gateway that you specify as a target for a route in your route table for traffic destined to a supported AWS service. The following AWS services are supported:

[Amazon Simple Storage Service (Amazon S3)](Storage/S3.md)

[Amazon DynamoDB](Database/NoSQL/Amazon%20DynamoDB.md)

Exam Alert:

You may see a question around this concept in the exam. Just remember that only [Amazon S3](Storage/S3.md) and [Amazon DynamoDB](Database/NoSQL/Amazon%20DynamoDB.md) support VPC gateway endpoint. All other services that support VPC Endpoints use a VPC interface endpoint (note that [Amazon S3](Storage/S3.md) supports the VPC interface endpoint as well).
![[Pasted image 20250718085045.png]]

![[Pasted image 20250718085136.png]]
