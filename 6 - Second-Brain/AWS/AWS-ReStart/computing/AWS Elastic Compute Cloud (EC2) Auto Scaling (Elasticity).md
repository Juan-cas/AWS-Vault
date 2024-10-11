2024-09-27 19:29

Status:

Tags:
[[AWS Computing Index]]
#computing 

# AWS Elastic Compute Cloud (EC2) Auto Scaling (Elasticity)

Its a service that helps you ensure that you have the correct number of Amazon EC2 instance available to handle the load for your application. You create collections of Ec2 instances, called *auto Scaling groups.* you can specify the minimum number of instances in each Auto Scaling Group and Amazon EC2 (AS) ensures that you group never goes below this size or set the maximum and it will never go above that size.

You can also specify desired capacity either when you create the group or at any time thereafter, Amazon EC2 (AS) ensures that your group has this many instances. If you specify scaling policies, then Amazon EC2 Auto Scaling can launch or terminate instances as demand on your application increases or decreases.

## For example

the following Auto Scaling group has a minimum size of four instances, a desired capacity of six instances, and a maximum size of twelve instances. The scaling policies that you define adjust the number of instances, within your minimum and maximum number of instances, based on the criteria that you specify.

![[EC2 AutoScaling example.png]]


References 
[what is EC2 autoscaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html)