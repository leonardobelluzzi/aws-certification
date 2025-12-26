
Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. You can add capacity (scale up) to handle compute-heavy tasks, such as monthly or yearly processes, or spikes in website traffic. When usage decreases, you can reduce capacity (scale down) again.

![[Pasted image 20250717082556.png]]

**Instances** - Virtual servers. 

**[Amazon Machine Images (AMIs)](../Storage/Amazon%20Machine%20Image.md)** - Preconfigured templates for your instances that package the components you need for your server (including the operating system and additional software). 

**Instance types** - Various configurations of CPU, memory, storage, networking capacity, and graphics hardware for your instances.

**Amazon EBS volumes** - Persistent storage volumes for your data using [Amazon Elastic Block Store (Amazon EBS)](Technology/Storage/EBS%20-%20Amazon%20Elastic%20Block%20Storage.md). 

**Instance store volumes** - Storage volumes for temporary data that is deleted when you stop, hibernate, or terminate your instance. 

**Key pairs** - Secure login information for your instances. AWS stores the public key and you store the private key in a secure place. 

**Security groups** - A virtual firewall that allows you to specify the protocols, ports, and source IP ranges that can reach your instances, and the destination IP ranges to which your instances can connect.

### Validation

**[Amazon EC2 Auto Scaling](../Concepts/Auto%20Scaling.md)** - Helps ensure you have the correct number of Amazon EC2 instances available to handle the load for your application. 

**AWS Backup** - Automate backing up your Amazon EC2 instances and the [Amazon EBS](Technology/Storage/EBS%20-%20Amazon%20Elastic%20Block%20Storage.md) volumes attached to them. 

**[Amazon CloudWatch](CloudWatch.md)** - Monitor your instances and [Amazon EBS](Technology/Storage/EBS%20-%20Amazon%20Elastic%20Block%20Storage.md) volumes. Related services 

**[Elastic Load Balancing](ELB%20-%20Elastic%20Load%20Balancing.md)** - Automatically distribute incoming application traffic across multiple instances. 

**Amazon GuardDuty** - Detect potentially unauthorized or malicious use of your EC2 instances. 

**EC2 Image Builder** - Automate the creation, management, and deployment of customized, secure, and up-to-date server images. 

**AWS Launch Wizard** - Size, configure, and deploy AWS resources for third-party applications without having to manually identify and provision individual AWS resources. 

**[AWS Systems Manager](Security%20and%20Compliance/AWS%20Systems%20Manager.md)** - Perform operations at scale on EC2 instances with this secure end-to-end management solution.

### Observation

Support VPC Gateway Endpoint for a private connection from a VPC

**60 seconds**

There is a one-minute minimum charge for Linux based EC2 instances, so this is the correct option.




## Licenses in EC2

Amazon EC2 Dedicated Hosts allow you to use your eligible software licenses from vendors such as Microsoft and Oracle on Amazon EC2. An Amazon EC2 Dedicated Host is a physical server fully dedicated for your use, so you can help address corporate compliance requirements.

![[Pasted image 20250716150508.png]]


Services support reservations to optimize costs

![[Pasted image 20250717094159.png]]

## Reserved instances (RI)

Reserved instances (RI) provide you with significant savings (up to 72%) on your Amazon Elastic Compute Cloud (Amazon EC2) costs compared to on-demand instance pricing. Reserved Instances (RI) are not physical instances, but rather a billing discount applied to the use of on-demand instances in your account. You can purchase a reserved instance (RI) for a one-year or three-year commitment, with the three-year commitment offering a bigger discount.



**EC2 instances can access files on an Amazon Elastic File System (Amazon EFS) file system across many Availability Zones (AZ), Regions and VPCs**

[Amazon EFS](Technology/Storage/EFS%20-%20Elastic%20File%20System.md) is a regional service storing data within and across multiple Availability Zones (AZs) for high availability and durability. Amazon EC2 instances can access your file system across AZs, regions, and VPCs, while on-premises servers can access using [AWS Direct Connect](AWS%20Direct%20Connect.md) or AWS VPN.


**Spot Instance**

A Spot Instance is an unused EC2 instance that is available for less than the On-Demand price. Because Spot Instances enable you to request unused EC2 instances at steep discounts (up to 90%), you can lower your Amazon EC2 costs significantly. Spot Instances are well-suited for data analysis, batch jobs, background processing, and other flexible tasks that can be interrupted. These can be terminated at short notice, so these are not suitable for critical workloads that need to run at a specific point in time.

**On-Demand Instance** - An On-Demand Instance is an instance that you use on-demand. You have full control over its lifecycle — you decide when to launch, stop, hibernate, start, reboot, or terminate it. There is no long-term commitment required when you purchase On-Demand Instances. There is no upfront payment and you pay only for the seconds that your On-Demand Instances are running. The price per second for running an On-Demand Instance is fixed. On-demand instances cannot be interrupted. However, On-demand instances are not as cost-effective as spot instances, so this option is not correct.

**Reserved Instance (RI)** - Reserved Instances (RI) provide you with significant savings (up to 75%) on your Amazon EC2 costs compared to On-Demand Instance pricing. Reserved Instances (RI) are not physical instances, but rather a billing discount applied to the use of On-Demand Instances in your account. You can purchase a Reserved Instance (RI) for a one-year or three-year commitment, with the three-year commitment offering a bigger discount. Reserved instances (RI) cannot be interrupted. Reserved instances (RI) are not as cost-effective as spot instances, so this option is not correct.

**Dedicated Host** - Amazon EC2 Dedicated Hosts allow you to use your eligible software licenses from vendors such as Microsoft and Oracle on Amazon EC2 so that you get the flexibility and cost-effectiveness of using your licenses, but with the resiliency, simplicity, and elasticity of AWS. An Amazon EC2 Dedicated Host is a physical server fully dedicated for your use, so you can help address corporate compliance requirement. They're not cost-efficient compared to spot instances. So this option is not correct.