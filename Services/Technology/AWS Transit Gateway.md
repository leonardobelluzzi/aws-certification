
AWS Transit Gateway is a highly scalable service that connects multiple [VPCs](VPC%20-.md) and on-premises networks through a central hub. It facilitates secure, private connectivity between [VPCs](VPC%20-.md) and supported services without using the public internet.

Transit Gateway enables customers to connect thousands of [VPCs](VPC%20-.md). You can attach all your hybrid connectivity (VPN and [Direct Connect](../../AWS%20Direct%20Connect.md) connections) to a single gateway, consolidating and controlling your organization's entire AWS routing configuration in one place (refer to the following figure). Transit Gateway controls how traffic is routed among all the connected spoke networks using route tables. This hub-and-spoke model simplifies management and reduces operational costs because [VPCs](VPC%20-.md) only connect to the Transit Gateway instance to gain access to the connected networks.

![](https://docs.aws.amazon.com/images/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/images/hub-and-spoke-design.png)

