# Servian Techchallenge

## Proposed Soutions
The applications can be deployed over kubernets or virtual machines with auto scale features for high availability. This code helps to deploy the servian tech app over AWS EC2 instances with high available features.

## Used AWS Services
* VPC
* EC2 
* ALB
* Auto Scale
* RDS

## Infra Architecture

The VPC has public and private subnets which used for placing EC2 instance and Postgres RDS. The EC2 instance deploy using auto scale feature. Both RDS and EC2 instances will be available on two AZs. The application is running behind an application load balancer which checks the application helath frequently and ensure the application health.

![architecture](img/architecture.png)

## Deploy Application
The application can be deployed in default port as per the code. Its also can be exposed to other port that can be accessed through the application load balancer.
