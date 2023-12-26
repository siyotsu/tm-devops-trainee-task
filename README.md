# TechMagic Technical Task
## AWS infrastructure (CloudFormation) to deploy a basic web application. Utilize Amazon EFS to store the HTML page content and Amazon ECS for containerized deployment
My CloudFormation Nested Stack:
- VPC (vpc-stack.yaml)
- EFS (efs-stack.yaml)
- ECS Cluster + ALB (cluster-stack.yaml)
- ECS Service (service-stack.yaml)
