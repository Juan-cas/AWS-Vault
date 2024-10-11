2024-10-10 20:30
# AWS Shared Responsibility Model

Security and compliance are shared responsibilities between AWS and the customer.

Depending on the services deployed this shared model can help relieve the customer's operational burden, this is because AWS operates, manages and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates. the customer assumes responsibility and management of the guest operating system (including updates and security patches) and other associated application software, in addition to the configuration of the AWS-provided security group firewall.

AWS recommends that customers carefully consider the services they choose because their responsibilities vary depending on the services used, the integration of those services into their IT environment, and applicable laws and regulations. It is possible for customers to enhance their security and/or meet their more stringent compliance requirements by leveraging technology such as host-based firewalls, host-based intrusion detection and prevention, encryption, and key management.

The nature of this shared responsibility also provides the flexibility and customer control that permits customers to deploy solutions that  meet the industry-specific certification requirements. 

![[AWS-Shared-Responsibility-Chart.png]]

This shared responsibility model also extends to IT controls. Just as the responsibility to operate the IT environment is shared between AWS and its customers, the management, operation, and verification of IT controls is also a shared responsibility.

AWS can help customers by managing those controls associated with the physical infrastructure deployed in the AWS environment. Customers can then use the AWS control and compliance documentation available to them to perform their control evaluation and verification procedures as required. For example how responsibility for certain controls is shared between AWS and its customers.

References 
[AWS Shared-Responsibility-Model](https://docs.aws.amazon.com/whitepapers/latest/aws-risk-and-compliance/shared-responsibility-model.html)