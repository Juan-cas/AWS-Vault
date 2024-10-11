2024-09-27 19:40

Status:

Tags:
[[AWS Computing Index]]

# Amazon Elastic Kubernetes Service (EKS) (Kubernetes containers)


Is a managed service that eliminates the need to install, operate, and maintain your own Kubernetes control panel on Amazon Web Services (AWS). 

[Kubernetes](https://kubernetes.io/docs/concepts/overview/) is an open-source system that automates the management, scaling, and deployment of containerized applications.


Key features of Amazon EKS:

- Secure networking and authentication
	Amazon EKS integrates your Kubernetes workloads with AWS networking and security services. It also integrates with AWS Identity and Access Management (IAM) to provide [authentication](https://docs.aws.amazon.com/eks/latest/userguide/cluster-auth.html) for your Kubernetes clusters.

 - Easy cluster scaling
	Amazon EKS enables you to scale your Kubernetes clusters up and down easily based on the demand of your workloads. Amazon EKS supports [horizontal Pod autoscaling](https://docs.aws.amazon.com/eks/latest/userguide/horizontal-pod-autoscaler.html) based on CPU or custom metrics, and [cluster autoscaling](https://docs.aws.amazon.com/eks/latest/userguide/autoscaling.html) based on the demand of the entire workload.

- Managed Kubernetes experience
	You can make changes to your Kubernetes clusters using [`eksctl`](https://eksctl.io/), [AWS Management Console](https://console.aws.amazon.com/eks/), [AWS Command Line Interface (AWS CLI)](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/eks/index.html), [the API](https://docs.aws.amazon.com/eks/latest/APIReference/Welcome.html), [kubectl](https://docs.aws.amazon.com/eks/latest/userguide/install-kubectl.html), and [Terraform](https://tf-eks-workshop.workshop.aws/).

- High Availability
	Amazon EKS provides [high availability](https://docs.aws.amazon.com/eks/latest/userguide/disaster-recovery-resiliency.html) for your control plane across multiple Availability Zones.

- Integration with AWS services
	Amazon EKS integrates with other [AWS services](https://docs.aws.amazon.com/eks/latest/userguide/eks-integrations.html), providing a comprehensive platform for deploying and managing your containerized applications. You can also more easily troubleshoot your Kubernetes workloads with various [observability](https://docs.aws.amazon.com/eks/latest/userguide/eks-observe.html) tools.


![[AWS EKS.png]]

References 
[What is Amazon EKS] (https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)