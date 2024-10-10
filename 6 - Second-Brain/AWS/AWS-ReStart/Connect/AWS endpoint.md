2024-10-06 15:50

Status:

Tags:
[[4 - Indexes/AWS 1/AWS Connections Index]]

# AWS endpoint

To connect programmatically to an AWS service, you use an endpoint. An endpoint is the URL of the entry point for an AWS web service.

The AWS SDKs and the AWS CLI (Command Line Interface) automatically use the default endpoint for each service in an AWS Region. But you can specify an alternate endpoint for your API requests.

If a service supports Regions, the resources in each Region are independent of similar resources in other Regions.
For example, you can create an Amazon EC2 instance or an Amazon SQS queue in one Region, When you do, the instance or queue is independent of instances or queue in all other regions.

References 
[AWS_End_Point](https://docs.aws.amazon.com/general/latest/gr/rande.html)