2024-10-06 15:50

Status:

Tags:
[[AWS Connections Index]]

# AWS VPC peering

VPC is a virtual network dedicated to your AWS account, it is logically isolated from other virtual networks in the AWS Cloud, you can launch AWS resources, such as Amazon EC2 instances, into your VPC.

Thus a VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them using private IPv4 addresses or IPv6 addresses.

Instances in either VPC can communicate with each other as if they are within the same network. You can create a VPC peering connection between your own VPCs, r with a VPC in another AWS account. The VPCs can be in different Regions (Also known as an inter-region VPC peering connection)

related image:

![[VPC peering.png]]

References 
[VPC_Peering](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html)