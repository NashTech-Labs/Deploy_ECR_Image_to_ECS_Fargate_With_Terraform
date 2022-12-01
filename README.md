# DESCRIPTION

This template is the second part of :- https://github.com/knoldus/Build-Image-On-ECR-Using-Jenkins

Here in this template, you will learn about the concept of ECS Fargate using Terraform.
In `terraform-ecs-fargate` folder there is the scripts to create network,security and logs. 

---

### Steps 

1. Open the `terraform-ecs-fargate` folder in your terminal.
2. Run the following commands:

`terraform init`

`terraform plan`

`terraform apply -auto-approve`

3.After running these commands it will create your  ECS , Fargate and ALB and you can access the application using the DNS in ALB as shown in `outputs.tf` file.

4.In `templates > ecs > myapp.json.tpl` file all the configuration is written for Fargate.

---

### Tech Stack
* Terraform
* AWS ECR
* AWS ECS Fargate
* Docker
* Jenkins

---

#### Notes

Please follow these links for any help:-

Previous template:-
https://github.com/knoldus/Build-Image-On-ECR-Using-Jenkins

Video:-
https://www.youtube.com/watch?v=h1g1hA_aMFQ&t=1328s

---
# springboot-docker-ecs
Run your Docker image on AWS ECS (Elastic Container Service)

### Application Flow  

<img width="576" alt="11" src="https://user-images.githubusercontent.com/25712816/91267149-570d0780-e790-11ea-8497-806b30cbcfc2.PNG">

---
#### AWS Fargate

AWS Fargate is a technology that provides on-demand, right-sized compute capacity for containers. With AWS Fargate, you don't have to provision, configure, or scale groups of virtual machines on your own to run containers. You also don't need to choose server types, decide when to scale your node groups, or optimize cluster packing. You can control which pods start on Fargate and how they run with Fargate profiles. Fargate profiles are defined as part of your Amazon EKS cluster.

#### AWS ECS

Amazon Elastic Container Service (Amazon ECS) is a highly scalable and fast container management service. You can use it to run, stop, and manage containers on a cluster. With Amazon ECS, your containers are defined in a task definition that you use to run an individual task or task within a service. In this context, a service is a configuration that you can use to run and maintain a specified number of tasks simultaneously in a cluster. You can run your tasks and services on a serverless infrastructure that's managed by AWS Fargate. Alternatively, for more control over your infrastructure, you can run your tasks and services on a cluster of Amazon EC2 instances that you manage.

---