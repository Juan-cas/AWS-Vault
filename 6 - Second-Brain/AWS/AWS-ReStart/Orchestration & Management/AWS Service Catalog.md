2024-10-06 16:07

Status:

Tags:
[[4 - Indexes/AWS 1/AWS Orchestration & Management Index]]

# AWS Service Catalog

This service enables organizations to create and manage catalogs of IT services that are approved for AWS. There It services can include everything from virtual machine images, servers, software, databases and more to complete multi-tier application architectures.

It also allows organizations to centrally manage commonly deployed IT services, and helps organizations achieve consistent governance and meet compliance requirements.

This includes the ability to deploy infrastructure as code (IaC) using AWS CloudFormation templates, helping in the governance and management of resources efficiently.

End users can quickly deploy only the approved IT services they need, following the constraints set by your organization.


Service Catalog provides the following benefits:

- Standardization:

Administer and manage approved assets by restricting where the product can be launched, the type of instance that can be used, and many other configuration options. the result is a standardized landscape for product provisioning for your entire organization.

- Self-Service discovery and launch

Users browse listings of products (Services or Applications) that they have access to, locate the product that they want to use, and launch it all on their own as a provisioned product.

- Fine-Grain access control

Administrators assemble portfolios of products from their catalog, add constraints and resource tags to be used at provisioning, and then grant access to the portfolio through AWS Identity and Access Management (IAM) users and groups.

- Extensibility and version control

Administrators can add a product to any number of portfolios and restrict it without creating another copy. Updating the product to a new version propagates the update to all products in every portfolio that references it.


For more information please check the [Service Catalog Detail Page](http://aws.amazon.com/servicecatalog/details)

References 
[What is AWS Service Catalog](https://docs.aws.amazon.com/servicecatalog/latest/adminguide/introduction.html)