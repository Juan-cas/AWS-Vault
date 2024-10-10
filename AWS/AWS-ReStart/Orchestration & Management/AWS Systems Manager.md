2024-10-06 16:07

Status:

Tags:
[[AWS Orchestration & Management Index]]

# AWS Systems Manager

Is the operations hub for your AWS applications and resources and a secure end-to-end management solution for [hybrid and multicloud](https://docs.aws.amazon.com/systems-manager/latest/userguide/operating-systems-and-machine-types.html#supported-machine-types) environments that enables secure operations at scale.


## How System Manager works

The following diagram describes how some Systems Manager capabilities perform actions on your resources. The diagram doesn't cover all capabilities. Each enumerated interactions is described before the diagram.

![[AWS System Management diagram.png]]

- **Access Systems Manager**

	Use one of the available options for [accessing Systems Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html#access-methods)

- **Choose a System manager capability**

	Determine which capability can help you perform the action you want to perform on your resources. The diagram shows only a few of the capabilities that IT administrators and DevOps personnel can use to manage their applications and resources.

- **Verification and processing**

	System Manager verifies that your user, group or role has the required AWS identity and access management (IAM) permissions to perform the action you specified.

	If the target of your action is a managed node, the Systems Managed Agent (SSM Agent) running on the node performs the action. For other types of resources, Systems Manager performs the specified action or communicates with other AWS services to perform the action on behalf of the System Manager.

- **Reporting**

	Systems Manager, SSM Agent, and other AWS services that performed an action on behalf of the Systems Manager report status. System Manager can send status details to other AWS services, if configured.

- **Systems Manager Operations Management Capabilities**

	If enabled, Systems Manager operations management capabilities such as Explorer, OpsCenter, and Incident Manager aggregate operations data or create artifacts in response to events or errors with your resources. 

	These artifacts include operational work items (OpsItems) and incidents. Systems Manager operations management capabilities provide operational insight into your applications and resources and automated remediation solutions to help troubleshoot problems.

References 
[What is AWS System Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html)