2024-10-06 16:07

Status:

Tags:
[[AWS Orchestration & Management Index]]
#management

# AWS Session Manager

Is a fully managed AWS System Manager capability.

With Session Manager, you can manage your Amazon Elastic Compute Cloud )Amazon EC2) instances, edge devices, on-premises servers, and virtual machines (VMs). You can use either an interactive on-click browser-based shell or the AWS Command Line Interface (AWS CLI).

Session Manager provides secure and audit-able node management without the need to open inbound ports, maintain bastion hosts, or manage SSH keys.

Session Manager also allows you to comply with corporate policies that require controlled access to managed nodes, strict security practices, and fully audit-able logs with node access details, while providing end users with simple one-click cross-platform access to your managed nodes.

To get started with Session Manager, open the [Systems Manager Console](https://console.aws.amazon.com/systems-manager/session-manager)


Benefits of using Session Manager to your organization:

- **Centralized access control to managed nodes using IAM policies**

	Administrators have a single place to grant and revoke access to managed nodes. Using only AWS Identity and Access Management (IAM) policies, you can control which individual users or groups in your organization can use Session Manager and which managed nodes they can access.

- **No open inbound ports and no need to manage bastion hosts or SSH keys**

	Leaving inbound SSH ports and remote PowerShell ports open on your managed nodes greatly increases the risk of entities running unauthorized or malicious commands on the managed nodes. Session Manager helps you improve your security posture by letting you close these inbound ports, freeing you from managing SSH keys and certificates, bastion hosts, and jump boxes.

- **One-click access to managed nodes from the console and CLI**

	Using the AWS Systems Manager console or Amazon EC2 console, you can start a session with a single click, Using the AWS CLI, you can also start a session that runs a single command or a sequence of commands.
	
	Because permissions to managed nodes are provided through IAM policies instead of SSH keys or other mechanisms, the connection time is greatly reduced.

- **Connect to both Amazon EC2 instances and non-EC2 managed nodes in [hybrid and multicloud](https://docs.aws.amazon.com/systems-manager/latest/userguide/operating-systems-and-machine-types.html#supported-machine-types) environments**
    
    You can connect to both Amazon Elastic Compute Cloud (Amazon EC2) instances and non-EC2 nodes in your [hybrid and multicloud](https://docs.aws.amazon.com/systems-manager/latest/userguide/operating-systems-and-machine-types.html#supported-machine-types) environment.
    
    To connect to non-EC2 nodes using Session Manager, you must first activate the advanced-instances tier. **There is a charge to use the advanced-instances tier.** However, there is no additional charge to connect to EC2 instances using Session Manager. For information, see [Configuring instance tiers](https://docs.aws.amazon.com/systems-manager/latest/userguide/fleet-manager-configure-instance-tiers.html).
    
- **Port forwarding**
    
    Redirect any port inside your managed node to a local port on a client. After that, connect to the local port and access the server application that is running inside the node.
    
- **Cross-platform support for Windows, Linux, and macOS**
    
    Session Manager provides support for Windows, Linux, and macOS from a single tool. For example, you don't need to use an SSH client for Linux and macOS managed nodes or an RDP connection for Windows Server managed nodes.
    
- **Logging and auditing session activity**
    
    To meet operational or security requirements in your organization, you might need to provide a record of the connections made to your managed nodes and the commands that were run on them. You can also receive notifications when a user in your organization starts or ends session activity.
    
    Logging and auditing capabilities are provided through integration with the following AWS services:
    
    - **AWS CloudTrail** – AWS CloudTrail captures information about Session Manager API calls made in your AWS account and writes it to log files that are stored in an Amazon Simple Storage Service (Amazon S3) bucket you specify. One bucket is used for all CloudTrail logs for your account. For more information, see [Logging AWS Systems Manager API calls with AWS CloudTrail](https://docs.aws.amazon.com/systems-manager/latest/userguide/monitoring-cloudtrail-logs.html).
        
    - **Amazon Simple Storage Service** – You can choose to store session log data in an Amazon S3 bucket of your choice for debugging and troubleshooting purposes. Log data can be sent to your Amazon S3 bucket with or without encryption using your AWS KMS key. For more information, see [Logging session data using Amazon S3 (console)](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-logging.html#session-manager-logging-s3).
        
    - **Amazon CloudWatch Logs** – CloudWatch Logs allows you to monitor, store, and access log files from various AWS services. You can send session log data to a CloudWatch Logs log group for debugging and troubleshooting purposes. Log data can be sent to your log group with or without AWS KMS encryption using your KMS key. For more information, see [Logging session data using Amazon CloudWatch Logs (console)](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-logging.html#session-manager-logging-cloudwatch-logs).
        
    - **Amazon EventBridge** and **Amazon Simple Notification Service** – EventBridge allows you to set up rules to detect when changes happen to AWS resources that you specify. You can create a rule to detect when a user in your organization starts or stops a session, and then receive a notification through Amazon SNS (for example, a text or email message) about the event. You can also configure a CloudWatch event to initiate other responses. For more information, see [Monitoring session activity using Amazon EventBridge (console)](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-auditing.html#session-manager-auditing-eventbridge-events).

References 
[What is AWS Session Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager.html)