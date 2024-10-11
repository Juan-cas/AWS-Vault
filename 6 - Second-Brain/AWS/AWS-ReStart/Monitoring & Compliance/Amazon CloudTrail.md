2024-10-06 17:42

Status:

Tags:
[[AWS Monitoring & Compliance Index]]
#monitoring

is an AWS service that helps you enable operational and risk auditing, governance, and compliance of your AWS account.

Actions taken by a user, role or an AWS service are recorded as events in CloudTrail. Events include actions taken in the AWS Management Console, AWS Command Line Interface, and AWS SDKs and APIs.

CloudTrail provides three ways to record events:

- **Event history**

	The event history provides a viewable, searchable, downloadable, and immutable record of the past 90 days of management events in an AWS Region.

- **CloudTrail Lake**

	Is a managed data lake for capturing, storing, accessing, and analyzing user and API activity on AWS for audit and security purposes. CloudTrail Lake converts existing events in row-based JSON format to Apache ORC format.

	you can keep the data for up to 10 years.

- **Trails**

	Trails capture record of AWS activities, delivering and storing these events in an Amazon S3 bucket, with optional delivery to CloudWatch Logs and Amazon EventBridge.

	You can input these events into your security monitoring solutions. You can also use your own third-party solutions or solutions such as AWS Athena to search and analyze your CloudTrail logs.

References 
[What is amazon Cloudtrail](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html)