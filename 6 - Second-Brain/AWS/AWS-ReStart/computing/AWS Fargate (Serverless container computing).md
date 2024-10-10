2024-09-27 19:33

Status:

Tags:
[[AWS Computing Index]]

# AWS Fargate (Serverless container computing)

Its a technology that you can use with Amazon ECS to run containers, without having to manage servers or clusters of Amazon EC2 instances. With AWS Fargate, you no longer have to provision, configure, or scale clusters of virtual machines to run containers.

This removes the need to choose server types, decide when to scale your clusters, or optimize cluster packing.

When you run your tasks and services with the Fargate launch type, you package your application in containers, specify the CPU and memory requirements, define networking and IAM policies, and launch the application.

Each Fargate task has its own isolation boundary and does not shara the underlying kernel, CPU resources, memory resources, or elastic network interface with another task.

you configure your task definitions for fargate by setting the `requiresCompatibilities` task definition parameter to `FARGATE`. for more information, see [launch types](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#requires_compatibilities).


References 
[What is AWS Fargate](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html)