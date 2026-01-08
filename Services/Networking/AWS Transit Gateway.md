
AWS Transit Gateway is a highly scalable service that connects multiple [VPCs](Amazon%20VPC%20-%20Virtual%20Private%20Cloud.md) and on-premises networks through a central hub. It facilitates secure, private connectivity between [VPCs](Amazon%20VPC%20-%20Virtual%20Private%20Cloud.md) and supported services without using the public internet.

Transit Gateway enables customers to connect thousands of [VPCs](Amazon%20VPC%20-%20Virtual%20Private%20Cloud.md). You can attach all your hybrid connectivity (VPN and [Direct Connect](../../AWS%20Direct%20Connect.md) connections) to a single gateway, consolidating and controlling your organization's entire AWS routing configuration in one place (refer to the following figure). Transit Gateway controls how traffic is routed among all the connected spoke networks using route tables. This hub-and-spoke model simplifies management and reduces operational costs because [VPCs](Amazon%20VPC%20-%20Virtual%20Private%20Cloud.md) only connect to the Transit Gateway instance to gain access to the connected networks.

![](https://docs.aws.amazon.com/images/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/images/hub-and-spoke-design.png)


## USE CASES

An organization needs to securely access AWS services and establish private connectivity between its Virtual Private Clouds (VPCs) and supported AWS services without using the public internet. Which AWS services can meet this requirement? (Select two)

AWS PrivateLink
AWS Transit Gateway

## USE CASE

An organization maintains separate Amazon Virtual Private Clouds (Amazon VPC) for each of its departments. With expanding business, the organization now wants to connect all Amazon Virtual Private Clouds (Amazon VPC) for better departmental collaboration. Which AWS service will help the organization tackle the issue effectively?

AWS Transit Gateway