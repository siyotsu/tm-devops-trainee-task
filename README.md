# TechMagic Technical Task
## AWS infrastructure (CloudFormation) to deploy a basic web application. Utilize Amazon EFS to store the HTML page content and Amazon ECS for containerized deployment
My CloudFormation Nested Stack (main.yaml):
- VPC (vpc-stack.yaml)
- EFS (efs-stack.yaml)
- ECS Cluster + ALB (cluster-stack.yaml)
- ECS Service (service-stack.yaml)

In order to use this nested stack you need to:
- Download all files with YAML extension. 
- Next, you need to upload the files below to your S3 Bucket.
  - vpc-stack.yaml
  - efs-stack.yaml
  - cluster-stack.yaml
  - service-stack.yaml

![image](https://github.com/siyotsu/tm-devops-trainee-task/assets/109180406/fe132bb0-2afd-4383-8be7-9569039540c6)


- Replace the links in the main.yaml file with the locations of the above files in your S3 Bucket.
- Deploy the CloudFormation stack using either the AWS Management Console:
  Go to AWS CloudFormation -> Create Stack
  
  ![image](https://github.com/siyotsu/tm-devops-trainee-task/assets/109180406/9cfd08ec-4bc7-4e24-9ecb-9558f750874f)
  
- Upload the updated template file named main.yaml -> Next

- Specify stack details (Provide a stack name and parameters) -> Next

- Configure stack options -> Next

- Review your stack -> Submit

- Your stack will start to deploy step-by-step.
  
  ![image](https://github.com/siyotsu/tm-devops-trainee-task/assets/109180406/1f9d1d35-168f-4a24-9446-7586376b1c4f)

Problems I encountered during the task:
1) How to properly use parameters in the nested stack.
2) How to upload HTML page to the EFS file system through EC2 instance.

