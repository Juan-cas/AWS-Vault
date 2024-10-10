2024-10-06 12:34

Status:

Tags:
[[4 - Indexes/AWS 1/AWS Connections Index]]

# AWS Transit Gateway

Provides a hub and spoke design for connection VPCs and on-premises networks as a fully managed service without requiring you to provision third-party virtual appliances, no VPN overlay is required, and AWS manages high availability and scalability.

This further enables customers to connect thousands of VPCs.

You can attach all your hybrid connectivity (VPN and Direct Connect connections) to a single gateway, consolidating and controlling your organization's entire AWS routing configuration in one place (refer to the following picture).

![[AWS_Transit_Gateway.png]]

Transit Gateway controls how traffic is routed among all the connected spoke networks using route tables.

This hub-and-spoke model simplifies management and reduces operational costs because VPCs only connect to the Transit Gateway instance to gain access to the connected networks.

References 
[transit gateway](https://docs.aws.amazon.com/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/transit-gateway.html)