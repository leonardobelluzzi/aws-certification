
**VPC peering connection** - A VPC peering connection is a networking connection between two [Amazon Virtual Private Clouds (Amazon VPC)](../Services/Technology/VPC%20-.md) that enables you to route traffic between them privately. VPC peering connection is not transitive, a separate VPC peering connection has to be made between two VPCs that need to talk to each other. With growing VPCs, this gets difficult to manage.

Transitive VPC peering connection is not allowed: 

![](https://docs.aws.amazon.com/vpc/latest/peering/images/transitive-peering-diagram.png)

 via - [https://docs.aws.amazon.com/vpc/latest/peering/invalid-peering-configurations.html](https://docs.aws.amazon.com/vpc/latest/peering/invalid-peering-configurations.html)