AWS Identity and Access Management (IAM) enables you to manage access to AWS services and resources securely. Using IAM, you can create and manage AWS users and groups, and use permissions to allow and deny their access to AWS resources.




Global in scope


Most policies are stored in AWS as JSON documents. Identity-based policies and policies used to set permissions boundaries are JSON policy documents that you attach to a user or role. Resource-based policies are JSON policy documents that you attach to a resource.

A JSON policy document includes these elements:

1. Optional policy-wide information at the top of the document
2. One or more individual statements

Each statement includes information about a single permission. The information in a statement is contained within a series of elements.

1. Version – Specify the version of the policy language that you want to use. As a best practice, use the latest 2012-10-17 version.
    
2. Statement – Use this main policy element as a container for the following elements. You can include more than one statement in a policy.
    
    1. Sid (Optional) – Include an optional statement ID to differentiate between your statements.
        
    2. Effect – Use Allow or Deny to indicate whether the policy allows or denies access.
        
    3. Principal (Required in only some circumstances) – If you create a resource-based policy, you must indicate the account, user, role, or federated user to which you would like to allow or deny access. If you are creating an IAM permissions policy to attach to a user or role, you cannot include this element. The principal is implied as that user or role.
        
    4. Action – Include a list of actions that the policy allows or denies.
        
    5. Resource (Required in only some circumstances) – If you create an IAM permissions policy, you must specify a list of resources to which the actions apply. If you create a resource-based policy, this element is optional. If you do not include this element, then the resource to which the action applies is the resource to which the policy is attached.
        
    6. Condition (Optional) – Specify the circumstances under which the policy grants permission.


## USE CASE

Which of the following AWS services are always free to use (Select two)?

AWS Auto Scaling
AWS Identity and Access Management (AWS IAM)

## USE CASE

Which of the following AWS services is essential for implementing security of resources in AWS Cloud?

AWS Identity and Access Management (IAM)

## USE CASE

Which of the following are recommended best practices for AWS Identity and Access Management (AWS IAM) service? (Select two)

Enable multi-factor authentication (MFA) for all users
Rotate credentials regularly

## USE CASE 

AWS Identity and Access Management (AWS IAM) policies are written as JSON documents. Which of the following are mandatory elements of an IAM policy?

Effect, Action

Which of the following entities should be used for an Amazon Elastic Compute Cloud (Amazon EC2) Instance to access a DynamoDB table?

IAM role

## USE CASE

A corporation would like to simplify access management to multiple AWS accounts as well as facilitate AWS Single Sign-On (AWS SSO) access to its AWS accounts. As a Cloud Practitioner, which AWS service would you use for this task?

AWS IAM Identity Center

## USE CASE

A multinational company has just moved its infrastructure to AWS Cloud and has employees traveling to different offices around the world. How should the company set the AWS accounts?

There is nothing to do, AWS Identity and Access Management (AWS IAM) is a global service

## USE CASE

Which of the following AWS Identity and Access Management (AWS IAM) Security Tools allows you to review permissions granted to an IAM user?

AWS Identity and Access Management (IAM) access advisor

## USE CASE

Which of the following are the security best practices suggested by AWS for Identity and Access Management (IAM)? (Select two)

When you create IAM policies, grant the least privileges required to perform a task
Do not share security credentials between accounts, use IAM roles instead

## USE CASE

As a Cloud Practitioner, which of the following credentials would you recommend for signing in to the AWS Management Console to meet security best practices? (Select two)

IAM Username and password
Multi Factor Authentication (MFA)