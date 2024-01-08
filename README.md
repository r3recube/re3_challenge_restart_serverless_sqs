# AWS Serverless Exercise - Lambda, SQS and DynamoDB
This exercise involves setting up an AWS serverless environment where a Lambda function is triggered based on SQS queue messages. It includes creating an SQS queue, writing Python scripts for a message producer (running on your desktop) and a Lambda function (acting as a consumer), and configuring the Lambda function to process messages and save data to a DynamoDB table. 

## Requirements
This task tests AWS serverless service integration, Python scripting

- Candidates must successfully complete the mandatory tasks to progress in the hiring process, demonstrating fundamental AWS and Python skills essential for the role. 
- Optional tasks are there for earning additional points, showing a deeper understanding and broader skill set. 
- The bonus task is specifically for those who want to showcase advanced knowledge in infrastructure automation and DevOps practices, going above the basic requirements.

### Mandatory requirements
Essential tasks that test the core competencies required for the position. These include setting up the AWS Serverless infrastructure, writing the basic producer and consumer scripts using python. These tasks assess the candidate's fundamental skills in AWS services, Python scripting, and understanding of Serverless architecture.

1) Create a standard Amazon SQS queue
2) Define the SQS Access Policy and Configure IAM permission for SQS send/receive operations.
3) Develop a Python producer script to send JSON messages to SQS [example](#examples-of-json-messages)
4) Set up a DynamoDB table that can store the content of processed messages
5) Create an AWS Lambda function to process messages from SQS and save data to the DynamoDB table.
4) Include error handling and logging in the Lambda function.

#### Examples of JSON Messages
```
{
    "vehicleId": "VH2001",
    "make": "Honda",
    "model": "Civic",
    "year": 2020,
    "color": "Blue",
    "mileage": 15000
}
```

### Optional requirements
Advanced tasks that offer the opportunity to demonstrate additional skills. These include configuring CloudWatch for monitoring and logging, creating a CloudWatch dashboard for better visibility of the infrastructure, and using infrastructure as code tools like CloudFormation or Terraform. These tasks are more complex and test the candidate's proficiency in monitoring, optimization, and modern cloud deployment practices.

1) Use CloudWatch to monitor Lambda executions and SQS message processing.
2) Create a CloudWatch dashboard to monitor SQS and Lambda function metrics.
3) Implement dead-letter queues for handling processing failures.

### Bonus requirements
This bonus requirement is aimed at candidates who are comfortable with DevOps practices and more advanced AWS functionalities.

1) Use a Serverless [Framework](https://aws.amazon.com/it/serverless/getting-started/?serverless.sort-by=item.additionalFields.createdDate&serverless.sort-order=desc#Developer_tools) for infrastructure creation.
2) Implement AWS X-Ray for tracing and analyzing the behavior of the Lambda, SQS and DynamoDB.
3) Share CloudWatch dashboards and any advanced analytics.

## Test Scale-Out/In Process
- Use the Producer script to load messages into the SQS queue.
- Monitor the Lambda function for execution and processing of SQS messages.
- Validate that messages are correctly processed and stored in the DynamoDB table.
- Observe CloudWatch for monitoring the function execution and SQS queue metrics.

## Deliverables
Candidates are required to submit the URL of a Git repository containing all the project components (you can clone this repository).
The repository should include:
- README.md file with detailed documentation of the setup process, configurations, and test results.
- Source code for the Producer and Consumer Python scripts.
- Scripts, command-line instructions or Screenshoot used for setting up the SQS queue, Lambda Function and DynamoDB.
- Any additional configuration files or scripts used in the project.
- A report file containing the test process and observations, including screenshots, logs, and metrics.

Candidates should ensure that their Git repository is well-organized and includes comprehensive documentation to demonstrate their work effectively. This approach allows for an efficient review process and provides a clear understanding of the candidate's technical abilities and approach to problem-solving.