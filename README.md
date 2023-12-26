# TechMagic Technical Task
## AWS infrastructure (CloudFormation) to deploy a basic web application. Utilize Amazon EFS to store the HTML page content and Amazon ECS for containerized deployment
My CloudFormation Nested Stack (main.yaml):
- VPC (vpc-stack.yaml)
- EFS (efs-stack.yaml)
- ECS Cluster + ALB (cluster-stack.yaml)
- ECS Service (service-stack.yaml)

In order to use this nested stack you need to:
1) Download all files with YAML extension. 
2) Next, you need to upload the files below to your S3 Bucket.
  - vpc-stack.yaml
  - efs-stack.yaml
  - cluster-stack.yaml
  - service-stack.yaml
3) Replace the links in the main.yaml file with the locations of the above files in your S3 Bucket.
4) Deploy the CloudFormation stack using either the AWS Management Console 
