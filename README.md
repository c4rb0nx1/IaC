# IaC
Let's Learn IaC
### Serverless Deployment Bucket ![click here](https://github.com/c4rb0nx1/IaC/blob/side/cloudformation-template-S3-Bucket.json).
This CloudFormation template deploys an S3 bucket for storing code artifacts and assets for serverless deployments.

### The template contains the following resources:
- ServerlessDeploymentBucket - An S3 bucket used for storing deployment files for serverless applications. The bucket is encrypted with default AES-256 encryption.
- ServerlessDeploymentBucketPolicy - An S3 bucket policy that denies public access to the bucket and enforces HTTPS only connections.

### Usage
To use this template:
- Upload the template to an S3 bucket in your account
- Launch the template using CloudFormation and specify the stack details
- The S3 bucket will be created in the region you deploy the stack to
- Pass the bucket name output to your CI/CD pipeline for serverless deployments
The bucket can be used to store ZIP files of your Lambda code, npm packages, static assets, CloudFormation templates, and other artifacts needed to deploy your serverless application.
