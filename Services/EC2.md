
Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. You can add capacity (scale up) to handle compute-heavy tasks, such as monthly or yearly processes, or spikes in website traffic. When usage decreases, you can reduce capacity (scale down) again.

![[Pasted image 20250717082556.png]]

**Instances** - Virtual servers. 

**Amazon Machine Images (AMIs)** - Preconfigured templates for your instances that package the components you need for your server (including the operating system and additional software). 

**Instance types** - Various configurations of CPU, memory, storage, networking capacity, and graphics hardware for your instances.

**Amazon EBS volumes** - Persistent storage volumes for your data using Amazon Elastic Block Store (Amazon EBS). 

**Instance store volumes** - Storage volumes for temporary data that is deleted when you stop, hibernate, or terminate your instance. 

**Key pairs** - Secure login information for your instances. AWS stores the public key and you store the private key in a secure place. 

**Security groups** - A virtual firewall that allows you to specify the protocols, ports, and source IP ranges that can reach your instances, and the destination IP ranges to which your instances can connect.

### Validation

**Amazon EC2 Auto Scaling** - Helps ensure you have the correct number of Amazon EC2 instances available to handle the load for your application. 

**AWS Backup** - Automate backing up your Amazon EC2 instances and the Amazon EBS volumes attached to them. 

**Amazon CloudWatch** - Monitor your instances and Amazon EBS volumes. Related services 

**Elastic Load Balancing** - Automatically distribute incoming application traffic across multiple instances. 

**Amazon GuardDuty** - Detect potentially unauthorized or malicious use of your EC2 instances. 

**EC2 Image Builder** - Automate the creation, management, and deployment of customized, secure, and up-to-date server images. 

**AWS Launch Wizard** - Size, configure, and deploy AWS resources for third-party applications without having to manually identify and provision individual AWS resources. 

**AWS Systems Manager** - Perform operations at scale on EC2 instances with this secure end-to-end management solution.

### Observation

Support VPC Gateway Endpoint for a private connection from a VPC

**60 seconds**

There is a one-minute minimum charge for Linux based EC2 instances, so this is the correct option.




## Licenses in EC2

Amazon EC2 Dedicated Hosts allow you to use your eligible software licenses from vendors such as Microsoft and Oracle on Amazon EC2. An Amazon EC2 Dedicated Host is a physical server fully dedicated for your use, so you can help address corporate compliance requirements.

![[Pasted image 20250716150508.png]]


Services support reservations to optimize costs

![[Pasted image 20250717094159.png]]