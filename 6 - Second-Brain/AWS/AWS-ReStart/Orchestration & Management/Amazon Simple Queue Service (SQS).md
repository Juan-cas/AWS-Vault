2024-10-06 16:06

Status:

Tags:
[[4 - Indexes/AWS 1/AWS Orchestration & Management Index]]

# Amazon Simple Queue Service (SQS)

offers a secure, durable and available hosted queue that lets you integrate and decouple distributed software systems and components.

Amazon SQS offers a common constructs such as [Dead-letter queues](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-dead-letter-queues.html) and [cost allocation tags](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-queue-tags.html). It provides a generic web services API that you can access using any programming language that the AWS SDK supports.

Benefits of using Amazon SQS:

- Security:

You control who can send messages to and receive messages from an Amazon SQS queue, you can choose to transmit sensitive data by protecting the contents of messages in queues by using default Amazon SQS managed server-side encryption (SSE), or by using custom SSE keys managed in AWS Key Management Service (AWS KMS).

- Durability:

For the safety of your messages, Amazon SQS stores them on multiple servers, standard queues support [at-least-once message delivery](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/standard-queues-at-least-once-delivery.html), and FIFO queues support [exactly-once message processing](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/FIFO-queues-exactly-once-processing.html) and [high-throughput](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/high-throughput-fifo.html) mode.

- Availability:

Amazon SQS uses [redundant infrastructure](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html#sqs-basic-architecture) to provide highly-concurrent access to messages and high availability for producing and consuming messages.

- Scalability:

Amazon SQS can process each [buffered request](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-client-side-buffering-request-batching.html) independently, scaling transparently to handle any load increases or spikes without any provisioning instructions.

- Reliability:

Amazon SQS locks your messages during processing, so that multiple producers can send and multiple consumers can receive messages at the same time.

- Customization:

Your queues don't have to be exactly alike -for example, you can [set a default delay on a queue](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-delay-queues.html). You can store the contents of messages larger than 256KB using [Amazon Simple Storage Service (S3)](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-s3-messages.html) or Amazon DynamoDB, with Amazon SQS holding a pointer to the Amazon S3 object, or you can split a larger message into smaller messages.

An example scenario would be:

	Your system has several producers (Components that send messages to the queue) and consumers (components that receive messages from the queue). The queue (which holds messages A through E) redundantly stores the messages across multiple Amazon SQS servers to ensure reliability.


![[Amazon SQS case..png]]

References 
[AWS SQS](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html)