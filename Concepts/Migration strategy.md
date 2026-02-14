
### **1. Initial Assessment**

- Analyze the current environment (applications, servers, databases, dependencies).
- Define business goals: cost reduction, scalability, modernization, etc.
- Use tools like **AWS Migration Evaluator** or **AWS Application Discovery Service**.

### **2. The 6 Migration Strategies (6 Rs)**

| Strategy       | Description                                                                                       |
| -------------- | ------------------------------------------------------------------------------------------------- |
| **Rehost**     | "Lift and Shift" – move applications to AWS with minimal or no changes. Example: migrate to EC2.  |
| **Replatform** | Make slight optimizations without changing the core architecture. Example: move databases to RDS. |
| **Repurchase** | Replace with a SaaS solution. Example: switch from custom CRM to Salesforce.                      |
| **Refactor**   | Redesign the application to leverage cloud-native features. Example: use AWS Lambda, DynamoDB.    |
| **Retire**     | Decommission applications that are no longer needed.                                              |
| **Retain**     | Keep some applications on-premises for now.                                                       |



![[Pasted image 20250716145338.png]]

## USE CASE

An enterprise is planning to move one of its older applications from its local data center to AWS. The IT team wants the fastest migration path and has decided not to update the application code or make any architectural changes.

Rehost