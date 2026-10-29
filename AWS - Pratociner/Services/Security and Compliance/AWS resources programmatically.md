## Overview

**Use Access Key ID and Secret Access Key to access AWS resources programmatically**

Access keys are long-term credentials for an IAM user or the AWS account root user. You can use access keys to sign programmatic requests to the AWS CLI or AWS API (directly or using the AWS SDK). Access keys consist of two parts: an access key ID and a secret access key. As a user name and password, you must use both the access key ID and secret access key together to authenticate your requests. When you create an access key pair, save the access key ID and secret access key in a secure location. The secret access key is available only at the time you create it.

## Use Cases

### 1. AWS CLI (Command Line Interface)
Use Access Key ID and Secret Access Key to configure AWS CLI for command-line access to AWS services.

**Example:**
```bash
aws configure
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
Default region name [None]: us-east-1
Default output format [None]: json
```

Once configured, you can execute AWS commands:
```bash
aws s3 ls
aws ec2 describe-instances
aws dynamodb list-tables
```

### 2. AWS SDKs (Software Development Kits)
Use Access Key ID and Secret Access Key in your application code to interact with AWS services programmatically.

**Example (Python - Boto3):**
```python
import boto3

# Configure credentials
s3_client = boto3.client(
    's3',
    aws_access_key_id='AKIAIOSFODNN7EXAMPLE',
    aws_secret_access_key='wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY',
    region_name='us-east-1'
)

# Upload file to S3
s3_client.upload_file('local_file.txt', 'my-bucket', 'remote_file.txt')
```

**Example (Node.js - AWS SDK):**
```javascript
const AWS = require('aws-sdk');

// Configure credentials
AWS.config.update({
    accessKeyId: 'AKIAIOSFODNN7EXAMPLE',
    secretAccessKey: 'wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY',
    region: 'us-east-1'
});

// Create DynamoDB client
const dynamodb = new AWS.DynamoDB();
dynamodb.listTables({}, (err, data) => {
    if (err) console.log(err);
    else console.log(data);
});
```

### 3. Direct API Calls
Use Access Key ID and Secret Access Key to make direct HTTPS requests to AWS service endpoints with proper authentication signatures.

**Example (REST API call to S3):**
```bash
curl -X GET https://my-bucket.s3.amazonaws.com/my-object.txt \
  -H "Authorization: AWS4-HMAC-SHA256 Credential=AKIAIOSFODNN7EXAMPLE/20231226/us-east-1/s3/aws4_request..." \
  -H "x-amz-date: 20231226T120000Z"
```

**Use case:** Integrating AWS services into custom applications where SDK is not available or when you need fine-grained control over API requests.

## Best Practices

- ✅ Never hardcode credentials in source code
- ✅ Use IAM roles for EC2 instances instead of access keys when possible
- ✅ Rotate access keys regularly
- ✅ Use environment variables or AWS credentials file to store keys
- ✅ Apply least privilege principle to IAM users with access keys
- ✅ Enable MFA for sensitive operations
- ❌ Never commit access keys to version control (GitHub, GitLab, etc.)
- ❌ Never share access keys via email or messaging platforms
