2024-10-06 20:11

Status:

Tags:
[[AWS Budgeting Index]]

# AWS Cost and Usage Report

it a service that contains the most comprehensive set of cost and usage data available. You can use cost and usage reports to publish your AWS billing reports to Amazon Simple Storage Service (Amazon S3) bucket that you own.

You can receive reports that break down your costs by the hour, day, or month, by product or product resource, or by tags that you define yourself.

AWS updates the report in your bucket once a day in comma-separated value (CSV) format. You can view the reports using spreadsheet software such as Microsoft Excel or Apache OpenOffice Calc, or access them from an application using the Amazon S3 API.

AWS Cost and Usage Reports tracks your AWS usage and provides estimated charges associated with your account. Each report contains line items for each unique combination of AWS products, usage type, and operation that you use in your AWS account. 

You can customize the AWS Cost and Usage Reports to aggregate the information either by the hour, day or month.

AWS cost and usage reports can do the following:

- Deliver report files to your Amazon S3 bucket.
- Update the report up to three times a day.
- Create, Retrieve, and delete your reports using the AWS CUR API Reference.


References 
[What is AWS Cost and Usage Report](https://docs.aws.amazon.com/cur/latest/userguide/what-is-cur.html)