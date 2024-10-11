2024-10-02 20:22

Status:

Tags:
[[Data Transfer Index]]
#transfer
# AWS Server Migration Service

Automates the migration of on-premises VMware vSphere or Microsoft Hyper-V/SCVMM virtual machines to the AWS cloud.

AWS SMS incrementally replicates server VMs as cloud-hosted Amazon machine Images (AMI's) ready for deployment on Amazon EC2.

Servers running on-premises and being migrated to the cloud with (AWS SMS) can contain PHI data. AWS SMS encrypts data while in transit and when server VM images are being staged for final placement onto EC2.

Refer to the guidance for EC2 and setting up encrypted storage volumes when migrating a server VM containing PHI with AWS SMS. AWS SMS uses CloudTrail to log all API calls.

References 
[What is AWS Server Migration Service](https://docs.aws.amazon.com/es_es/whitepapers/latest/architecting-hipaa-security-and-compliance-on-aws/aws-server-migration-service.html)