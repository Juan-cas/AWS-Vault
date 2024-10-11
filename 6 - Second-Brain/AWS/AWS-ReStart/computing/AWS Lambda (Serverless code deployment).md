2024-09-27 19:56

Status:

Tags:
[[AWS Computing Index]]
#computing 


# AWS Lambda (Serverless code deployment)

It can be used to run code without provisioning or managing servers.

Lambda runs your code on a high-availability compute infrastructure and performs all of the administration of the compute resources, including server and operating system maintenance, capacity provisioning and automatic scaling, and logging. With lambda, all you need to do is supply your code in one of the language run-times that lambda supports.

You organize your code into lambda functions. The Lambda service runs your function only when needed and scales automatically. You only pay for the compute time that you consume- there is no charge when your code is not running.

## When to use Lambda ?

- File processing:
	Use Amazon S3 to trigger lambda data processing in real time after an upload.

- Stream processing:
	Use Lambda and Kinesis to process real-time streaming data for application activity tracking, transaction order processing, click-stream analysis, data cleansing, log filtering, indexing, social media analysis, internet of Things (IoT) device data telemetry, and metering.

- Web Applications:
	Combine lambda with other AWS services to build powerful web applications that automatically scale up and down and run in a highly available configuration across multiple data centers.

- IoT backends: 
	Build serverless backends using Lambda to handle web, mobile, IoT, and third-party API requests.

- Mobile Backends:
	Build backends using Lambda and amazon API gateway to authenticate and process API requests. use AWS Amplify to easily integrate with your IOS, Android, Web and React Native Front-ends.

##### *When using lambda you are responsible only for your code.*
Lambda managed the compute fleet that offers a balance of memory, CPU, network, and other resources to run your code. Because lambda manages these resources you cannot log in to compute instances or customize the operating system on provided runtimes. Lambda performs operational and administrative activities on your behalf, including managing capacity, monitoring and logging your lambda functions.


for further information please enter the reference...

References 
[What is AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)