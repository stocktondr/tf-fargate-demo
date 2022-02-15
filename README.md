# Terraform Fargate Web App Demo

- Deploys an ECS Fargate container behind an Application Load Balancer
- The application is a simple todo list web app

### Primary Resources

- AWS Application load Balancer
- EC2 Fargate
- Dockerhub - Container Image Registry

### Requirements:

- terraform CLI
- AWS Default VPC
- AWS programmatic access
  - Use bash/zsh terminal command "aws configure" to set up access keys
  - terraform CLI will look for these when planning/applying from your local env

### Directions

- clone the repo code :
  - https:
    - git clone https://github.com/stocktondr/tf-fargate-demo.git
- in root dir perform:
  - terraform init
  - terraform plan
  - terraform apply , yes
- The alb will take a couple of minutes to reach completion
- An output will be displayed in the terminal window alb_dns = "`some URL`"
- Copy the URL from between the quotes ("`fargate-lb-tf......`")
- the health checks will still be warming up upon visiting the url... please wait at least 10 seconds following ALB completion step.
