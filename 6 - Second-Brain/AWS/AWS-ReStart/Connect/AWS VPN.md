2024-10-06 12:35

Status:

Tags:
[[AWS Connections Index]]

# AWS VPN

Amazon offers the following VPN connectivity options:

- AWS Site-to-Site VPN:

You can create an IPsec VPN connection between your VPC and your remote network. On the AWS side of the Site-to-Site VPN connection, a virtual private gateway or transit gateway provides two VPN endpoints (tunnels) for automatic fail-over.

You configure your customer gateway device on the remote side of the Site-to-Site VPN connection. more info on [AWS Site-to-Site VPN User Guide](https://docs.aws.amazon.com/vpn/latest/s2svpn/VPC_VPN.html)

- AWS Client VPN:

AWS Client VPN is a managed client-based VPN service that enables you to securely access your AWS resources or your on-premises network. with AWS Client VPN, you configure an endpoint to which your users can connect to establish a secure TLS VPN session. This enables clients to access resources in AWS or on-premises from any location using an OpenVPN-based VPN client. more info on [AWS Client VPN Administrator Guide](https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/)

- AWS VPN CloudHub:

If you have more than one remote network (For example, multiple branch offices), you can create multiple AWS Site-to-Site VPN connections via your virtual private gateway to enable communication between these networks. for more info check [Providing secure communication between sites using VPN CloudHub](https://docs.aws.amazon.com/vpn/latest/s2svpn/VPN_CloudHub.html)

- third party software VPN appliance:

You can create a VPN connection to your remote network by using an Amazon EC2 instance in your VPC that's running a third party software VPN appliance. AWS does not provide or maintain third party software VPN appliances.

However, you can choose from a range of products provided by partners and open source communities. you can also find third party software VPN appliances on the [AWS Marketplace](https://aws.amazon.com/marketplace/search/results/ref=brs_navgno_search_box?searchTerms=vpn)

References 
[AWS_VPN](https://docs.aws.amazon.com/vpc/latest/userguide/vpn-connections.html)