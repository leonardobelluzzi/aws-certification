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