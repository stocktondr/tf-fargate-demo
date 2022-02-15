# Terrafrom web app demo

### Utilizes

- AWS Application load Balancer
- EC2 Fargate
- Dockerhub as Image Registry

### Directions

- in root dir perform:
  - terraform init
  - terraform plan
  - terraform apply , yes
- The alb will take a couple of minutes to create
- when the alb creation has completed and the output is displayed,
  the app will still be warming up upon visiting the url... please wait at
  least 15 seconds.
