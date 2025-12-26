
AWS PrivateLink enables private connectivity between [VPCs](Technology/VPC%20-.md) and supported AWS services without traffic traversing the public internet. It ensures secure communication for applications and services.

In the following diagram, the VPC on the left has several Amazon EC2 instances in a private subnet and five VPC endpoints - three interface VPC endpoints, a resource VPC endpoint and a service-network VPC endpoint. The first interface VPC endpoint connects to an AWS service. The second interface VPC endpoint connects to a service hosted by another AWS account (a VPC endpoint service). The third interface VPC endpoint connects to an AWS Marketplace partner service. The resource VPC endpoint connects to a database. The service network VPC endpoint connects to a service network.

![](https://docs.aws.amazon.com/images/vpc/latest/privatelink/images/use-cases.png)