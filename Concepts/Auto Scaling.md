**Auto Scaling group scales out and adds more number of Amazon EC2 instances to match an increase in demand**

**Auto Scaling group scales in and reduces the number of Amazon EC2 instances to match a decrease in demand**

![[Pasted image 20260106140604.png]]

AWS Auto Scaling monitors your applications and automatically adjusts the capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it's easy to setup application scaling for multiple resources across multiple services in minutes. The service provides a simple, powerful user interface that lets you build scaling plans for resources including [Amazon EC2](../Services/EC2.md) instances and Spot Fleets, [Amazon ECS](../Services/ECS%20-%20Amazon%20Elastic%20Container%20Service%20-%20%20Fargate%20launch%20type.md) tasks, [Amazon DynamoDB](../Services/DynamoDb.md) tables and indexes, and Amazon Aurora Replicas.

You can use scaling policies to increase or decrease the number of instances in your group dynamically to meet changing conditions. When the scaling policy is in effect, the Auto Scaling group adjusts the desired capacity of the group, between the minimum and maximum capacity values that you specify, and launches or terminates the instances as needed. You can also scale on a schedule.


## USE CASE

Which of the following AWS services are always free to use (Select two)?

AWS Auto Scaling
AWS Identity and Access Management (AWS IAM)


## USE CASE

Which of the following are examples of Horizontal Scalability (aka Elasticity)?

Elastic Load Balancing (ELB)
Read Replicas in Amazon Relational Database Service (Amazon RDS)



**High Availability** - A system that is available is capable of delivering the designed functionality at a given point in time. Highly available systems are those that can withstand some measure of degradation while still remaining available. On AWS Cloud, you can run instances for an application in a multi-AZ deployment to achieve High Availability.

**Scale out** - The scale out (horizontal scaling) operation refers to an increase in capacity by adding more computers to the system. This is in contrast to a "scale up" operation, which is constrained to running its processes on only one computer; in such systems, the only way to increase performance is to add more resources into one computer in the form of faster (or more) CPUs, memory or storage. Horizontally scalable systems are oftentimes able to outperform vertically scalable systems by enabling parallel execution of workloads and distributing those across many different computers. Auto Scaling Group is an example of Horizontal Scaling on AWS.

**Scale up** - The scale up (vertical scaling) operation implies adding more resources (like CPU, RAM) to a single node or machine. Example- Resizing an instance of EC2.

**Performance Efficiency** - Performance Efficiency is the ability to use computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies



## USE CASE

Which AWS technology/service helps you to scale your resources to match supply with demand while still keeping your cloud solution cost-effective?

AWS Auto Scaling