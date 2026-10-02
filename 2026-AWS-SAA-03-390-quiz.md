# AWS Certified Solutions Architect - Associate (SAA)

> Bộ 390 câu hỏi luyện thi chứng chỉ AWS Certified Solutions Architect – Associate (SAA).
> Đây là chứng chỉ dành cho người thiết kế các kiến trúc AWS an toàn, có khả năng mở rộng, hiệu năng cao và tối ưu chi phí.
> Chọn đáp án trong từng câu và mở **Kiểm tra đáp án** để xem đáp án đúng. 

## Hướng dẫn

- Câu chỉ có một đáp án đúng dùng radio button.
- Câu có nhiều đáp án đúng dùng checkbox; chọn đủ các đáp án trước khi kiểm tra.

**Tổng số câu: 390**

## Câu 1

**Chủ đề:** Design Cost-Optimized Architectures

A retail company has developed a REST API which is deployed in an Auto Scaling group behind an Application Load Balancer. The REST API stores the user data in Amazon DynamoDB and any static content, such as images, are served via Amazon Simple Storage Service (Amazon S3). On analyzing the usage trends, it is found that 90% of the read requests are for commonly accessed data across all users.

As a Solutions Architect, which of the following would you suggest as the MOST efficient solution to improve the application performance?

**Lựa chọn:**

<label for="q1-a"><input type="radio" id="q1-a" name="q1" value="A"> <strong>A.</strong> Enable Amazon DynamoDB Accelerator (DAX) for Amazon DynamoDB and Amazon CloudFront for Amazon S3</label><br>
<label for="q1-b"><input type="radio" id="q1-b" name="q1" value="B"> <strong>B.</strong> Enable ElastiCache Redis for DynamoDB and Amazon CloudFront for Amazon S3</label><br>
<label for="q1-c"><input type="radio" id="q1-c" name="q1" value="C"> <strong>C.</strong> Enable Amazon DynamoDB Accelerator (DAX) for Amazon DynamoDB and ElastiCache Memcached for Amazon S3</label><br>
<label for="q1-d"><input type="radio" id="q1-d" name="q1" value="D"> <strong>D.</strong> Enable ElastiCache Redis for DynamoDB and ElastiCache Memcached for Amazon S3</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Enable Amazon DynamoDB Accelerator (DAX) for Amazon DynamoDB and Amazon CloudFront for Amazon S3

</details>

---

## Câu 2

**Chủ đề:** Design Resilient Architectures

An e-commerce company is looking for a solution with high availability, as it plans to migrate its flagship application to a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances. The solution should allow for content-based routing as part of the architecture.

As a Solutions Architect, which of the following will you suggest for the company?

**Lựa chọn:**

<label for="q2-a"><input type="radio" id="q2-a" name="q2" value="A"> <strong>A.</strong> Use an Application Load Balancer for distributing traffic to the Amazon EC2 instances spread across different Availability Zones (AZs). Configure Auto Scaling group to mask any failure of an instance</label><br>
<label for="q2-b"><input type="radio" id="q2-b" name="q2" value="B"> <strong>B.</strong> Use a Network Load Balancer for distributing traffic to the Amazon EC2 instances spread across different Availability Zones (AZs). Configure a Private IP address to mask any failure of an instance</label><br>
<label for="q2-c"><input type="radio" id="q2-c" name="q2" value="C"> <strong>C.</strong> Use an Auto Scaling group for distributing traffic to the Amazon EC2 instances spread across different Availability Zones (AZs). Configure an elastic IP address (EIP) to mask any failure of an instance</label><br>
<label for="q2-d"><input type="radio" id="q2-d" name="q2" value="D"> <strong>D.</strong> Use an Auto Scaling group for distributing traffic to the Amazon EC2 instances spread across different Availability Zones (AZs). Configure a Public IP address to mask any failure of an instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use an Application Load Balancer for distributing traffic to the Amazon EC2 instances spread across different Availability Zones (AZs). Configure Auto Scaling group to mask any failure of an instance

</details>

---

## Câu 3

**Chủ đề:** Design Resilient Architectures

A healthcare company uses its on-premises infrastructure to run legacy applications that require specialized customizations to the underlying Oracle database as well as its host operating system (OS). The company also wants to improve the availability of the Oracle database layer. The company has hired you as an AWS Certified Solutions Architect – Associate to build a solution on AWS that meets these requirements while minimizing the underlying infrastructure maintenance effort.

Which of the following options represents the best solution for this use case?

**Lựa chọn:**

<label for="q3-a"><input type="radio" id="q3-a" name="q3" value="A"> <strong>A.</strong> Deploy the Oracle database layer on multiple Amazon EC2 instances spread across two Availability Zones (AZs). This deployment configuration guarantees high availability and also allows the Database Administrator (DBA) to access and customize the database environment and the underlying operating system</label><br>
<label for="q3-b"><input type="radio" id="q3-b" name="q3" value="B"> <strong>B.</strong> Leverage multi-AZ configuration of Amazon RDS Custom for Oracle that allows the Database Administrator (DBA) to access and customize the database environment and the underlying operating system</label><br>
<label for="q3-c"><input type="radio" id="q3-c" name="q3" value="C"> <strong>C.</strong> Leverage multi-AZ configuration of Amazon RDS for Oracle that allows the Database Administrator (DBA) to access and customize the database environment and the underlying operating system</label><br>
<label for="q3-d"><input type="radio" id="q3-d" name="q3" value="D"> <strong>D.</strong> Leverage cross AZ read-replica configuration of Amazon RDS for Oracle that allows the Database Administrator (DBA) to access and customize the database environment and the underlying operating system</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Leverage multi-AZ configuration of Amazon RDS Custom for Oracle that allows the Database Administrator (DBA) to access and customize the database environment and the underlying operating system

</details>

---

## Câu 4

**Chủ đề:** Design High-Performing Architectures

An e-commerce company manages a digital catalog of consumer products submitted by third-party sellers. Each product submission includes a description stored as a text file in an Amazon S3 bucket. These descriptions may include ingredient information for consumable products like snacks, supplements, or beverages. The company wants to build a fully automated solution that extracts ingredient names from the uploaded product descriptions and uses those names to query an Amazon DynamoDB table, which returns precomputed health and safety scores for each ingredient. Non-food items and invalid submissions can be ignored without affecting application logic. The company has no in-house machine learning (ML) experts and is looking for the most cost-effective solution with minimal operational overhead.

Which solution meets these requirements MOST cost-effectively?

**Lựa chọn:**

<label for="q4-a"><input type="radio" id="q4-a" name="q4" value="A"> <strong>A.</strong> Configure S3 Event Notifications to trigger an AWS Lambda function whenever a new product description is uploaded. Inside the function, use Amazon Comprehend's custom entity recognition feature to extract ingredient names. Store these names in the DynamoDB table and let the front-end application query for health scores</label><br>
<label for="q4-b"><input type="radio" id="q4-b" name="q4" value="B"> <strong>B.</strong> Use Amazon SageMaker with a custom-trained NLP model to identify ingredients from the uploaded descriptions. Use Amazon EventBridge to invoke a Lambda function that forwards the document content to a SageMaker endpoint and stores the results in DynamoDB. Fine-tune the model using labeled ingredient datasets from open-source repositories and retrain it monthly</label><br>
<label for="q4-c"><input type="radio" id="q4-c" name="q4" value="C"> <strong>C.</strong> Create a workflow where Amazon Transcribe is used to convert synthetic audio versions (created from text of the product descriptions) back into text. Analyze the transcripts manually or using simple keyword matching within a Lambda function. Use Amazon SNS to notify the content moderation team for each processed file</label><br>
<label for="q4-d"><input type="radio" id="q4-d" name="q4" value="D"> <strong>D.</strong> Use Amazon Lookout for Vision to scan the uploaded text files in the S3 bucket and extract entities. Invoke this workflow using an S3-triggered Lambda function. Parse the output and use Amazon API Gateway to push updates to the frontend in real time</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Configure S3 Event Notifications to trigger an AWS Lambda function whenever a new product description is uploaded. Inside the function, use Amazon Comprehend's custom entity recognition feature to extract ingredient names. Store these names in the DynamoDB table and let the front-end application query for health scores

</details>

---

## Câu 5

**Chủ đề:** Design Secure Architectures

An enterprise runs a microservices-based application on Amazon EKS, deployed on EC2 worker nodes. The application includes a frontend UI service that interacts with Amazon DynamoDB and a data-processing service that stores and retrieves files from Amazon S3. The organization needs to strictly enforce least privilege access: the UI Pods must access only DynamoDB, and the data-processing Pods must access only S3.

Which solution will best enforce these access controls within the EKS cluster?

**Lựa chọn:**

<label for="q5-a"><input type="radio" id="q5-a" name="q5" value="A"> <strong>A.</strong> Create one Kubernetes service account shared across all Pods. Attach a single IAM role to this account with both AmazonS3FullAccess and AmazonDynamoDBFullAccess policies</label><br>
<label for="q5-b"><input type="radio" id="q5-b" name="q5" value="B"> <strong>B.</strong> Create separate Kubernetes service accounts for the UI and data services. Use IAM Roles for Service Accounts (IRSA) to map each service account to an IAM role with only the required permissions. Assign DynamoDB access to the UI Pods and S3 access to the data Pods</label><br>
<label for="q5-c"><input type="radio" id="q5-c" name="q5" value="C"> <strong>C.</strong> Attach an IAM policy directly to each Pod using Kubernetes annotations. Assign the S3 policy to data-service Pods and the DynamoDB policy to UI Pods</label><br>
<label for="q5-d"><input type="radio" id="q5-d" name="q5" value="D"> <strong>D.</strong> Create IAM policies for DynamoDB and S3 access, and attach both to the EC2 instance profile used by the EKS nodes. Use Kubernetes role-based access control (RBAC) to control service-level permissions within the cluster</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create separate Kubernetes service accounts for the UI and data services. Use IAM Roles for Service Accounts (IRSA) to map each service account to an IAM role with only the required permissions. Assign DynamoDB access to the UI Pods and S3 access to the data Pods

</details>

---

## Câu 6

**Chủ đề:** Design Secure Architectures

A media company runs a photo-sharing web application that is accessed across three different countries. The application is deployed on several Amazon Elastic Compute Cloud (Amazon EC2) instances running behind an Application Load Balancer. With new government regulations, the company has been asked to block access from two countries and allow access only from the home country of the company.

Which configuration should be used to meet this changed requirement?

**Lựa chọn:**

<label for="q6-a"><input type="radio" id="q6-a" name="q6" value="A"> <strong>A.</strong> Configure the security group on the Application Load Balancer</label><br>
<label for="q6-b"><input type="radio" id="q6-b" name="q6" value="B"> <strong>B.</strong> Configure AWS Web Application Firewall (AWS WAF) on the Application Load Balancer in a Amazon Virtual Private Cloud (Amazon VPC)</label><br>
<label for="q6-c"><input type="radio" id="q6-c" name="q6" value="C"> <strong>C.</strong> Use Geo Restriction feature of Amazon CloudFront in a Amazon Virtual Private Cloud (Amazon VPC)</label><br>
<label for="q6-d"><input type="radio" id="q6-d" name="q6" value="D"> <strong>D.</strong> Configure the security group for the Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure AWS Web Application Firewall (AWS WAF) on the Application Load Balancer in a Amazon Virtual Private Cloud (Amazon VPC)

</details>

---

## Câu 7

**Chủ đề:** Design Secure Architectures

The flagship application for a gaming company connects to an Amazon Aurora database and the entire technology stack is currently deployed in the United States. Now, the company has plans to expand to Europe and Asia for its operations. It needs the games table to be accessible globally but needs the users and games_played tables to be regional only.

How would you implement this with minimal application refactoring?

**Lựa chọn:**

<label for="q7-a"><input type="radio" id="q7-a" name="q7" value="A"> <strong>A.</strong> Use an Amazon Aurora Global Database for the games table and use Amazon Aurora for the users and games_played tables</label><br>
<label for="q7-b"><input type="radio" id="q7-b" name="q7" value="B"> <strong>B.</strong> Use an Amazon Aurora Global Database for the games table and use Amazon DynamoDB tables for the users and games_played tables</label><br>
<label for="q7-c"><input type="radio" id="q7-c" name="q7" value="C"> <strong>C.</strong> Use a Amazon DynamoDB global table for the games table and use Amazon Aurora for the users and games_played tables</label><br>
<label for="q7-d"><input type="radio" id="q7-d" name="q7" value="D"> <strong>D.</strong> Use a Amazon DynamoDB global table for the games table and use Amazon DynamoDB tables for the users and games_played tables</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use an Amazon Aurora Global Database for the games table and use Amazon Aurora for the users and games_played tables

</details>

---

## Câu 8

**Chủ đề:** Design Cost-Optimized Architectures

A media agency stores its re-creatable assets on Amazon Simple Storage Service (Amazon S3) buckets. The assets are accessed by a large number of users for the first few days and the frequency of access falls down drastically after a week. Although the assets would be accessed occasionally after the first week, but they must continue to be immediately accessible when required. The cost of maintaining all the assets on Amazon S3 storage is turning out to be very expensive and the agency is looking at reducing costs as much as possible.

As an AWS Certified Solutions Architect – Associate, can you suggest a way to lower the storage costs while fulfilling the business requirements?

**Lựa chọn:**

<label for="q8-a"><input type="radio" id="q8-a" name="q8" value="A"> <strong>A.</strong> Configure a lifecycle policy to transition the objects to Amazon S3 Standard-Infrequent Access (S3 Standard-IA) after 30 days</label><br>
<label for="q8-b"><input type="radio" id="q8-b" name="q8" value="B"> <strong>B.</strong> Configure a lifecycle policy to transition the objects to Amazon S3 Standard-Infrequent Access (S3 Standard-IA) after 7 days</label><br>
<label for="q8-c"><input type="radio" id="q8-c" name="q8" value="C"> <strong>C.</strong> Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 30 days</label><br>
<label for="q8-d"><input type="radio" id="q8-d" name="q8" value="D"> <strong>D.</strong> Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 7 days</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 30 days

</details>

---

## Câu 9

**Chủ đề:** Design Cost-Optimized Architectures

A biotechnology firm runs genomics data analysis workloads using AWS Lambda functions deployed inside a VPC in their central AWS account. The input data for these workloads consists of large files stored in an Amazon Elastic File System (Amazon EFS) that resides in a separate AWS account managed by a research partner. The firm wants the Lambda function in their account to access the shared EFS storage directly. The access pattern and file volume are expected to grow as additional research datasets are added over time, so the solution must be scalable and cost-efficient, and should require minimal operational overhead.

Which solution best meets these requirements in the MOST cost-effective way?

**Lựa chọn:**

<label for="q9-a"><input type="radio" id="q9-a" name="q9" value="A"> <strong>A.</strong> Use Amazon EFS resource policies to allow cross-account access to the file system from the central account. Attach the EFS mount target to a shared VPC or peered VPC, and mount the file system in the Lambda function configuration using an EFS access point</label><br>
<label for="q9-b"><input type="radio" id="q9-b" name="q9" value="B"> <strong>B.</strong> Set up an Amazon S3 bucket in the research partner’s account and periodically copy EFS contents into the bucket using scheduled AWS DataSync jobs. Use Amazon S3 Access Points to expose the data to the Lambda function in the central account, allowing access via S3 API calls instead of file system mounts</label><br>
<label for="q9-c"><input type="radio" id="q9-c" name="q9" value="C"> <strong>C.</strong> Create a second Lambda function in the research partner's account that mounts the EFS file system locally. Have the main Lambda function in the central account invoke this secondary Lambda via Amazon API Gateway for data access and computation. Use IAM cross-account permissions to allow invocation</label><br>
<label for="q9-d"><input type="radio" id="q9-d" name="q9" value="D"> <strong>D.</strong> Package the genomic input data as a Lambda layer and publish it in the research partner's account. Share the layer across accounts by modifying its resource policy and attach the layer to the Lambda function in the central account to access the data during execution</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon EFS resource policies to allow cross-account access to the file system from the central account. Attach the EFS mount target to a shared VPC or peered VPC, and mount the file system in the Lambda function configuration using an EFS access point

</details>

---

## Câu 10

**Chủ đề:** Design Secure Architectures

A software company has a globally distributed team of developers, that requires secure and compliant access to AWS environments. The company manages multiple AWS accounts under AWS Organizations and uses an on-premises Microsoft Active Directory for user authentication. To simplify access control and identity governance across projects and accounts, the company wants a centrally managed solution that integrates with their existing infrastructure. The solution should require the least amount of ongoing operational management.

Which approach best meets the company’s requirements?

**Lựa chọn:**

<label for="q10-a"><input type="radio" id="q10-a" name="q10" value="A"> <strong>A.</strong> Deploy AWS Directory Service for Microsoft Active Directory in AWS. Establish a trust relationship with the on-premises Active Directory. Use IAM roles linked to AD groups to control access to AWS resources</label><br>
<label for="q10-b"><input type="radio" id="q10-b" name="q10" value="B"> <strong>B.</strong> Use AWS Directory Service AD Connector to connect AWS to the on-premises Active Directory. Integrate AD Connector with AWS IAM Identity Center. Use permission sets to assign access to AWS accounts and resources based on Active Directory group membership</label><br>
<label for="q10-c"><input type="radio" id="q10-c" name="q10" value="C"> <strong>C.</strong> Deploy an open-source identity provider (IdP) on Amazon EC2. Synchronize it with the on-premises Active Directory and use SAML to federate access to AWS accounts. Assign IAM roles to federated users based on SAML assertions</label><br>
<label for="q10-d"><input type="radio" id="q10-d" name="q10" value="D"> <strong>D.</strong> Use AWS Control Tower to enable account access for developers. Create AWS IAM roles in each member account and manually assign permissions. Instruct developers to assume roles across accounts using the AWS CLI</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS Directory Service AD Connector to connect AWS to the on-premises Active Directory. Integrate AD Connector with AWS IAM Identity Center. Use permission sets to assign access to AWS accounts and resources based on Active Directory group membership

</details>

---

## Câu 11

**Chủ đề:** Design High-Performing Architectures

A digital wallet company plans to launch a new cloud-based service for processing user cash transfers and peer-to-peer payments. The application will receive transaction requests from mobile clients via a secure endpoint. Each transaction request must go through a lightweight validation step before being forwarded for backend processing, which includes fraud detection, ledger updates, and notifications. The backend workload is compute- and memory-intensive, requires scaling based on volume, and must run for a longer duration than typical short-lived tasks. The engineering team prefers a fully managed solution that minimizes infrastructure maintenance, including provisioning and patching of virtual machines or containers.

Which solution will meet these requirements with the LEAST operational overhead?

**Lựa chọn:**

<label for="q11-a"><input type="radio" id="q11-a" name="q11" value="A"> <strong>A.</strong> Build a REST API using Amazon API Gateway. Integrate it with an AWS Step Functions state machine for validation. Launch the backend application using Amazon EKS with self-managed nodes, and use Kubernetes Jobs to handle transaction processing workflows. Manually scale the cluster based on demand</label><br>
<label for="q11-b"><input type="radio" id="q11-b" name="q11" value="B"> <strong>B.</strong> Configure Amazon SQS to receive encrypted payment notifications from mobile devices. Use Amazon EventBridge rules to extract the payload and perform validation. Route the messages to a backend system hosted on Amazon Lightsail instances with dynamic scaling policies based on memory thresholds and instance health checks</label><br>
<label for="q11-c"><input type="radio" id="q11-c" name="q11" value="C"> <strong>C.</strong> Expose an Amazon API Gateway REST API endpoint to receive transaction requests from mobile clients. Integrate the API with AWS Lambda to perform basic validation. For backend processing, deploy the long-running application to Amazon ECS using the Fargate launch type, allowing ECS to manage compute and memory provisioning automatically, with no server management required</label><br>
<label for="q11-d"><input type="radio" id="q11-d" name="q11" value="D"> <strong>D.</strong> Create an Amazon API Gateway endpoint to receive transaction requests from mobile devices. Use AWS Lambda to validate the transactions. For backend processing, deploy the application on Amazon EKS Anywhere, running on on-premises servers in the company’s data center. Use a custom provisioning script to scale Kubernetes worker nodes based on transaction volume</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Expose an Amazon API Gateway REST API endpoint to receive transaction requests from mobile clients. Integrate the API with AWS Lambda to perform basic validation. For backend processing, deploy the long-running application to Amazon ECS using the Fargate launch type, allowing ECS to manage compute and memory provisioning automatically, with no server management required

</details>

---

## Câu 12

**Chủ đề:** Design Secure Architectures

A company has moved its business critical data to Amazon Elastic File System (Amazon EFS) which will be accessed by multiple Amazon EC2 instances.

As an AWS Certified Solutions Architect - Associate, which of the following would you recommend to exercise access control such that only the permitted Amazon EC2 instances can read from the Amazon EFS file system? (Select two)

**Lựa chọn:**

<label for="q12-a"><input type="checkbox" id="q12-a" name="q12" value="A"> <strong>A.</strong> Use VPC security groups to control the network traffic to and from your file system</label><br>
<label for="q12-b"><input type="checkbox" id="q12-b" name="q12" value="B"> <strong>B.</strong> Use an IAM policy to control access for clients who can mount your file system with the required permissions</label><br>
<label for="q12-c"><input type="checkbox" id="q12-c" name="q12" value="C"> <strong>C.</strong> Use network access control list (network ACL) to control the network traffic to and from your Amazon EC2 instance</label><br>
<label for="q12-d"><input type="checkbox" id="q12-d" name="q12" value="D"> <strong>D.</strong> Use Amazon GuardDuty to curb unwanted access to Amazon EFS file system</label><br>
<label for="q12-e"><input type="checkbox" id="q12-e" name="q12" value="E"> <strong>E.</strong> Set up the IAM policy root credentials to control and configure the clients accessing the Amazon EFS file system</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use VPC security groups to control the network traffic to and from your file system

B. Use an IAM policy to control access for clients who can mount your file system with the required permissions

</details>

---

## Câu 13

**Chủ đề:** Design Resilient Architectures

A government agency is developing a online application to assist users in submitting permit requests through a web-based interface. The system architecture consists of a front-end web application tier and a background processing tier that handles the validation and submission of the forms. The application is expected to see high traffic and it must ensure that every submitted request is processed exactly once, with no loss of data.

Which design choice best satisfies these requirements?

**Lựa chọn:**

<label for="q13-a"><input type="radio" id="q13-a" name="q13" value="A"> <strong>A.</strong> Implement an Amazon SQS FIFO queue to reliably buffer and deliver form submissions from the web application layer to the processing tier</label><br>
<label for="q13-b"><input type="radio" id="q13-b" name="q13" value="B"> <strong>B.</strong> Implement an Amazon SQS standard queue to reliably buffer and deliver form submissions from the web application layer to the processing tier</label><br>
<label for="q13-c"><input type="radio" id="q13-c" name="q13" value="C"> <strong>C.</strong> Leverage Amazon EventBridge to send events from the web application to the processing tier for asynchronous form handling</label><br>
<label for="q13-d"><input type="radio" id="q13-d" name="q13" value="D"> <strong>D.</strong> Leverage Amazon API Gateway to pass the form submissions to AWS Lambda for processing in real time</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Implement an Amazon SQS FIFO queue to reliably buffer and deliver form submissions from the web application layer to the processing tier

</details>

---

## Câu 14

**Chủ đề:** Design Cost-Optimized Architectures

A leading social media analytics company is contemplating moving its dockerized application stack into AWS Cloud. The company is not sure about the pricing for using Amazon Elastic Container Service (Amazon ECS) with the EC2 launch type compared to the Amazon Elastic Container Service (Amazon ECS) with the Fargate launch type.

Which of the following is correct regarding the pricing for these two services?

**Lựa chọn:**

<label for="q14-a"><input type="radio" id="q14-a" name="q14" value="A"> <strong>A.</strong> Amazon ECS with EC2 launch type is charged based on EC2 instances and EBS volumes used. Amazon ECS with Fargate launch type is charged based on vCPU and memory resources that the containerized application requests</label><br>
<label for="q14-b"><input type="radio" id="q14-b" name="q14" value="B"> <strong>B.</strong> Both Amazon ECS with EC2 launch type and Amazon ECS with Fargate launch type are just charged based on Elastic Container Service used per hour</label><br>
<label for="q14-c"><input type="radio" id="q14-c" name="q14" value="C"> <strong>C.</strong> Both Amazon ECS with EC2 launch type and Amazon ECS with Fargate launch type are charged based on vCPU and memory resources that the containerized application requests</label><br>
<label for="q14-d"><input type="radio" id="q14-d" name="q14" value="D"> <strong>D.</strong> Both Amazon ECS with EC2 launch type and Amazon ECS with Fargate launch type are charged based on Amazon EC2 instances and Amazon EBS Elastic Volumes used</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon ECS with EC2 launch type is charged based on EC2 instances and EBS volumes used. Amazon ECS with Fargate launch type is charged based on vCPU and memory resources that the containerized application requests

</details>

---

## Câu 15

**Chủ đề:** Design Cost-Optimized Architectures

An audit department generates and accesses the audit reports only twice in a financial year. The department uses AWS Step Functions to orchestrate the report creating process that has failover and retry scenarios built into the solution. The underlying data to create these audit reports is stored on Amazon S3, runs into hundreds of Terabytes and should be available with millisecond latency.

As an AWS Certified Solutions Architect – Associate, which is the MOST cost-effective storage class that you would recommend to be used for this use-case?

**Lựa chọn:**

<label for="q15-a"><input type="radio" id="q15-a" name="q15" value="A"> <strong>A.</strong> Amazon S3 Intelligent-Tiering (S3 Intelligent-Tiering)</label><br>
<label for="q15-b"><input type="radio" id="q15-b" name="q15" value="B"> <strong>B.</strong> Amazon S3 Standard-Infrequent Access (S3 Standard-IA)</label><br>
<label for="q15-c"><input type="radio" id="q15-c" name="q15" value="C"> <strong>C.</strong> Amazon S3 Standard</label><br>
<label for="q15-d"><input type="radio" id="q15-d" name="q15" value="D"> <strong>D.</strong> Amazon S3 Glacier Deep Archive</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Amazon S3 Standard-Infrequent Access (S3 Standard-IA)

</details>

---

## Câu 16

**Chủ đề:** Design Secure Architectures

A new DevOps engineer has joined a large financial services company recently. As part of his onboarding, the IT department is conducting a review of the checklist for tasks related to AWS Identity and Access Management (AWS IAM).

As an AWS Certified Solutions Architect – Associate, which best practices would you recommend (Select two)?

**Lựa chọn:**

<label for="q16-a"><input type="checkbox" id="q16-a" name="q16" value="A"> <strong>A.</strong> Create a minimum number of accounts and share these account credentials among employees</label><br>
<label for="q16-b"><input type="checkbox" id="q16-b" name="q16" value="B"> <strong>B.</strong> Grant maximum privileges to avoid assigning privileges again</label><br>
<label for="q16-c"><input type="checkbox" id="q16-c" name="q16" value="C"> <strong>C.</strong> Enable AWS Multi-Factor Authentication (AWS MFA) for privileged users</label><br>
<label for="q16-d"><input type="checkbox" id="q16-d" name="q16" value="D"> <strong>D.</strong> Use user credentials to provide access specific permissions for Amazon EC2 instances</label><br>
<label for="q16-e"><input type="checkbox" id="q16-e" name="q16" value="E"> <strong>E.</strong> Configure AWS CloudTrail to log all AWS Identity and Access Management (AWS IAM) actions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Enable AWS Multi-Factor Authentication (AWS MFA) for privileged users

E. Configure AWS CloudTrail to log all AWS Identity and Access Management (AWS IAM) actions

</details>

---

## Câu 17

**Chủ đề:** Design Secure Architectures

An organization wants to delegate access to a set of users from the development environment so that they can access some resources in the production environment which is managed under another AWS account.

As a solutions architect, which of the following steps would you recommend?

**Lựa chọn:**

<label for="q17-a"><input type="radio" id="q17-a" name="q17" value="A"> <strong>A.</strong> Create new IAM user credentials for the production environment and share these credentials with the set of users from the development environment</label><br>
<label for="q17-b"><input type="radio" id="q17-b" name="q17" value="B"> <strong>B.</strong> Create a new IAM role with the required permissions to access the resources in the production environment. The users can then assume this IAM role while accessing the resources from the production environment</label><br>
<label for="q17-c"><input type="radio" id="q17-c" name="q17" value="C"> <strong>C.</strong> It is not possible to access cross-account resources</label><br>
<label for="q17-d"><input type="radio" id="q17-d" name="q17" value="D"> <strong>D.</strong> Both IAM roles and IAM users can be used interchangeably for cross-account access</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create a new IAM role with the required permissions to access the resources in the production environment. The users can then assume this IAM role while accessing the resources from the production environment

</details>

---

## Câu 18

**Chủ đề:** Design Cost-Optimized Architectures

A news network uses Amazon Simple Storage Service (Amazon S3) to aggregate the raw video footage from its reporting teams across the US. The news network has recently expanded into new geographies in Europe and Asia. The technical teams at the overseas branch offices have reported huge delays in uploading large video files to the destination Amazon S3 bucket.

Which of the following are the MOST cost-effective options to improve the file upload speed into Amazon S3 (Select two)

**Lựa chọn:**

<label for="q18-a"><input type="checkbox" id="q18-a" name="q18" value="A"> <strong>A.</strong> Create multiple AWS Site-to-Site VPN connections between the AWS Cloud and branch offices in Europe and Asia. Use these VPN connections for faster file uploads into Amazon S3</label><br>
<label for="q18-b"><input type="checkbox" id="q18-b" name="q18" value="B"> <strong>B.</strong> Create multiple AWS Direct Connect connections between the AWS Cloud and branch offices in Europe and Asia. Use the direct connect connections for faster file uploads into Amazon S3</label><br>
<label for="q18-c"><input type="checkbox" id="q18-c" name="q18" value="C"> <strong>C.</strong> Use Amazon S3 Transfer Acceleration (Amazon S3TA) to enable faster file uploads into the destination S3 bucket</label><br>
<label for="q18-d"><input type="checkbox" id="q18-d" name="q18" value="D"> <strong>D.</strong> Use multipart uploads for faster file uploads into the destination Amazon S3 bucket</label><br>
<label for="q18-e"><input type="checkbox" id="q18-e" name="q18" value="E"> <strong>E.</strong> Use AWS Global Accelerator for faster file uploads into the destination Amazon S3 bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Amazon S3 Transfer Acceleration (Amazon S3TA) to enable faster file uploads into the destination S3 bucket

D. Use multipart uploads for faster file uploads into the destination Amazon S3 bucket

</details>

---

## Câu 19

**Chủ đề:** Design Cost-Optimized Architectures

The IT department at a consulting firm is conducting a training workshop for new developers. As part of an evaluation exercise on Amazon S3, the new developers were asked to identify the invalid storage class lifecycle transitions for objects stored on Amazon S3.

Can you spot the INVALID lifecycle transitions from the options below? (Select two)

**Lựa chọn:**

<label for="q19-a"><input type="checkbox" id="q19-a" name="q19" value="A"> <strong>A.</strong> Amazon S3 Intelligent-Tiering => Amazon S3 Standard</label><br>
<label for="q19-b"><input type="checkbox" id="q19-b" name="q19" value="B"> <strong>B.</strong> Amazon S3 One Zone-IA => Amazon S3 Standard-IA</label><br>
<label for="q19-c"><input type="checkbox" id="q19-c" name="q19" value="C"> <strong>C.</strong> Amazon S3 Standard => Amazon S3 Intelligent-Tiering</label><br>
<label for="q19-d"><input type="checkbox" id="q19-d" name="q19" value="D"> <strong>D.</strong> Amazon S3 Standard-IA => Amazon S3 Intelligent-Tiering</label><br>
<label for="q19-e"><input type="checkbox" id="q19-e" name="q19" value="E"> <strong>E.</strong> Amazon S3 Standard-IA => Amazon S3 One Zone-IA</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon S3 Intelligent-Tiering => Amazon S3 Standard

B. Amazon S3 One Zone-IA => Amazon S3 Standard-IA

</details>

---

## Câu 20

**Chủ đề:** Design Resilient Architectures

A healthcare startup needs to enforce compliance and regulatory guidelines for objects stored in Amazon S3. One of the key requirements is to provide adequate protection against accidental deletion of objects.

As a solutions architect, what are your recommendations to address these guidelines? (Select two) ?

**Lựa chọn:**

<label for="q20-a"><input type="checkbox" id="q20-a" name="q20" value="A"> <strong>A.</strong> Establish a process to get managerial approval for deleting Amazon S3 objects</label><br>
<label for="q20-b"><input type="checkbox" id="q20-b" name="q20" value="B"> <strong>B.</strong> Create an event trigger on deleting any Amazon S3 object. The event invokes an Amazon Simple Notification Service (Amazon SNS) notification via email to the IT manager</label><br>
<label for="q20-c"><input type="checkbox" id="q20-c" name="q20" value="C"> <strong>C.</strong> Enable versioning on the Amazon S3 bucket</label><br>
<label for="q20-d"><input type="checkbox" id="q20-d" name="q20" value="D"> <strong>D.</strong> Change the configuration on Amazon S3 console so that the user needs to provide additional confirmation while deleting any Amazon S3 object</label><br>
<label for="q20-e"><input type="checkbox" id="q20-e" name="q20" value="E"> <strong>E.</strong> Enable multi-factor authentication (MFA) delete on the Amazon S3 bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Enable versioning on the Amazon S3 bucket

E. Enable multi-factor authentication (MFA) delete on the Amazon S3 bucket

</details>

---

## Câu 21

**Chủ đề:** Design Cost-Optimized Architectures

A company runs a data processing workflow that takes about 60 minutes to complete. The workflow can withstand disruptions and it can be started and stopped multiple times.

Which is the most cost-effective solution to build a solution for the workflow?

**Lựa chọn:**

<label for="q21-a"><input type="radio" id="q21-a" name="q21" value="A"> <strong>A.</strong> Use AWS Lambda function to run the workflow processes</label><br>
<label for="q21-b"><input type="radio" id="q21-b" name="q21" value="B"> <strong>B.</strong> Use Amazon EC2 on-demand instances to run the workflow processes</label><br>
<label for="q21-c"><input type="radio" id="q21-c" name="q21" value="C"> <strong>C.</strong> Use Amazon EC2 reserved instances to run the workflow processes</label><br>
<label for="q21-d"><input type="radio" id="q21-d" name="q21" value="D"> <strong>D.</strong> Use Amazon EC2 spot instances to run the workflow processes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon EC2 spot instances to run the workflow processes

</details>

---

## Câu 22

**Chủ đề:** Design Secure Architectures

A US-based healthcare startup is building an interactive diagnostic tool for COVID-19 related assessments. The users would be required to capture their personal health records via this tool. As this is sensitive health information, the backup of the user data must be kept encrypted in Amazon Simple Storage Service (Amazon S3). The startup does not want to provide its own encryption keys but still wants to maintain an audit trail of when an encryption key was used and by whom.

Which of the following is the BEST solution for this use-case?

**Lựa chọn:**

<label for="q22-a"><input type="radio" id="q22-a" name="q22" value="A"> <strong>A.</strong> Use server-side encryption with Amazon S3 managed keys (SSE-S3) to encrypt the user data on Amazon S3</label><br>
<label for="q22-b"><input type="radio" id="q22-b" name="q22" value="B"> <strong>B.</strong> Use server-side encryption with AWS Key Management Service keys (SSE-KMS) to encrypt the user data on Amazon S3</label><br>
<label for="q22-c"><input type="radio" id="q22-c" name="q22" value="C"> <strong>C.</strong> Use server-side encryption with customer-provided keys (SSE-C) to encrypt the user data on Amazon S3</label><br>
<label for="q22-d"><input type="radio" id="q22-d" name="q22" value="D"> <strong>D.</strong> Use client-side encryption with client provided keys and then upload the encrypted user data to Amazon S3</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use server-side encryption with AWS Key Management Service keys (SSE-KMS) to encrypt the user data on Amazon S3

</details>

---

## Câu 23

**Chủ đề:** Design High-Performing Architectures

An ivy-league university is assisting NASA to find potential landing sites for exploration vehicles of unmanned missions to our neighboring planets. The university uses High Performance Computing (HPC) driven application architecture to identify these landing sites.

Which of the following Amazon EC2 instance topologies should this application be deployed on?

**Lựa chọn:**

<label for="q23-a"><input type="radio" id="q23-a" name="q23" value="A"> <strong>A.</strong> The Amazon EC2 instances should be deployed in a spread placement group so that there are no correlated failures</label><br>
<label for="q23-b"><input type="radio" id="q23-b" name="q23" value="B"> <strong>B.</strong> The Amazon EC2 instances should be deployed in a partition placement group so that distributed workloads can be handled effectively</label><br>
<label for="q23-c"><input type="radio" id="q23-c" name="q23" value="C"> <strong>C.</strong> The Amazon EC2 instances should be deployed in a cluster placement group so that the underlying workload can benefit from low network latency and high network throughput</label><br>
<label for="q23-d"><input type="radio" id="q23-d" name="q23" value="D"> <strong>D.</strong> The Amazon EC2 instances should be deployed in an Auto Scaling group so that application meets high availability requirements</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. The Amazon EC2 instances should be deployed in a cluster placement group so that the underlying workload can benefit from low network latency and high network throughput

</details>

---

## Câu 24

**Chủ đề:** Design High-Performing Architectures

An Electronic Design Automation (EDA) application produces massive volumes of data that can be divided into two categories. The 'hot data' needs to be both processed and stored quickly in a parallel and distributed fashion. The 'cold data' needs to be kept for reference with quick access for reads and updates at a low cost.

Which of the following AWS services is BEST suited to accelerate the aforementioned chip design process?

**Lựa chọn:**

<label for="q24-a"><input type="radio" id="q24-a" name="q24" value="A"> <strong>A.</strong> Amazon FSx for Windows File Server</label><br>
<label for="q24-b"><input type="radio" id="q24-b" name="q24" value="B"> <strong>B.</strong> Amazon EMR</label><br>
<label for="q24-c"><input type="radio" id="q24-c" name="q24" value="C"> <strong>C.</strong> Amazon FSx for Lustre</label><br>
<label for="q24-d"><input type="radio" id="q24-d" name="q24" value="D"> <strong>D.</strong> AWS Glue</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Amazon FSx for Lustre

</details>

---

## Câu 25

**Chủ đề:** Design Secure Architectures

An IT company wants to review its security best-practices after an incident was reported where a new developer on the team was assigned full access to Amazon DynamoDB. The developer accidentally deleted a couple of tables from the production environment while building out a new feature.

Which is the MOST effective way to address this issue so that such incidents do not recur?

**Lựa chọn:**

<label for="q25-a"><input type="radio" id="q25-a" name="q25" value="A"> <strong>A.</strong> The CTO should review the permissions for each new developer's IAM user so that such incidents don't recur</label><br>
<label for="q25-b"><input type="radio" id="q25-b" name="q25" value="B"> <strong>B.</strong> Remove full database access for all IAM users in the organization</label><br>
<label for="q25-c"><input type="radio" id="q25-c" name="q25" value="C"> <strong>C.</strong> Only root user should have full database access in the organization</label><br>
<label for="q25-d"><input type="radio" id="q25-d" name="q25" value="D"> <strong>D.</strong> Use permissions boundary to control the maximum permissions employees can grant to the IAM principals</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use permissions boundary to control the maximum permissions employees can grant to the IAM principals

</details>

---

## Câu 26

**Chủ đề:** Design High-Performing Architectures

A retail analytics company operates a large-scale data lake on Amazon S3, where they store daily logs of customer transactions, product views, and inventory updates. Each morning, they need to transform and load the data into a data warehouse to support fast analytical queries. The company also wants to enable data analysts to build and train machine learning (ML) models using familiar SQL syntax without writing custom Python code. The architecture must support massively parallel processing (MPP) for fast data aggregation and scoring, and must use serverless AWS services wherever possible to reduce infrastructure management and operational overhead.

Which solution best meets these requirements?

**Lựa chọn:**

<label for="q26-a"><input type="radio" id="q26-a" name="q26" value="A"> <strong>A.</strong> Use a daily AWS Glue job to transform and clean the data stored in Amazon S3. Load the transformed dataset into Amazon Redshift Serverless, which offers MPP capabilities in a serverless model. Enable analysts to use Amazon Redshift ML to build and train ML models</label><br>
<label for="q26-b"><input type="radio" id="q26-b" name="q26" value="B"> <strong>B.</strong> Provision and run a daily Amazon EMR cluster with Apache Spark to process and transform the S3 data. Load the results into Amazon Redshift (provisioned). Enable ML model development by integrating Redshift with Amazon SageMaker notebooks for advanced modeling tasks</label><br>
<label for="q26-c"><input type="radio" id="q26-c" name="q26" value="C"> <strong>C.</strong> Use an AWS Glue job to transform and load data into Amazon RDS for PostgreSQL. Allow analysts to run machine learning models using Amazon Aurora ML integrated with PostgreSQL, leveraging Amazon SageMaker endpoints behind the scenes</label><br>
<label for="q26-d"><input type="radio" id="q26-d" name="q26" value="D"> <strong>D.</strong> Run a daily AWS Glue job to process and transform the raw files in S3 and register the outputs as Amazon Athena tables in AWS Glue Data Catalog. Allow analysts to build ML models using Amazon Athena ML, with SQL-based predictions on top of S3 data without moving it to a warehouse</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use a daily AWS Glue job to transform and clean the data stored in Amazon S3. Load the transformed dataset into Amazon Redshift Serverless, which offers MPP capabilities in a serverless model. Enable analysts to use Amazon Redshift ML to build and train ML models

</details>

---

## Câu 27

**Chủ đề:** Design Secure Architectures

A financial services company operates a containerized microservices architecture using Kubernetes in its on-premises data center. Due to strict industry regulations and internal security policies, all application data and workloads must remain physically within the on-premises environment. The company’s infrastructure team wants to modernize its Kubernetes stack and take advantage of AWS-managed services and APIs, including automated Kubernetes upgrades, Amazon CloudWatch integration, and access to AWS IAM features — but without migrating any data or compute resources to the cloud.

Which AWS solution will best meet the company’s requirements for modernization while ensuring that all data remains on premises?

**Lựa chọn:**

<label for="q27-a"><input type="radio" id="q27-a" name="q27" value="A"> <strong>A.</strong> Set up a dedicated AWS Direct Connect connection between the on-premises environment and an AWS Region. Deploy Amazon EKS in the cloud and connect it to the local Kubernetes cluster. Use IAM roles and API Gateway to integrate authentication and traffic flow for hybrid workloads</label><br>
<label for="q27-b"><input type="radio" id="q27-b" name="q27" value="B"> <strong>B.</strong> Deploy Amazon ECS with Fargate in a nearby AWS Local Zone. Use CloudWatch Logs to forward events to the primary region. Connect the Local Zone to the company’s data center over a VPN. Configure containers to pull data from on-premises storage through a mounted file share</label><br>
<label for="q27-c"><input type="radio" id="q27-c" name="q27" value="C"> <strong>C.</strong> Use an AWS Snowball Edge Compute Optimized device to run EKS-compatible Docker containers on-site. Periodically export application logs and container snapshots to Amazon S3 using Snowball’s offline data transfer features. Use the Snowball console to orchestrate workloads in batches</label><br>
<label for="q27-d"><input type="radio" id="q27-d" name="q27" value="D"> <strong>D.</strong> Install an AWS Outposts rack in the company’s data center. Use Amazon EKS Anywhere on Outposts to run containerized workloads locally while integrating with AWS APIs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Install an AWS Outposts rack in the company’s data center. Use Amazon EKS Anywhere on Outposts to run containerized workloads locally while integrating with AWS APIs

</details>

---

## Câu 28

**Chủ đề:** Design Cost-Optimized Architectures

A leading video streaming service delivers billions of hours of content from Amazon Simple Storage Service (Amazon S3) to customers around the world. Amazon S3 also serves as the data lake for its big data analytics solution. The data lake has a staging zone where intermediary query results are kept only for 24 hours. These results are also heavily referenced by other parts of the analytics pipeline.

Which of the following is the MOST cost-effective strategy for storing this intermediary query data?

**Lựa chọn:**

<label for="q28-a"><input type="radio" id="q28-a" name="q28" value="A"> <strong>A.</strong> Store the intermediary query results in Amazon S3 Standard storage class</label><br>
<label for="q28-b"><input type="radio" id="q28-b" name="q28" value="B"> <strong>B.</strong> Store the intermediary query results in Amazon S3 Glacier Instant Retrieval storage class</label><br>
<label for="q28-c"><input type="radio" id="q28-c" name="q28" value="C"> <strong>C.</strong> Store the intermediary query results in Amazon S3 Standard-Infrequent Access storage class</label><br>
<label for="q28-d"><input type="radio" id="q28-d" name="q28" value="D"> <strong>D.</strong> Store the intermediary query results in Amazon S3 One Zone-Infrequent Access storage class</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Store the intermediary query results in Amazon S3 Standard storage class

</details>

---

## Câu 29

**Chủ đề:** Design High-Performing Architectures

The engineering team at an in-home fitness company is evaluating multiple in-memory data stores with the ability to power its on-demand, live leaderboard. The company's leaderboard requires high availability, low latency, and real-time processing to deliver customizable user data for the community of users working out together virtually from the comfort of their home.

As a solutions architect, which of the following solutions would you recommend? (Select two)

**Lựa chọn:**

<label for="q29-a"><input type="checkbox" id="q29-a" name="q29" value="A"> <strong>A.</strong> Power the on-demand, live leaderboard using Amazon DynamoDB as it meets the in-memory, high availability, low latency requirements</label><br>
<label for="q29-b"><input type="checkbox" id="q29-b" name="q29" value="B"> <strong>B.</strong> Power the on-demand, live leaderboard using Amazon ElastiCache for Redis as it meets the in-memory, high availability, low latency requirements</label><br>
<label for="q29-c"><input type="checkbox" id="q29-c" name="q29" value="C"> <strong>C.</strong> Power the on-demand, live leaderboard using Amazon DynamoDB with DynamoDB Accelerator (DAX) as it meets the in-memory, high availability, low latency requirements</label><br>
<label for="q29-d"><input type="checkbox" id="q29-d" name="q29" value="D"> <strong>D.</strong> Power the on-demand, live leaderboard using Amazon Neptune as it meets the in-memory, high availability, low latency requirements</label><br>
<label for="q29-e"><input type="checkbox" id="q29-e" name="q29" value="E"> <strong>E.</strong> Power the on-demand, live leaderboard using Amazon RDS for Aurora as it meets the in-memory, high availability, low latency requirements</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Power the on-demand, live leaderboard using Amazon ElastiCache for Redis as it meets the in-memory, high availability, low latency requirements

C. Power the on-demand, live leaderboard using Amazon DynamoDB with DynamoDB Accelerator (DAX) as it meets the in-memory, high availability, low latency requirements

</details>

---

## Câu 30

**Chủ đề:** Design High-Performing Architectures

The engineering team at a data analytics company has observed that its flagship application functions at its peak performance when the underlying Amazon Elastic Compute Cloud (Amazon EC2) instances have a CPU utilization of about 50%. The application is built on a fleet of Amazon EC2 instances managed under an Auto Scaling group. The workflow requests are handled by an internal Application Load Balancer that routes the requests to the instances.

As a solutions architect, what would you recommend so that the application runs near its peak performance state?

**Lựa chọn:**

<label for="q30-a"><input type="radio" id="q30-a" name="q30" value="A"> <strong>A.</strong> Configure the Auto Scaling group to use target tracking policy and set the CPU utilization as the target metric with a target value of 50%</label><br>
<label for="q30-b"><input type="radio" id="q30-b" name="q30" value="B"> <strong>B.</strong> Configure the Auto Scaling group to use step scaling policy and set the CPU utilization as the target metric with a target value of 50%</label><br>
<label for="q30-c"><input type="radio" id="q30-c" name="q30" value="C"> <strong>C.</strong> Configure the Auto Scaling group to use simple scaling policy and set the CPU utilization as the target metric with a target value of 50%</label><br>
<label for="q30-d"><input type="radio" id="q30-d" name="q30" value="D"> <strong>D.</strong> Configure the Auto Scaling group to use a Amazon Cloudwatch alarm triggered on a CPU utilization threshold of 50%</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Configure the Auto Scaling group to use target tracking policy and set the CPU utilization as the target metric with a target value of 50%

</details>

---

## Câu 31

**Chủ đề:** Design Secure Architectures

An IT consultant is helping the owner of a medium-sized business set up an AWS account. What are the security recommendations he must follow while creating the AWS account root user? (Select two)

**Lựa chọn:**

<label for="q31-a"><input type="checkbox" id="q31-a" name="q31" value="A"> <strong>A.</strong> Create a strong password for the AWS account root user</label><br>
<label for="q31-b"><input type="checkbox" id="q31-b" name="q31" value="B"> <strong>B.</strong> Encrypt the access keys and save them on Amazon S3</label><br>
<label for="q31-c"><input type="checkbox" id="q31-c" name="q31" value="C"> <strong>C.</strong> Create AWS account root user access keys and share those keys only with the business owner</label><br>
<label for="q31-d"><input type="checkbox" id="q31-d" name="q31" value="D"> <strong>D.</strong> Send an email to the business owner with details of the login username and password for the AWS root user. This will help the business owner to troubleshoot any login issues in future</label><br>
<label for="q31-e"><input type="checkbox" id="q31-e" name="q31" value="E"> <strong>E.</strong> Enable Multi Factor Authentication (MFA) for the AWS account root user account</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a strong password for the AWS account root user

E. Enable Multi Factor Authentication (MFA) for the AWS account root user account

</details>

---

## Câu 32

**Chủ đề:** Design Resilient Architectures

The DevOps team at an e-commerce company wants to perform some maintenance work on a specific Amazon EC2 instance that is part of an Auto Scaling group using a step scaling policy. The team is facing a maintenance challenge - every time the team deploys a maintenance patch, the instance health check status shows as out of service for a few minutes. This causes the Auto Scaling group to provision another replacement instance immediately.

As a solutions architect, which are the MOST time/resource efficient steps that you would recommend so that the maintenance work can be completed at the earliest? (Select two)

**Lựa chọn:**

<label for="q32-a"><input type="checkbox" id="q32-a" name="q32" value="A"> <strong>A.</strong> Put the instance into the Standby state and then update the instance by applying the maintenance patch. Once the instance is ready, you can exit the Standby state and then return the instance to service</label><br>
<label for="q32-b"><input type="checkbox" id="q32-b" name="q32" value="B"> <strong>B.</strong> Take a snapshot of the instance, create a new Amazon Machine Image (AMI) and then launch a new instance using this AMI. Apply the maintenance patch to this new instance and then add it back to the Auto Scaling Group by using the manual scaling policy. Terminate the earlier instance that had the maintenance issue</label><br>
<label for="q32-c"><input type="checkbox" id="q32-c" name="q32" value="C"> <strong>C.</strong> Delete the Auto Scaling group and apply the maintenance fix to the given instance. Create a new Auto Scaling group and add all the instances again using the manual scaling policy</label><br>
<label for="q32-d"><input type="checkbox" id="q32-d" name="q32" value="D"> <strong>D.</strong> Suspend the ReplaceUnhealthy process type for the Auto Scaling group and apply the maintenance patch to the instance. Once the instance is ready, you can manually set the instance's health status back to healthy and activate the ReplaceUnhealthy process type again</label><br>
<label for="q32-e"><input type="checkbox" id="q32-e" name="q32" value="E"> <strong>E.</strong> Suspend the ScheduledActions process type for the Auto Scaling group and apply the maintenance patch to the instance. Once the instance is ready, you can you can manually set the instance's health status back to healthy and activate the ScheduledActions process type again</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Put the instance into the Standby state and then update the instance by applying the maintenance patch. Once the instance is ready, you can exit the Standby state and then return the instance to service

D. Suspend the ReplaceUnhealthy process type for the Auto Scaling group and apply the maintenance patch to the instance. Once the instance is ready, you can manually set the instance's health status back to healthy and activate the ReplaceUnhealthy process type again

</details>

---

## Câu 33

**Chủ đề:** Design Resilient Architectures

A leading carmaker would like to build a new car-as-a-sensor service by leveraging fully serverless components that are provisioned and managed automatically by AWS. The development team at the carmaker does not want an option that requires the capacity to be manually provisioned, as it does not want to respond manually to changing volumes of sensor data.

Given these constraints, which of the following solutions is the BEST fit to develop this car-as-a-sensor service?

**Lựa chọn:**

<label for="q33-a"><input type="radio" id="q33-a" name="q33" value="A"> <strong>A.</strong> Ingest the sensor data in an Amazon Simple Queue Service (Amazon SQS) standard queue, which is polled by an AWS Lambda function in batches and the data is written into an auto-scaled Amazon DynamoDB table for downstream processing</label><br>
<label for="q33-b"><input type="radio" id="q33-b" name="q33" value="B"> <strong>B.</strong> Ingest the sensor data in an Amazon Simple Queue Service (Amazon SQS) standard queue, which is polled by an application running on an Amazon EC2 instance and the data is written into an auto-scaled Amazon DynamoDB table for downstream processing</label><br>
<label for="q33-c"><input type="radio" id="q33-c" name="q33" value="C"> <strong>C.</strong> Ingest the sensor data in Amazon Kinesis Data Firehose, which directly writes the data into an auto-scaled Amazon DynamoDB table for downstream processing</label><br>
<label for="q33-d"><input type="radio" id="q33-d" name="q33" value="D"> <strong>D.</strong> Ingest the sensor data in Amazon Kinesis Data Streams, which is polled by an application running on an Amazon EC2 instance and the data is written into an auto-scaled Amazon DynamoDB table for downstream processing</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Ingest the sensor data in an Amazon Simple Queue Service (Amazon SQS) standard queue, which is polled by an AWS Lambda function in batches and the data is written into an auto-scaled Amazon DynamoDB table for downstream processing

</details>

---

## Câu 34

**Chủ đề:** Design Resilient Architectures

A major bank is using Amazon Simple Queue Service (Amazon SQS) to migrate several core banking applications to the cloud to ensure high availability and cost efficiency while simplifying administrative complexity and overhead. The development team at the bank expects a peak rate of about 1000 messages per second to be processed via SQS. It is important that the messages are processed in order.

Which of the following options can be used to implement this system?

**Lựa chọn:**

<label for="q34-a"><input type="radio" id="q34-a" name="q34" value="A"> <strong>A.</strong> Use Amazon SQS standard queue to process the messages</label><br>
<label for="q34-b"><input type="radio" id="q34-b" name="q34" value="B"> <strong>B.</strong> Use Amazon SQS FIFO (First-In-First-Out) queue to process the messages</label><br>
<label for="q34-c"><input type="radio" id="q34-c" name="q34" value="C"> <strong>C.</strong> Use Amazon SQS FIFO (First-In-First-Out) queue in batch mode of 4 messages per operation to process the messages at the peak rate</label><br>
<label for="q34-d"><input type="radio" id="q34-d" name="q34" value="D"> <strong>D.</strong> Use Amazon SQS FIFO (First-In-First-Out) queue in batch mode of 2 messages per operation to process the messages at the peak rate</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Amazon SQS FIFO (First-In-First-Out) queue in batch mode of 4 messages per operation to process the messages at the peak rate

</details>

---

## Câu 35

**Chủ đề:** Design Cost-Optimized Architectures

A video analytics company runs data-intensive batch processing workloads that generate large log files and metadata daily. These files are currently stored in an on-premises NFS-based storage system located in the company's primary data center. However, the storage system is becoming increasingly difficult to scale and is unable to meet the company's growing storage demands. The IT team wants to migrate to a cloud-based storage solution that minimizes costs, retains NFS compatibility, and supports automated tiering of rarely accessed data to lower-cost storage. The team prefers to continue using existing NFS-based tools and protocols for compatibility with their current application stack.

Which solution will meet these requirements MOST cost-effectively?

**Lựa chọn:**

<label for="q35-a"><input type="radio" id="q35-a" name="q35" value="A"> <strong>A.</strong> Provision an Amazon Elastic File System (Amazon EFS) file system with the One Zone–IA storage class. Use AWS DataSync to migrate the NFS data to EFS. Configure the application to mount the file system over NFS and activate lifecycle management to tier infrequently accessed files</label><br>
<label for="q35-b"><input type="radio" id="q35-b" name="q35" value="B"> <strong>B.</strong> Deploy an AWS Storage Gateway Volume Gateway in cached mode. Attach it as a block device to an on-premises file server and mount NFS on top. Store snapshots in Amazon S3 Glacier Deep Archive, and use AWS Backup to manage recovery operations and tiering</label><br>
<label for="q35-c"><input type="radio" id="q35-c" name="q35" value="C"> <strong>C.</strong> Deploy an AWS Storage Gateway File Gateway on premises. Configure it to present an NFS-compatible file share to the workloads. Store the uploaded files in Amazon S3, and use S3 Lifecycle policies to automatically transition infrequently accessed objects to lower-cost storage classes</label><br>
<label for="q35-d"><input type="radio" id="q35-d" name="q35" value="D"> <strong>D.</strong> Use Amazon FSx for Windows File Server to replace the NFS workload. Enable data deduplication and automatic backups. Use Amazon S3 Glacier to move snapshots to a cost-efficient storage tier. Reconfigure the analytics application to access files using SMB protocol</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Deploy an AWS Storage Gateway File Gateway on premises. Configure it to present an NFS-compatible file share to the workloads. Store the uploaded files in Amazon S3, and use S3 Lifecycle policies to automatically transition infrequently accessed objects to lower-cost storage classes

</details>

---

## Câu 36

**Chủ đề:** Design Secure Architectures

An IT security consultancy is working on a solution to protect data stored in Amazon S3 from any malicious activity as well as check for any vulnerabilities on Amazon EC2 instances.

As a solutions architect, which of the following solutions would you suggest to help address the given requirement?

**Lựa chọn:**

<label for="q36-a"><input type="radio" id="q36-a" name="q36" value="A"> <strong>A.</strong> Use Amazon GuardDuty to monitor any malicious activity on data stored in Amazon S3. Use security assessments provided by Amazon Inspector to check for vulnerabilities on Amazon EC2 instances</label><br>
<label for="q36-b"><input type="radio" id="q36-b" name="q36" value="B"> <strong>B.</strong> Use Amazon GuardDuty to monitor any malicious activity on data stored in Amazon S3. Use security assessments provided by Amazon GuardDuty to check for vulnerabilities on Amazon EC2 instances</label><br>
<label for="q36-c"><input type="radio" id="q36-c" name="q36" value="C"> <strong>C.</strong> Use Amazon Inspector to monitor any malicious activity on data stored in Amazon S3. Use security assessments provided by Amazon Inspector to check for vulnerabilities on Amazon EC2 instances</label><br>
<label for="q36-d"><input type="radio" id="q36-d" name="q36" value="D"> <strong>D.</strong> Use Amazon Inspector to monitor any malicious activity on data stored in Amazon S3. Use security assessments provided by Amazon GuardDuty to check for vulnerabilities on Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon GuardDuty to monitor any malicious activity on data stored in Amazon S3. Use security assessments provided by Amazon Inspector to check for vulnerabilities on Amazon EC2 instances

</details>

---

## Câu 37

**Chủ đề:** Design High-Performing Architectures

The engineering team at an e-commerce company wants to establish a dedicated, encrypted, low latency, and high throughput connection between its data center and AWS Cloud. The engineering team has set aside sufficient time to account for the operational overhead of establishing this connection.

As a solutions architect, which of the following solutions would you recommend to the company?

**Lựa chọn:**

<label for="q37-a"><input type="radio" id="q37-a" name="q37" value="A"> <strong>A.</strong> Use AWS Direct Connect to establish a connection between the data center and AWS Cloud</label><br>
<label for="q37-b"><input type="radio" id="q37-b" name="q37" value="B"> <strong>B.</strong> Use AWS site-to-site VPN to establish a connection between the data center and AWS Cloud</label><br>
<label for="q37-c"><input type="radio" id="q37-c" name="q37" value="C"> <strong>C.</strong> Use AWS Direct Connect plus virtual private network (VPN) to establish a connection between the data center and AWS Cloud</label><br>
<label for="q37-d"><input type="radio" id="q37-d" name="q37" value="D"> <strong>D.</strong> Use AWS Transit Gateway to establish a connection between the data center and AWS Cloud</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use AWS Direct Connect plus virtual private network (VPN) to establish a connection between the data center and AWS Cloud

</details>

---

## Câu 38

**Chủ đề:** Design Secure Architectures

One of the biggest football leagues in Europe has granted the distribution rights for live streaming its matches in the USA to a silicon valley based streaming services company. As per the terms of distribution, the company must make sure that only users from the USA are able to live stream the matches on their platform. Users from other countries in the world must be denied access to these live-streamed matches.

Which of the following options would allow the company to enforce these streaming restrictions? (Select two)

**Lựa chọn:**

<label for="q38-a"><input type="checkbox" id="q38-a" name="q38" value="A"> <strong>A.</strong> Use Amazon Route 53 based latency-based routing policy to restrict distribution of content to only the locations in which you have distribution rights</label><br>
<label for="q38-b"><input type="checkbox" id="q38-b" name="q38" value="B"> <strong>B.</strong> Use Amazon Route 53 based weighted routing policy to restrict distribution of content to only the locations in which you have distribution rights</label><br>
<label for="q38-c"><input type="checkbox" id="q38-c" name="q38" value="C"> <strong>C.</strong> Use Amazon Route 53 based failover routing policy to restrict distribution of content to only the locations in which you have distribution rights</label><br>
<label for="q38-d"><input type="checkbox" id="q38-d" name="q38" value="D"> <strong>D.</strong> Use Amazon Route 53 based geolocation routing policy to restrict distribution of content to only the locations in which you have distribution rights</label><br>
<label for="q38-e"><input type="checkbox" id="q38-e" name="q38" value="E"> <strong>E.</strong> Use georestriction to prevent users in specific geographic locations from accessing content that you're distributing through a Amazon CloudFront web distribution</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon Route 53 based geolocation routing policy to restrict distribution of content to only the locations in which you have distribution rights

E. Use georestriction to prevent users in specific geographic locations from accessing content that you're distributing through a Amazon CloudFront web distribution

</details>

---

## Câu 39

**Chủ đề:** Design Secure Architectures

A biotech research company needs to perform data analytics on real-time lab results provided by a partner organization. The partner stores these lab results in an Amazon RDS for MySQL instance within the partner’s own AWS account. The research company has a private VPC that does not have internet access, Direct Connect, or a VPN connection. However, the company must establish secure and private connectivity to the RDS database in the partner’s VPC. The solution must allow the research company to connect from its VPC while minimizing complexity and complying with data security requirements.

Which solution will meet these requirements?

**Lựa chọn:**

<label for="q39-a"><input type="radio" id="q39-a" name="q39" value="A"> <strong>A.</strong> Instruct the partner to enable public access on the Amazon RDS instance and add a security group rule to allow inbound access from the company’s IP range. The company accesses the database over the public internet through a NAT Gateway configured in a private subnet</label><br>
<label for="q39-b"><input type="radio" id="q39-b" name="q39" value="B"> <strong>B.</strong> Set up VPC peering between the company’s VPC and the partner’s VPC. Use AWS Transit Gateway in the partner's account to route traffic from the company’s VPC to the database. Modify the RDS subnet route tables to allow access from the company’s CIDR block</label><br>
<label for="q39-c"><input type="radio" id="q39-c" name="q39" value="C"> <strong>C.</strong> Configure a client VPN endpoint in the company’s account. Have researchers connect to the VPN from their local machines. Establish a Direct Connect gateway to the partner’s VPC and route RDS traffic via this connection</label><br>
<label for="q39-d"><input type="radio" id="q39-d" name="q39" value="D"> <strong>D.</strong> Instruct the partner to create a Network Load Balancer (NLB) in front of the Amazon RDS for MySQL instance. Use AWS PrivateLink to expose the NLB as an interface VPC endpoint in the research company’s VPC</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Instruct the partner to create a Network Load Balancer (NLB) in front of the Amazon RDS for MySQL instance. Use AWS PrivateLink to expose the NLB as an interface VPC endpoint in the research company’s VPC

</details>

---

## Câu 40

**Chủ đề:** Design High-Performing Architectures

A junior scientist working with the Deep Space Research Laboratory at NASA is trying to upload a high-resolution image of a nebula into Amazon S3. The image size is approximately 3 gigabytes. The junior scientist is using Amazon S3 Transfer Acceleration (Amazon S3TA) for faster image upload. It turns out that Amazon S3TA did not result in an accelerated transfer.

Given this scenario, which of the following is correct regarding the charges for this image transfer?

**Lựa chọn:**

<label for="q40-a"><input type="radio" id="q40-a" name="q40" value="A"> <strong>A.</strong> The junior scientist does not need to pay any transfer charges for the image upload</label><br>
<label for="q40-b"><input type="radio" id="q40-b" name="q40" value="B"> <strong>B.</strong> The junior scientist only needs to pay S3TA transfer charges for the image upload</label><br>
<label for="q40-c"><input type="radio" id="q40-c" name="q40" value="C"> <strong>C.</strong> The junior scientist only needs to pay Amazon S3 transfer charges for the image upload</label><br>
<label for="q40-d"><input type="radio" id="q40-d" name="q40" value="D"> <strong>D.</strong> The junior scientist needs to pay both S3 transfer charges and S3TA transfer charges for the image upload</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The junior scientist does not need to pay any transfer charges for the image upload

</details>

---

## Câu 41

**Chủ đề:** Design High-Performing Architectures

The solo founder at a tech startup has just created a brand new AWS account. The founder has provisioned an Amazon EC2 instance 1A which is running in AWS Region A. Later, he takes a snapshot of the instance 1A and then creates a new Amazon Machine Image (AMI) in Region A from this snapshot. This AMI is then copied into another Region B. The founder provisions an instance 1B in Region B using this new AMI in Region B.

At this point in time, what entities exist in Region B?

**Lựa chọn:**

<label for="q41-a"><input type="radio" id="q41-a" name="q41" value="A"> <strong>A.</strong> 1 Amazon EC2 instance, 1 AMI and 1 snapshot exist in Region B</label><br>
<label for="q41-b"><input type="radio" id="q41-b" name="q41" value="B"> <strong>B.</strong> 1 Amazon EC2 instance and 1 AMI exist in Region B</label><br>
<label for="q41-c"><input type="radio" id="q41-c" name="q41" value="C"> <strong>C.</strong> 1 Amazon EC2 instance and 1 snapshot exist in Region B</label><br>
<label for="q41-d"><input type="radio" id="q41-d" name="q41" value="D"> <strong>D.</strong> 1 Amazon EC2 instance and 2 AMIs exist in Region B</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. 1 Amazon EC2 instance, 1 AMI and 1 snapshot exist in Region B

</details>

---

## Câu 42

**Chủ đề:** Design High-Performing Architectures

The sourcing team at the US headquarters of a global e-commerce company is preparing a spreadsheet of the new product catalog. The spreadsheet is saved on an Amazon Elastic File System (Amazon EFS) created in us-east-1 region. The sourcing team counterparts from other AWS regions such as Asia Pacific and Europe also want to collaborate on this spreadsheet.

As a solutions architect, what is your recommendation to enable this collaboration with the LEAST amount of operational overhead?

**Lựa chọn:**

<label for="q42-a"><input type="radio" id="q42-a" name="q42" value="A"> <strong>A.</strong> The spreadsheet on the Amazon Elastic File System (Amazon EFS) can be accessed in other AWS regions by using an inter-region VPC peering connection</label><br>
<label for="q42-b"><input type="radio" id="q42-b" name="q42" value="B"> <strong>B.</strong> The spreadsheet will have to be copied into Amazon EFS file systems of other AWS regions as Amazon EFS is a regional service and it does not allow access from other AWS regions</label><br>
<label for="q42-c"><input type="radio" id="q42-c" name="q42" value="C"> <strong>C.</strong> The spreadsheet will have to be copied in Amazon S3 which can then be accessed from any AWS region</label><br>
<label for="q42-d"><input type="radio" id="q42-d" name="q42" value="D"> <strong>D.</strong> The spreadsheet data will have to be moved into an Amazon RDS for MySQL database which can then be accessed from any AWS region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The spreadsheet on the Amazon Elastic File System (Amazon EFS) can be accessed in other AWS regions by using an inter-region VPC peering connection

</details>

---

## Câu 43

**Chủ đề:** Design High-Performing Architectures

A research group runs its flagship application on a fleet of Amazon EC2 instances for a specialized task that must deliver high random I/O performance. Each instance in the fleet would have access to a dataset that is replicated across the instances by the application itself. Because of the resilient application architecture, the specialized task would continue to be processed even if any instance goes down, as the underlying application would ensure the replacement instance has access to the required dataset.

Which of the following options is the MOST cost-optimal and resource-efficient solution to build this fleet of Amazon EC2 instances?

**Lựa chọn:**

<label for="q43-a"><input type="radio" id="q43-a" name="q43" value="A"> <strong>A.</strong> Use Amazon Elastic Block Store (Amazon EBS) based EC2 instances</label><br>
<label for="q43-b"><input type="radio" id="q43-b" name="q43" value="B"> <strong>B.</strong> Use Amazon EC2 instances with Amazon EFS mount points</label><br>
<label for="q43-c"><input type="radio" id="q43-c" name="q43" value="C"> <strong>C.</strong> Use Instance Store based Amazon EC2 instances</label><br>
<label for="q43-d"><input type="radio" id="q43-d" name="q43" value="D"> <strong>D.</strong> Use Amazon EC2 instances with access to Amazon S3 based storage</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Instance Store based Amazon EC2 instances

</details>

---

## Câu 44

**Chủ đề:** Design High-Performing Architectures

A software engineering intern at an e-commerce company is documenting the process flow to provision Amazon EC2 instances via the Amazon EC2 API. These instances are to be used for an internal application that processes Human Resources payroll data. He wants to highlight those volume types that cannot be used as a boot volume.

Can you help the intern by identifying those storage volume types that CANNOT be used as boot volumes while creating the instances? (Select two)

**Lựa chọn:**

<label for="q44-a"><input type="checkbox" id="q44-a" name="q44" value="A"> <strong>A.</strong> General Purpose Solid State Drive (gp2)</label><br>
<label for="q44-b"><input type="checkbox" id="q44-b" name="q44" value="B"> <strong>B.</strong> Throughput Optimized Hard disk drive (st1)</label><br>
<label for="q44-c"><input type="checkbox" id="q44-c" name="q44" value="C"> <strong>C.</strong> Provisioned IOPS Solid state drive (io1)</label><br>
<label for="q44-d"><input type="checkbox" id="q44-d" name="q44" value="D"> <strong>D.</strong> Instance Store</label><br>
<label for="q44-e"><input type="checkbox" id="q44-e" name="q44" value="E"> <strong>E.</strong> Cold Hard disk drive (sc1)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Throughput Optimized Hard disk drive (st1)

E. Cold Hard disk drive (sc1)

</details>

---

## Câu 45

**Chủ đề:** Design Resilient Architectures

The payroll department at a company initiates several computationally intensive workloads on Amazon EC2 instances at a designated hour on the last day of every month. The payroll department has noticed a trend of severe performance lag during this hour. The engineering team has figured out a solution by using Auto Scaling Group for these Amazon EC2 instances and making sure that 10 Amazon EC2 instances are available during this peak usage hour. For normal operations only 2 Amazon EC2 instances are enough to cater to the workload.

As a solutions architect, which of the following steps would you recommend to implement the solution?

**Lựa chọn:**

<label for="q45-a"><input type="radio" id="q45-a" name="q45" value="A"> <strong>A.</strong> Configure your Auto Scaling group by creating a scheduled action that kicks-off at the designated hour on the last day of the month. Set the min count as well as the max count of instances to 10. This causes the scale-out to happen before peak traffic kicks in at the designated hour</label><br>
<label for="q45-b"><input type="radio" id="q45-b" name="q45" value="B"> <strong>B.</strong> Configure your Auto Scaling group by creating a scheduled action that kicks-off at the designated hour on the last day of the month. Set the desired capacity of instances to 10. This causes the scale-out to happen before peak traffic kicks in at the designated hour</label><br>
<label for="q45-c"><input type="radio" id="q45-c" name="q45" value="C"> <strong>C.</strong> Configure your Auto Scaling group by creating a target tracking policy and setting the instance count to 10 at the designated hour. This causes the scale-out to happen before peak traffic kicks in at the designated hour</label><br>
<label for="q45-d"><input type="radio" id="q45-d" name="q45" value="D"> <strong>D.</strong> Configure your Auto Scaling group by creating a simple tracking policy and setting the instance count to 10 at the designated hour. This causes the scale-out to happen before peak traffic kicks in at the designated hour</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure your Auto Scaling group by creating a scheduled action that kicks-off at the designated hour on the last day of the month. Set the desired capacity of instances to 10. This causes the scale-out to happen before peak traffic kicks in at the designated hour

</details>

---

## Câu 46

**Chủ đề:** Design Cost-Optimized Architectures

A technology blogger wants to write a review on the comparative pricing for various storage types available on AWS Cloud. The blogger has created a test file of size 1 gigabytes with some random data. Next he copies this test file into AWS S3 Standard storage class, provisions an Amazon EBS volume (General Purpose SSD (gp2)) with 100 gigabytes of provisioned storage and copies the test file into the Amazon EBS volume, and lastly copies the test file into an Amazon EFS Standard Storage filesystem. At the end of the month, he analyses the bill for costs incurred on the respective storage types for the test file.

What is the correct order of the storage charges incurred for the test file on these three storage types?

**Lựa chọn:**

<label for="q46-a"><input type="radio" id="q46-a" name="q46" value="A"> <strong>A.</strong> Cost of test file storage on Amazon S3 Standard < Cost of test file storage on Amazon EBS < Cost of test file storage on Amazon EFS</label><br>
<label for="q46-b"><input type="radio" id="q46-b" name="q46" value="B"> <strong>B.</strong> Cost of test file storage on Amazon S3 Standard < Cost of test file storage on Amazon EFS < Cost of test file storage on Amazon EBS</label><br>
<label for="q46-c"><input type="radio" id="q46-c" name="q46" value="C"> <strong>C.</strong> Cost of test file storage on Amazon EFS < Cost of test file storage on Amazon S3 Standard < Cost of test file storage on Amazon EBS</label><br>
<label for="q46-d"><input type="radio" id="q46-d" name="q46" value="D"> <strong>D.</strong> Cost of test file storage on Amazon EBS < Cost of test file storage on Amazon S3 Standard < Cost of test file storage on Amazon EFS</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Cost of test file storage on Amazon S3 Standard < Cost of test file storage on Amazon EFS < Cost of test file storage on Amazon EBS

</details>

---

## Câu 47

**Chủ đề:** Design High-Performing Architectures

A retail company runs a customer management system backed by a Microsoft SQL Server database. The system is tightly integrated with applications that rely on T-SQL queries. The company wants to modernize its infrastructure by migrating to Amazon Aurora PostgreSQL, but it needs to avoid major modifications to the existing application logic.

Which combination of actions should the company take to achieve this goal with minimal application refactoring? (Select two)

**Lựa chọn:**

<label for="q47-a"><input type="checkbox" id="q47-a" name="q47" value="A"> <strong>A.</strong> Configure Amazon Aurora PostgreSQL with a custom endpoint that emulates Microsoft SQL Server behavior</label><br>
<label for="q47-b"><input type="checkbox" id="q47-b" name="q47" value="B"> <strong>B.</strong> Use Amazon Aurora Global Database to replicate data across regions for compatibility</label><br>
<label for="q47-c"><input type="checkbox" id="q47-c" name="q47" value="C"> <strong>C.</strong> Deploy Babelfish for Aurora PostgreSQL to enable support for T-SQL commands</label><br>
<label for="q47-d"><input type="checkbox" id="q47-d" name="q47" value="D"> <strong>D.</strong> Use AWS Schema Conversion Tool (AWS SCT) along with AWS Database Migration Service (AWS DMS) to migrate the schema and data</label><br>
<label for="q47-e"><input type="checkbox" id="q47-e" name="q47" value="E"> <strong>E.</strong> Use AWS Glue to convert T-SQL queries to PostgreSQL-compatible SQL during the migration</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Deploy Babelfish for Aurora PostgreSQL to enable support for T-SQL commands

D. Use AWS Schema Conversion Tool (AWS SCT) along with AWS Database Migration Service (AWS DMS) to migrate the schema and data

</details>

---

## Câu 48

**Chủ đề:** Design Resilient Architectures

The development team at an e-commerce startup has set up multiple microservices running on Amazon EC2 instances under an Application Load Balancer. The team wants to route traffic to multiple back-end services based on the URL path of the HTTP header. So it wants requests for https://www.example.com/orders to go to a specific microservice and requests for https://www.example.com/products to go to another microservice.

Which of the following features of Application Load Balancers can be used for this use-case?

**Lựa chọn:**

<label for="q48-a"><input type="radio" id="q48-a" name="q48" value="A"> <strong>A.</strong> Query string parameter-based routing</label><br>
<label for="q48-b"><input type="radio" id="q48-b" name="q48" value="B"> <strong>B.</strong> HTTP header-based routing</label><br>
<label for="q48-c"><input type="radio" id="q48-c" name="q48" value="C"> <strong>C.</strong> Host-based Routing</label><br>
<label for="q48-d"><input type="radio" id="q48-d" name="q48" value="D"> <strong>D.</strong> Path-based Routing</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Path-based Routing

</details>

---

## Câu 49

**Chủ đề:** Design High-Performing Architectures

The product team at a startup has figured out a market need to support both stateful and stateless client-server communications via the application programming interface (APIs) developed using its platform. You have been hired by the startup as a solutions architect to build a solution to fulfill this market need using Amazon API Gateway.

Which of the following would you identify as correct?

**Lựa chọn:**

<label for="q49-a"><input type="radio" id="q49-a" name="q49" value="A"> <strong>A.</strong> Amazon API Gateway creates RESTful APIs that enable stateless client-server communication and Amazon API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server</label><br>
<label for="q49-b"><input type="radio" id="q49-b" name="q49" value="B"> <strong>B.</strong> Amazon API Gateway creates RESTful APIs that enable stateful client-server communication and Amazon API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server</label><br>
<label for="q49-c"><input type="radio" id="q49-c" name="q49" value="C"> <strong>C.</strong> Amazon API Gateway creates RESTful APIs that enable stateless client-server communication and Amazon API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateless, full-duplex communication between client and server</label><br>
<label for="q49-d"><input type="radio" id="q49-d" name="q49" value="D"> <strong>D.</strong> Amazon API Gateway creates RESTful APIs that enable stateful client-server communication and Amazon API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateless, full-duplex communication between client and server</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon API Gateway creates RESTful APIs that enable stateless client-server communication and Amazon API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server

</details>

---

## Câu 50

**Chủ đề:** Design Resilient Architectures

The engineering team at a Spanish professional football club has built a notification system for its website using Amazon Simple Notification Service (Amazon SNS) notifications which are then handled by an AWS Lambda function for end-user delivery. During the off-season, the notification systems need to handle about 100 requests per second. During the peak football season, the rate touches about 5000 requests per second and it is noticed that a significant number of the notifications are not being delivered to the end-users on the website.

As a solutions architect, which of the following would you suggest as the BEST possible solution to this issue?

**Lựa chọn:**

<label for="q50-a"><input type="radio" id="q50-a" name="q50" value="A"> <strong>A.</strong> Amazon SNS has hit a scalability limit, so the team needs to contact AWS support to raise the account limit</label><br>
<label for="q50-b"><input type="radio" id="q50-b" name="q50" value="B"> <strong>B.</strong> Amazon SNS message deliveries to AWS Lambda have crossed the account concurrency quota for AWS Lambda, so the team needs to contact AWS support to raise the account limit</label><br>
<label for="q50-c"><input type="radio" id="q50-c" name="q50" value="C"> <strong>C.</strong> The engineering team needs to provision more servers running the Amazon SNS service</label><br>
<label for="q50-d"><input type="radio" id="q50-d" name="q50" value="D"> <strong>D.</strong> The engineering team needs to provision more servers running the AWS Lambda service</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Amazon SNS message deliveries to AWS Lambda have crossed the account concurrency quota for AWS Lambda, so the team needs to contact AWS support to raise the account limit

</details>

---

## Câu 51

**Chủ đề:** Design High-Performing Architectures

A file-hosting service uses Amazon Simple Storage Service (Amazon S3) under the hood to power its storage offerings. Currently all the customer files are uploaded directly under a single Amazon S3 bucket. The engineering team has started seeing scalability issues where customer file uploads have started failing during the peak access hours with more than 5000 requests per second.

Which of the following is the MOST resource efficient and cost-optimal way of addressing this issue?

**Lựa chọn:**

<label for="q51-a"><input type="radio" id="q51-a" name="q51" value="A"> <strong>A.</strong> Change the application architecture to create a new Amazon S3 bucket for each customer and then upload each customer's files directly under the respective buckets</label><br>
<label for="q51-b"><input type="radio" id="q51-b" name="q51" value="B"> <strong>B.</strong> Change the application architecture to create a new Amazon S3 bucket for each day's data and then upload the daily files directly under that day's bucket</label><br>
<label for="q51-c"><input type="radio" id="q51-c" name="q51" value="C"> <strong>C.</strong> Change the application architecture to use Amazon Elastic File System (Amazon EFS) instead of Amazon S3 for storing the customers' uploaded files</label><br>
<label for="q51-d"><input type="radio" id="q51-d" name="q51" value="D"> <strong>D.</strong> Change the application architecture to create customer-specific custom prefixes within the single Amazon S3 bucket and then upload the daily files into those prefixed locations</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Change the application architecture to create customer-specific custom prefixes within the single Amazon S3 bucket and then upload the daily files into those prefixed locations

</details>

---

## Câu 52

**Chủ đề:** Design Resilient Architectures

A new DevOps engineer has just joined a development team and wants to understand the replication capabilities for Amazon RDS Multi-AZ deployment as well as Amazon RDS Read-replicas.

Which of the following correctly summarizes these capabilities for the given database?

**Lựa chọn:**

<label for="q52-a"><input type="radio" id="q52-a" name="q52" value="A"> <strong>A.</strong> Multi-AZ follows asynchronous replication and spans one Availability Zone (AZ) within a single region. Read replicas follow synchronous replication and can be within an Availability Zone (AZ), Cross-AZ, or Cross-Region</label><br>
<label for="q52-b"><input type="radio" id="q52-b" name="q52" value="B"> <strong>B.</strong> Multi-AZ follows synchronous replication and spans at least two Availability Zones (AZs) within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone (AZ), Cross-AZ, or Cross-Region</label><br>
<label for="q52-c"><input type="radio" id="q52-c" name="q52" value="C"> <strong>C.</strong> Multi-AZ follows asynchronous replication and spans at least two Availability Zones (AZs) within a single region. Read replicas follow synchronous replication and can be within an Availability Zone (AZ), Cross-AZ, or Cross-Region</label><br>
<label for="q52-d"><input type="radio" id="q52-d" name="q52" value="D"> <strong>D.</strong> Multi-AZ follows asynchronous replication and spans at least two Availability Zones (AZs) within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone (AZ), Cross-AZ, or Cross-Region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Multi-AZ follows synchronous replication and spans at least two Availability Zones (AZs) within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone (AZ), Cross-AZ, or Cross-Region

</details>

---

## Câu 53

**Chủ đề:** Design Resilient Architectures

A healthcare analytics company centralizes clinical and operational datasets in an Amazon S3–based data lake. Incoming data is ingested in Apache Parquet format from multiple hospitals and wearable health devices. To ensure quality and standardization, the company applies several transformation steps: anomaly filtering, datetime normalization, and aggregation by patient cohort. The company needs a solution to support a code-free interface that enables data engineers and business analysts to collaborate on data preparation workflows. The company also requires data lineage tracking, data profiling capabilities, and an easy way to share transformation logic across teams without writing or managing code.

Which AWS solution best meets these requirements?

**Lựa chọn:**

<label for="q53-a"><input type="radio" id="q53-a" name="q53" value="A"> <strong>A.</strong> Use Amazon AppFlow to move and transform Parquet files in S3. Configure AppFlow transformations and mappings within the visual interface. Share flows with collaborators through AWS IAM policies and scheduled executions</label><br>
<label for="q53-b"><input type="radio" id="q53-b" name="q53" value="B"> <strong>B.</strong> Create Amazon Athena SQL queries to perform transformation steps directly on S3. Store queries in AWS Glue Data Catalog and share saved queries with other users through Amazon Athena's query editor</label><br>
<label for="q53-c"><input type="radio" id="q53-c" name="q53" value="C"> <strong>C.</strong> Use AWS Glue Studio’s visual canvas to design data transformation workflows on top of the Parquet files in Amazon S3. Configure Glue Studio jobs to run these transformations without writing code. Share the job definitions with team members for reuse. Use the visual job editor to track transformation progress and inspect profiling statistics for each dataset column</label><br>
<label for="q53-d"><input type="radio" id="q53-d" name="q53" value="D"> <strong>D.</strong> Use AWS Glue DataBrew to visually build transformation workflows on top of the raw Parquet files in S3. Use DataBrew recipes to track, audit, and share the transformation steps with others. Enable data profiling to inspect column statistics, null values, and data types across datasets</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Glue DataBrew to visually build transformation workflows on top of the raw Parquet files in S3. Use DataBrew recipes to track, audit, and share the transformation steps with others. Enable data profiling to inspect column statistics, null values, and data types across datasets

</details>

---

## Câu 54

**Chủ đề:** Design High-Performing Architectures

The DevOps team at an e-commerce company has deployed a fleet of Amazon EC2 instances under an Auto Scaling group (ASG). The instances under the ASG span two Availability Zones (AZ) within the us-east-1 region. All the incoming requests are handled by an Application Load Balancer (ALB) that routes the requests to the Amazon EC2 instances under the Auto Scaling Group. As part of a test run, two instances (instance 1 and 2, belonging to AZ A) were manually terminated by the DevOps team causing the Availability Zones (AZ) to have unbalanced resources. Later that day, another instance (belonging to AZ B) was detected as unhealthy by the Application Load Balancer's health check.

Can you identify the correct outcomes for these events? (Select two)

**Lựa chọn:**

<label for="q54-a"><input type="checkbox" id="q54-a" name="q54" value="A"> <strong>A.</strong> As the resources are unbalanced in the Availability Zones, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling launches new instances before terminating the old ones, so that rebalancing does not compromise the performance or availability of your application</label><br>
<label for="q54-b"><input type="checkbox" id="q54-b" name="q54" value="B"> <strong>B.</strong> Amazon EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it. Later, another scaling activity launches a new instance to replace the terminated instance</label><br>
<label for="q54-c"><input type="checkbox" id="q54-c" name="q54" value="C"> <strong>C.</strong> Amazon EC2 Auto Scaling creates a new scaling activity for launching a new instance to replace the unhealthy instance. Later, Amazon EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it</label><br>
<label for="q54-d"><input type="checkbox" id="q54-d" name="q54" value="D"> <strong>D.</strong> As the resources are unbalanced in the Availability Zones, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling terminates old instances before launching new instances, so that rebalancing does not cause extra instances to be launched</label><br>
<label for="q54-e"><input type="checkbox" id="q54-e" name="q54" value="E"> <strong>E.</strong> Amazon EC2 Auto Scaling creates a new scaling activity to terminate the unhealthy instance and launch the new instance simultaneously</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. As the resources are unbalanced in the Availability Zones, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling launches new instances before terminating the old ones, so that rebalancing does not compromise the performance or availability of your application

B. Amazon EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it. Later, another scaling activity launches a new instance to replace the terminated instance

</details>

---

## Câu 55

**Chủ đề:** Design High-Performing Architectures

A digital event-ticketing platform hosts its core transaction-processing service on AWS. The service runs on Amazon EC2 instances and stores finalized transactions in an Amazon Aurora PostgreSQL database. During periods of high user activity - such as flash ticket sales or holiday promotions - the application begins timing out, causing failed or delayed purchases. A solutions architect has been asked to redesign the backend for scalability and cost-efficiency, without reengineering the database layer.

Which combination of actions will meet these goals in the most cost-effective and scalable manner? (Select two)

**Lựa chọn:**

<label for="q55-a"><input type="checkbox" id="q55-a" name="q55" value="A"> <strong>A.</strong> Implement Amazon RDS Proxy between the application and the Aurora PostgreSQL cluster. Deploy EC2 instances in an Auto Scaling group to retry transactions as needed</label><br>
<label for="q55-b"><input type="checkbox" id="q55-b" name="q55" value="B"> <strong>B.</strong> Modify the application to publish purchase events to an Amazon SQS queue. Launch an Auto Scaling group of EC2 workers that poll the queue and process purchases asynchronously</label><br>
<label for="q55-c"><input type="checkbox" id="q55-c" name="q55" value="C"> <strong>C.</strong> Use an Amazon ElastiCache cluster to cache database queries. Configure the application to store purchase transactions in the cache before writing to the database</label><br>
<label for="q55-d"><input type="checkbox" id="q55-d" name="q55" value="D"> <strong>D.</strong> Deploy an Amazon API Gateway with throttling and usage plans to slow down incoming purchase requests during peak times and maintain application stability</label><br>
<label for="q55-e"><input type="checkbox" id="q55-e" name="q55" value="E"> <strong>E.</strong> Deploy read replicas for the Aurora database in another Region and configure EC2 instances to read and write from the nearest replica based on latency</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Implement Amazon RDS Proxy between the application and the Aurora PostgreSQL cluster. Deploy EC2 instances in an Auto Scaling group to retry transactions as needed

B. Modify the application to publish purchase events to an Amazon SQS queue. Launch an Auto Scaling group of EC2 workers that poll the queue and process purchases asynchronously

</details>

---

## Câu 56

**Chủ đề:** Design Secure Architectures

A company uses Amazon S3 buckets for storing sensitive customer data. The company has defined different retention periods for different objects present in the Amazon S3 buckets, based on the compliance requirements. But, the retention rules do not seem to work as expected.

Which of the following options represent a valid configuration for setting up retention periods for objects in Amazon S3 buckets? (Select two)

**Lựa chọn:**

<label for="q56-a"><input type="checkbox" id="q56-a" name="q56" value="A"> <strong>A.</strong> When you apply a retention period to an object version explicitly, you specify a Retain Until Date for the object version</label><br>
<label for="q56-b"><input type="checkbox" id="q56-b" name="q56" value="B"> <strong>B.</strong> You cannot place a retention period on an object version through a bucket default setting</label><br>
<label for="q56-c"><input type="checkbox" id="q56-c" name="q56" value="C"> <strong>C.</strong> When you use bucket default settings, you specify a Retain Until Date for the object version</label><br>
<label for="q56-d"><input type="checkbox" id="q56-d" name="q56" value="D"> <strong>D.</strong> Different versions of a single object can have different retention modes and periods</label><br>
<label for="q56-e"><input type="checkbox" id="q56-e" name="q56" value="E"> <strong>E.</strong> The bucket default settings will override any explicit retention mode or period you request on an object version</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. When you apply a retention period to an object version explicitly, you specify a Retain Until Date for the object version

D. Different versions of a single object can have different retention modes and periods

</details>

---

## Câu 57

**Chủ đề:** Design High-Performing Architectures

A logistics company is building a multi-tier application to track the location of its trucks during peak operating hours. The company wants these data points to be accessible in real-time in its analytics platform via a REST API. The company has hired you as an AWS Certified Solutions Architect Associate to build a multi-tier solution to store and retrieve this location data for analysis.

Which of the following options addresses the given use case?

**Lựa chọn:**

<label for="q57-a"><input type="radio" id="q57-a" name="q57" value="A"> <strong>A.</strong> Leverage Amazon Athena with Amazon S3</label><br>
<label for="q57-b"><input type="radio" id="q57-b" name="q57" value="B"> <strong>B.</strong> Leverage Amazon QuickSight with Amazon Redshift</label><br>
<label for="q57-c"><input type="radio" id="q57-c" name="q57" value="C"> <strong>C.</strong> Leverage Amazon API Gateway with Amazon Kinesis Data Analytics</label><br>
<label for="q57-d"><input type="radio" id="q57-d" name="q57" value="D"> <strong>D.</strong> Leverage Amazon API Gateway with AWS Lambda</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Leverage Amazon API Gateway with Amazon Kinesis Data Analytics

</details>

---

## Câu 58

**Chủ đề:** Design Secure Architectures

A development team requires permissions to list an Amazon S3 bucket and delete objects from that bucket. A systems administrator has created the following IAM policy to provide access to the bucket and applied that policy to the group. The group is not able to delete objects in the bucket. The company follows the principle of least privilege.

    "Version": "2021-10-17",
    "Statement": [
        {
            "Action": [
                "s3:ListBucket",
                "s3:DeleteObject"
            ],
            "Resource": [
                "arn:aws:s3:::example-bucket"
            ],
            "Effect": "Allow"
        }
    ]

Which statement should a solutions architect add to the policy to address this issue?

**Lựa chọn:**

<label for="q58-a"><input type="radio" id="q58-a" name="q58" value="A"> <strong>A.</strong> {
    "Action": [
        "s3:*Object"
    ],
    "Resource": [
        "arn:aws:s3:::example-bucket/*"
    ],
    "Effect": "Allow"
}</label><br>
<label for="q58-b"><input type="radio" id="q58-b" name="q58" value="B"> <strong>B.</strong> {
    "Action": [
        "s3:DeleteObject"
    ],
    "Resource": [
        "arn:aws:s3:::example-bucket/*"
    ],
    "Effect": "Allow"
}</label><br>
<label for="q58-c"><input type="radio" id="q58-c" name="q58" value="C"> <strong>C.</strong> {
    "Action": [
        "s3:DeleteObject"
    ],
    "Resource": [
        "arn:aws:s3:::example-bucket*"
    ],
    "Effect": "Allow"
}</label><br>
<label for="q58-d"><input type="radio" id="q58-d" name="q58" value="D"> <strong>D.</strong> {
    "Action": [
        "s3:*"
    ],
    "Resource": [
        "arn:aws:s3:::example-bucket/*"
    ],
    "Effect": "Allow"
}</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. {
    "Action": [
        "s3:DeleteObject"
    ],
    "Resource": [
        "arn:aws:s3:::example-bucket/*"
    ],
    "Effect": "Allow"
}

</details>

---

## Câu 59

**Chủ đề:** Design High-Performing Architectures

A gaming company is looking at improving the availability and performance of its global flagship application which utilizes User Datagram Protocol and needs to support fast regional failover in case an AWS Region goes down. The company wants to continue using its own custom Domain Name System (DNS) service.

Which of the following AWS services represents the best solution for this use-case?

**Lựa chọn:**

<label for="q59-a"><input type="radio" id="q59-a" name="q59" value="A"> <strong>A.</strong> AWS Elastic Load Balancing (ELB)</label><br>
<label for="q59-b"><input type="radio" id="q59-b" name="q59" value="B"> <strong>B.</strong> AWS Global Accelerator</label><br>
<label for="q59-c"><input type="radio" id="q59-c" name="q59" value="C"> <strong>C.</strong> Amazon CloudFront</label><br>
<label for="q59-d"><input type="radio" id="q59-d" name="q59" value="D"> <strong>D.</strong> Amazon Route 53</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. AWS Global Accelerator

</details>

---

## Câu 60

**Chủ đề:** Design High-Performing Architectures

A gaming company is developing a mobile game that streams score updates to a backend processor and then publishes results on a leaderboard. The company has hired you as an AWS Certified Solutions Architect Associate to design a solution that can handle major traffic spikes, process the mobile game updates in the order of receipt, and store the processed updates in a highly available database. The company wants to minimize the management overhead required to maintain the solution.

Which of the following will you recommend to meet these requirements?

**Lựa chọn:**

<label for="q60-a"><input type="radio" id="q60-a" name="q60" value="A"> <strong>A.</strong> Push score updates to an Amazon Simple Queue Service (Amazon SQS) queue which uses a fleet of Amazon EC2 instances (with Auto Scaling) to process these updates in the Amazon SQS queue and then store these processed updates in an Amazon RDS MySQL database</label><br>
<label for="q60-b"><input type="radio" id="q60-b" name="q60" value="B"> <strong>B.</strong> Push score updates to Amazon Kinesis Data Streams which uses an AWS Lambda function to process these updates and then store these processed updates in Amazon DynamoDB</label><br>
<label for="q60-c"><input type="radio" id="q60-c" name="q60" value="C"> <strong>C.</strong> Push score updates to Amazon Kinesis Data Streams which uses a fleet of Amazon EC2 instances (with Auto Scaling) to process the updates in Amazon Kinesis Data Streams and then store these processed updates in Amazon DynamoDB</label><br>
<label for="q60-d"><input type="radio" id="q60-d" name="q60" value="D"> <strong>D.</strong> Push score updates to an Amazon Simple Notification Service (Amazon SNS) topic, subscribe an AWS Lambda function to this Amazon SNS topic to process the updates and then store these processed updates in a SQL database running on Amazon EC2 instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Push score updates to Amazon Kinesis Data Streams which uses an AWS Lambda function to process these updates and then store these processed updates in Amazon DynamoDB

</details>

---

## Câu 61

**Chủ đề:** Design Resilient Architectures

While consolidating logs for the weekly reporting, a development team at an e-commerce company noticed that an unusually large number of illegal AWS application programming interface (API) queries were made sometime during the week. Due to the off-season, there was no visible impact on the systems. However, this event led the management team to seek an automated solution that can trigger near-real-time warnings in case such an event recurs.

Which of the following represents the best solution for the given scenario?

**Lựa chọn:**

<label for="q61-a"><input type="radio" id="q61-a" name="q61" value="A"> <strong>A.</strong> Configure AWS CloudTrail to stream event data to Amazon Kinesis. Use Amazon Kinesis stream-level metrics in the Amazon CloudWatch to trigger an AWS Lambda function that will trigger an error workflow</label><br>
<label for="q61-b"><input type="radio" id="q61-b" name="q61" value="B"> <strong>B.</strong> Run Amazon Athena SQL queries against AWS CloudTrail log files stored in Amazon S3 buckets. Use Amazon QuickSight to generate reports for managerial dashboards</label><br>
<label for="q61-c"><input type="radio" id="q61-c" name="q61" value="C"> <strong>C.</strong> AWS Trusted Advisor publishes metrics about check results to Amazon CloudWatch. Create an alarm to track status changes for checks in the Service Limits category for the APIs. The alarm will then notify when the service quota is reached or exceeded</label><br>
<label for="q61-d"><input type="radio" id="q61-d" name="q61" value="D"> <strong>D.</strong> Create an Amazon CloudWatch metric filter that processes AWS CloudTrail logs having API call details and looks at any errors by factoring in all the error codes that need to be tracked. Create an alarm based on this metric's rate to send an Amazon SNS notification to the required team</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Create an Amazon CloudWatch metric filter that processes AWS CloudTrail logs having API call details and looks at any errors by factoring in all the error codes that need to be tracked. Create an alarm based on this metric's rate to send an Amazon SNS notification to the required team

</details>

---

## Câu 62

**Chủ đề:** Design High-Performing Architectures

A retail company's dynamic website is hosted using on-premises servers in its data center in the United States. The company is launching its website in Asia, and it wants to optimize the website loading times for new users in Asia. The website's backend must remain in the United States. The website is being launched in a few days, and an immediate solution is needed.

What would you recommend?

**Lựa chọn:**

<label for="q62-a"><input type="radio" id="q62-a" name="q62" value="A"> <strong>A.</strong> Use Amazon CloudFront with a custom origin pointing to the DNS record of the website on Amazon Route 53</label><br>
<label for="q62-b"><input type="radio" id="q62-b" name="q62" value="B"> <strong>B.</strong> Use Amazon CloudFront with a custom origin pointing to the on-premises servers</label><br>
<label for="q62-c"><input type="radio" id="q62-c" name="q62" value="C"> <strong>C.</strong> Migrate the website to Amazon S3. Use S3 cross-region replication (S3 CRR) between AWS Regions in the US and Asia</label><br>
<label for="q62-d"><input type="radio" id="q62-d" name="q62" value="D"> <strong>D.</strong> Leverage a Amazon Route 53 geo-proximity routing policy pointing to on-premises servers</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon CloudFront with a custom origin pointing to the on-premises servers

</details>

---

## Câu 63

**Chủ đề:** Design Secure Architectures

A healthcare company is developing a secure internal web portal hosted on AWS. The application must communicate with legacy systems that reside in the company's on-premises data centers. These data centers are connected to AWS via a site-to-site VPN. The company uses Amazon Route 53 as its DNS solution and requires the application to resolve private DNS records for the on-premises services from within its Amazon VPC.

What is the MOST secure and appropriate way to meet these DNS resolution requirements?

**Lựa chọn:**

<label for="q63-a"><input type="radio" id="q63-a" name="q63" value="A"> <strong>A.</strong> Create a Route 53 Resolver outbound endpoint. Define a forwarding rule that routes DNS queries for on-premises domains to the on-premises DNS server. Associate the rule with the VPC</label><br>
<label for="q63-b"><input type="radio" id="q63-b" name="q63" value="B"> <strong>B.</strong> Configure a Route 53 Resolver inbound endpoint and create a DNS forwarding rule. Enable recursive DNS resolution in the VPC to access on-premises services</label><br>
<label for="q63-c"><input type="radio" id="q63-c" name="q63" value="C"> <strong>C.</strong> Create a hybrid connectivity gateway and attach the on-premises DNS servers to Route 53 as authoritative zones for internal domains</label><br>
<label for="q63-d"><input type="radio" id="q63-d" name="q63" value="D"> <strong>D.</strong> Create a Route 53 private hosted zone for the on-premises domain. Associate the hosted zone with the VPC to allow the application to resolve DNS names of the on-premises services</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a Route 53 Resolver outbound endpoint. Define a forwarding rule that routes DNS queries for on-premises domains to the on-premises DNS server. Associate the rule with the VPC

</details>

---

## Câu 64

**Chủ đề:** Design High-Performing Architectures

A data analytics company measures what the consumers watch and what advertising they’re exposed to. This real-time data is ingested into its on-premises data center and subsequently, the daily data feed is compressed into a single file and uploaded on Amazon S3 for backup. The typical compressed file size is around 2 gigabytes.

Which of the following is the fastest way to upload the daily compressed file into Amazon S3?

**Lựa chọn:**

<label for="q64-a"><input type="radio" id="q64-a" name="q64" value="A"> <strong>A.</strong> Upload the compressed file in a single operation</label><br>
<label for="q64-b"><input type="radio" id="q64-b" name="q64" value="B"> <strong>B.</strong> Upload the compressed file using multipart upload</label><br>
<label for="q64-c"><input type="radio" id="q64-c" name="q64" value="C"> <strong>C.</strong> FTP the compressed file into an Amazon EC2 instance that runs in the same region as the Amazon S3 bucket. Then transfer the file from the Amazon EC2 instance into the Amazon S3 bucket</label><br>
<label for="q64-d"><input type="radio" id="q64-d" name="q64" value="D"> <strong>D.</strong> Upload the compressed file using multipart upload with Amazon S3 Transfer Acceleration (Amazon S3TA)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Upload the compressed file using multipart upload with Amazon S3 Transfer Acceleration (Amazon S3TA)

</details>

---

## Câu 65

**Chủ đề:** Design High-Performing Architectures

A large financial institution operates an on-premises data center with hundreds of petabytes of data managed on Microsoft’s Distributed File System (DFS). The CTO wants the organization to transition into a hybrid cloud environment and run data-intensive analytics workloads that support DFS.

Which of the following AWS services can facilitate the migration of these workloads?

**Lựa chọn:**

<label for="q65-a"><input type="radio" id="q65-a" name="q65" value="A"> <strong>A.</strong> Amazon FSx for Windows File Server</label><br>
<label for="q65-b"><input type="radio" id="q65-b" name="q65" value="B"> <strong>B.</strong> Microsoft SQL Server on AWS</label><br>
<label for="q65-c"><input type="radio" id="q65-c" name="q65" value="C"> <strong>C.</strong> Amazon FSx for Lustre</label><br>
<label for="q65-d"><input type="radio" id="q65-d" name="q65" value="D"> <strong>D.</strong> AWS Directory Service for Microsoft Active Directory (AWS Managed Microsoft AD)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon FSx for Windows File Server

</details>

---

## Câu 66

**Chủ đề:** Design Resilient Architectures

A financial services company runs a Kubernetes-based microservices application in its on-premises data center. The application uses the Advanced Message Queuing Protocol (AMQP) to interact with a message queue. The company is experiencing rapid growth and its on-prem infrastructure cannot scale fast enough. The company wants to migrate the application to AWS with minimal code changes and reduce infrastructure management overhead. The messaging component must continue using AMQP, and the solution should offer high scalability and low operational effort.

Which combination of options will together meet these requirements? (Select two)

**Lựa chọn:**

<label for="q66-a"><input type="checkbox" id="q66-a" name="q66" value="A"> <strong>A.</strong> Deploy the containerized application to Amazon Elastic Kubernetes Service (Amazon EKS) using AWS Fargate to avoid managing EC2 nodes</label><br>
<label for="q66-b"><input type="checkbox" id="q66-b" name="q66" value="B"> <strong>B.</strong> Use Amazon Simple Queue Service (Amazon SQS) as the replacement for the AMQP message broker. Refactor the application to use SQS SDKs and polling logic</label><br>
<label for="q66-c"><input type="checkbox" id="q66-c" name="q66" value="C"> <strong>C.</strong> Replace the current messaging system with Amazon MQ, a fully managed broker that supports AMQP natively. Integrate the application with the Amazon MQ endpoint without modifying the existing message format</label><br>
<label for="q66-d"><input type="checkbox" id="q66-d" name="q66" value="D"> <strong>D.</strong> Deploy the application to Amazon ECS on EC2, and integrate the messaging workflow using Amazon SNS for asynchronous pub/sub delivery</label><br>
<label for="q66-e"><input type="checkbox" id="q66-e" name="q66" value="E"> <strong>E.</strong> Run the application on Amazon EC2 Auto Scaling groups and use a self-hosted RabbitMQ instance on EC2 to preserve AMQP compatibility</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy the containerized application to Amazon Elastic Kubernetes Service (Amazon EKS) using AWS Fargate to avoid managing EC2 nodes

C. Replace the current messaging system with Amazon MQ, a fully managed broker that supports AMQP natively. Integrate the application with the Amazon MQ endpoint without modifying the existing message format

</details>

---

## Câu 67

**Chủ đề:** Design High-Performing Architectures

A Hollywood studio is planning a series of promotional events leading up to the launch of the trailer of its next sci-fi thriller. The executives at the studio want to create a static website with lots of animations in line with the theme of the movie. The studio has hired you as a solutions architect to build a scalable serverless solution.

Which of the following represents the MOST cost-optimal and high-performance solution?

**Lựa chọn:**

<label for="q67-a"><input type="radio" id="q67-a" name="q67" value="A"> <strong>A.</strong> Build the website as a static website hosted on Amazon S3. Create an Amazon CloudFront distribution with Amazon S3 as the origin. Use Amazon Route 53 to create an alias record that points to your Amazon CloudFront distribution</label><br>
<label for="q67-b"><input type="radio" id="q67-b" name="q67" value="B"> <strong>B.</strong> Host the website on an Amazon EC2 instance. Create a Amazon CloudFront distribution with the Amazon EC2 instance as the custom origin</label><br>
<label for="q67-c"><input type="radio" id="q67-c" name="q67" value="C"> <strong>C.</strong> Host the website on an instance in the studio's on-premises data center. Create an Amazon CloudFront distribution with this instance as the custom origin</label><br>
<label for="q67-d"><input type="radio" id="q67-d" name="q67" value="D"> <strong>D.</strong> Host the website on AWS Lambda. Create an Amazon CloudFront distribution with Lambda as the origin</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Build the website as a static website hosted on Amazon S3. Create an Amazon CloudFront distribution with Amazon S3 as the origin. Use Amazon Route 53 to create an alias record that points to your Amazon CloudFront distribution

</details>

---

## Câu 68

**Chủ đề:** Design Secure Architectures

A social photo-sharing web application is hosted on Amazon Elastic Compute Cloud (Amazon EC2) instances behind an Elastic Load Balancer. The app gives the users the ability to upload their photos and also shows a leaderboard on the homepage of the app. The uploaded photos are stored in Amazon Simple Storage Service (Amazon S3) and the leaderboard data is maintained in Amazon DynamoDB. The Amazon EC2 instances need to access both Amazon S3 and Amazon DynamoDB for these features.

As a solutions architect, which of the following solutions would you recommend as the MOST secure option?

**Lựa chọn:**

<label for="q68-a"><input type="radio" id="q68-a" name="q68" value="A"> <strong>A.</strong> Attach the appropriate IAM role to the Amazon EC2 instance profile so that the instance can access Amazon S3 and Amazon DynamoDB</label><br>
<label for="q68-b"><input type="radio" id="q68-b" name="q68" value="B"> <strong>B.</strong> Save the AWS credentials (access key Id and secret access token) in a configuration file within the application code on the Amazon EC2 instances. Amazon EC2 instances can use these credentials to access Amazon S3 and Amazon DynamoDB</label><br>
<label for="q68-c"><input type="radio" id="q68-c" name="q68" value="C"> <strong>C.</strong> Configure AWS CLI on the Amazon EC2 instances using a valid IAM user's credentials. The application code can then invoke shell scripts to access Amazon S3 and Amazon DynamoDB via AWS CLI</label><br>
<label for="q68-d"><input type="radio" id="q68-d" name="q68" value="D"> <strong>D.</strong> Encrypt the AWS credentials via a custom encryption library and save it in a secret directory on the Amazon EC2 instances. The application code can then safely decrypt the AWS credentials to make the API calls to Amazon S3 and Amazon DynamoDB</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Attach the appropriate IAM role to the Amazon EC2 instance profile so that the instance can access Amazon S3 and Amazon DynamoDB

</details>

---

## Câu 69

**Chủ đề:** Design Secure Architectures

A multinational logistics company is migrating its core systems to AWS. As part of this migration, the company has built an Amazon S3–based data lake to ingest and analyze supply chain data from external carriers and vendors. While some vendors have adopted the company’s modern REST-based APIs for S3 uploads, others operate legacy systems that rely exclusively on SFTP for file transfers. These vendors are unable or unwilling to modify their workflows to support S3 APIs. The company wants to provide these vendors with an SFTP-compatible solution that allows direct uploads to Amazon S3, and must use fully managed AWS services to avoid managing any infrastructure. It must also support identity federation so that internal teams can map vendor access securely to specific S3 buckets or prefixes.

Which combination of options will provide a scalable and low-maintenance solution for this use case? (Select two)

**Lựa chọn:**

<label for="q69-a"><input type="checkbox" id="q69-a" name="q69" value="A"> <strong>A.</strong> Deploy a fully managed AWS Transfer Family endpoint with SFTP enabled. Configure it to store uploaded files directly in an Amazon S3 bucket. Set up IAM roles mapped to each vendor for secure bucket or prefix access</label><br>
<label for="q69-b"><input type="checkbox" id="q69-b" name="q69" value="B"> <strong>B.</strong> Set up an Amazon EC2 instance with a custom SFTP server using OpenSSH. Configure cron jobs to upload received files to S3. Use Amazon CloudWatch to monitor EC2 health and disk usage</label><br>
<label for="q69-c"><input type="checkbox" id="q69-c" name="q69" value="C"> <strong>C.</strong> Configure Amazon S3 bucket policies to use IAM role-based access control for each vendor. Combine this with Transfer Family identity provider integration using Amazon Cognito or a custom identity provider for fine-grained permissions</label><br>
<label for="q69-d"><input type="checkbox" id="q69-d" name="q69" value="D"> <strong>D.</strong> Use AWS Transfer Family with SFTP for file uploads. Integrate the SFTP access control with Amazon Route 53 private hosted zones to create vendor-specific upload subdomains pointing to the SFTP endpoint</label><br>
<label for="q69-e"><input type="checkbox" id="q69-e" name="q69" value="E"> <strong>E.</strong> Use Amazon AppFlow to extract data from the legacy vendor systems and transform it into S3-compliant uploads. Schedule batch sync jobs to trigger every hour and send logs to CloudWatch for audit purposes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy a fully managed AWS Transfer Family endpoint with SFTP enabled. Configure it to store uploaded files directly in an Amazon S3 bucket. Set up IAM roles mapped to each vendor for secure bucket or prefix access

C. Configure Amazon S3 bucket policies to use IAM role-based access control for each vendor. Combine this with Transfer Family identity provider integration using Amazon Cognito or a custom identity provider for fine-grained permissions

</details>

---

## Câu 70

**Chủ đề:** Design High-Performing Architectures

An IT company has an Access Control Management (ACM) application that uses Amazon RDS for MySQL but is running into performance issues despite using Read Replicas. The company has hired you as a solutions architect to address these performance-related challenges without moving away from the underlying relational database schema. The company has branch offices across the world, and it needs the solution to work on a global scale.

Which of the following will you recommend as the MOST cost-effective and high-performance solution?

**Lựa chọn:**

<label for="q70-a"><input type="radio" id="q70-a" name="q70" value="A"> <strong>A.</strong> Use Amazon Aurora Global Database to enable fast local reads with low latency in each region</label><br>
<label for="q70-b"><input type="radio" id="q70-b" name="q70" value="B"> <strong>B.</strong> Spin up Amazon EC2 instances in each AWS region, install MySQL databases and migrate the existing data into these new databases</label><br>
<label for="q70-c"><input type="radio" id="q70-c" name="q70" value="C"> <strong>C.</strong> Use Amazon DynamoDB Global Tables to provide fast, local, read and write performance in each region</label><br>
<label for="q70-d"><input type="radio" id="q70-d" name="q70" value="D"> <strong>D.</strong> Spin up a Amazon Redshift cluster in each AWS region. Migrate the existing data into Redshift clusters</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon Aurora Global Database to enable fast local reads with low latency in each region

</details>

---

## Câu 71

**Chủ đề:** Design High-Performing Architectures

A silicon valley based startup has a content management application with the web-tier running on Amazon EC2 instances and the database tier running on Amazon Aurora. Currently, the entire infrastructure is located in us-east-1 region. The startup has 90% of its customers in the US and Europe. The engineering team is getting reports of deteriorated application performance from customers in Europe with high application load time.

As a solutions architect, which of the following would you recommend addressing these performance issues? (Select two)

**Lựa chọn:**

<label for="q71-a"><input type="checkbox" id="q71-a" name="q71" value="A"> <strong>A.</strong> Setup another fleet of Amazon EC2 instances for the web tier in the eu-west-1 region. Enable latency routing policy in Amazon Route 53</label><br>
<label for="q71-b"><input type="checkbox" id="q71-b" name="q71" value="B"> <strong>B.</strong> Setup another fleet of Amazon EC2 instances for the web tier in the eu-west-1 region. Enable geolocation routing policy in Amazon Route 53</label><br>
<label for="q71-c"><input type="checkbox" id="q71-c" name="q71" value="C"> <strong>C.</strong> Create Amazon Aurora read replicas in the eu-west-1 region</label><br>
<label for="q71-d"><input type="checkbox" id="q71-d" name="q71" value="D"> <strong>D.</strong> Create Amazon Aurora Multi-AZ standby instance in the eu-west-1 region</label><br>
<label for="q71-e"><input type="checkbox" id="q71-e" name="q71" value="E"> <strong>E.</strong> Setup another fleet of Amazon EC2 instances for the web tier in the eu-west-1 region. Enable failover routing policy in Amazon Route 53</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Setup another fleet of Amazon EC2 instances for the web tier in the eu-west-1 region. Enable latency routing policy in Amazon Route 53

C. Create Amazon Aurora read replicas in the eu-west-1 region

</details>

---

## Câu 72

**Chủ đề:** Design High-Performing Architectures

A video conferencing platform serves users worldwide through a globally distributed deployment of Amazon EC2 instances behind Network Load Balancers (NLBs) in several AWS Regions. The platform's architecture currently allows clients to connect to any Region via public endpoints, depending on how DNS resolves. However, users in regions far from the load balancers frequently experience high latency and slow connection times, especially during session initiation. The company wants to optimize the experience for global users by reducing end-to-end latency and load time while keeping the existing NLBs and EC2-based application infrastructure in place.

Which solution will best meet these requirements?

**Lựa chọn:**

<label for="q72-a"><input type="radio" id="q72-a" name="q72" value="A"> <strong>A.</strong> Deploy a standard accelerator in AWS Global Accelerator and register the existing regional NLBs as endpoints. Use the accelerator to route user requests through AWS’s global edge network to the closest healthy Regional NLB</label><br>
<label for="q72-b"><input type="radio" id="q72-b" name="q72" value="B"> <strong>B.</strong> Deploy Amazon CloudFront with HTTP caching enabled in front of the NLBs. Use CloudFront edge locations to serve user requests faster and reduce the load on the backend EC2 instances</label><br>
<label for="q72-c"><input type="radio" id="q72-c" name="q72" value="C"> <strong>C.</strong> Replace all Network Load Balancers (NLBs) with Application Load Balancers (ALBs) in each Region. Register the EC2 instances as targets behind the ALBs and use cross-zone load balancing for latency distribution</label><br>
<label for="q72-d"><input type="radio" id="q72-d" name="q72" value="D"> <strong>D.</strong> Configure Amazon Route 53 with latency-based routing policies to direct users to the Region with the lowest response time. Use health checks to fail over to another Region if a specific NLB becomes unhealthy</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy a standard accelerator in AWS Global Accelerator and register the existing regional NLBs as endpoints. Use the accelerator to route user requests through AWS’s global edge network to the closest healthy Regional NLB

</details>

---

## Câu 73

**Chủ đề:** Design Resilient Architectures

An IT company is working on a client project to build a Supply Chain Management application. The web-tier of the application runs on an Amazon EC2 instance and the database tier is on Amazon RDS MySQL. For beta testing, all the resources are currently deployed in a single Availability Zone (AZ). The development team wants to improve application availability before the go-live.

Given that all end users of the web application would be located in the US, which of the following would be the MOST resource-efficient solution?

**Lựa chọn:**

<label for="q73-a"><input type="radio" id="q73-a" name="q73" value="A"> <strong>A.</strong> Deploy the web-tier Amazon EC2 instances in two Availability Zones (AZs), behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in read replica configuration</label><br>
<label for="q73-b"><input type="radio" id="q73-b" name="q73" value="B"> <strong>B.</strong> Deploy the web-tier Amazon EC2 instances in two Availability Zones (AZs), behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in Multi-AZ configuration</label><br>
<label for="q73-c"><input type="radio" id="q73-c" name="q73" value="C"> <strong>C.</strong> Deploy the web-tier Amazon EC2 instances in two regions, behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in Multi-AZ configuration</label><br>
<label for="q73-d"><input type="radio" id="q73-d" name="q73" value="D"> <strong>D.</strong> Deploy the web-tier Amazon EC2 instances in two regions, behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in read replica configuration</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Deploy the web-tier Amazon EC2 instances in two Availability Zones (AZs), behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in Multi-AZ configuration

</details>

---

## Câu 74

**Chủ đề:** Design Secure Architectures

A financial services company has deployed its flagship application on Amazon EC2 instances. Since the application handles sensitive customer data, the security team at the company wants to ensure that any third-party Secure Sockets Layer certificate (SSL certificate) SSL/Transport Layer Security (TLS) certificates configured on Amazon EC2 instances via the AWS Certificate Manager (ACM) are renewed before their expiry date. The company has hired you as an AWS Certified Solutions Architect Associate to build a solution that notifies the security team 30 days before the certificate expiration. The solution should require the least amount of scripting and maintenance effort.

What will you recommend?

**Lựa chọn:**

<label for="q74-a"><input type="radio" id="q74-a" name="q74" value="A"> <strong>A.</strong> Monitor the days to expiry Amazon CloudWatch metric for certificates created via ACM. Create a CloudWatch alarm to monitor such certificates based on the days to expiry metric and then trigger a custom action of notifying the security team</label><br>
<label for="q74-b"><input type="radio" id="q74-b" name="q74" value="B"> <strong>B.</strong> Monitor the days to expiry Amazon CloudWatch metric for certificates imported into ACM. Create a CloudWatch alarm to monitor such certificates based on the days to expiry metric and then trigger a custom action of notifying the security team</label><br>
<label for="q74-c"><input type="radio" id="q74-c" name="q74" value="C"> <strong>C.</strong> Leverage AWS Config managed rule to check if any SSL/TLS certificates created via ACM are marked for expiration within 30 days. Configure the rule to trigger an Amazon SNS notification to the security team if any certificate expires within 30 days</label><br>
<label for="q74-d"><input type="radio" id="q74-d" name="q74" value="D"> <strong>D.</strong> Leverage AWS Config managed rule to check if any third-party SSL/TLS certificates imported into ACM are marked for expiration within 30 days. Configure the rule to trigger an Amazon SNS notification to the security team if any certificate expires within 30 days</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Leverage AWS Config managed rule to check if any third-party SSL/TLS certificates imported into ACM are marked for expiration within 30 days. Configure the rule to trigger an Amazon SNS notification to the security team if any certificate expires within 30 days

</details>

---

## Câu 75

**Chủ đề:** Design Secure Architectures

A financial services company has developed its flagship application on AWS Cloud with data security requirements such that the encryption key must be stored in a custom application running on-premises. The company wants to offload the data storage as well as the encryption process to Amazon S3 but continue to use the existing encryption key.

Which of the following Amazon S3 encryption options allows the company to leverage Amazon S3 for storing data with given constraints?

**Lựa chọn:**

<label for="q75-a"><input type="radio" id="q75-a" name="q75" value="A"> <strong>A.</strong> Server-Side Encryption with Amazon S3 managed keys (SSE-S3)</label><br>
<label for="q75-b"><input type="radio" id="q75-b" name="q75" value="B"> <strong>B.</strong> Server-Side Encryption with AWS Key Management Service (AWS KMS) keys (SSE-KMS)</label><br>
<label for="q75-c"><input type="radio" id="q75-c" name="q75" value="C"> <strong>C.</strong> Server-Side Encryption with Customer-Provided Keys (SSE-C)</label><br>
<label for="q75-d"><input type="radio" id="q75-d" name="q75" value="D"> <strong>D.</strong> Client-Side Encryption with data encryption is done on the client-side before sending it to Amazon S3</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Server-Side Encryption with Customer-Provided Keys (SSE-C)

</details>

---

## Câu 76

**Chủ đề:** Design High-Performing Architectures

A media company has created an AWS Direct Connect connection for migrating its flagship application to the AWS Cloud. The on-premises application writes hundreds of video files into a mounted NFS file system daily. Post-migration, the company will host the application on an Amazon EC2 instance with a mounted Amazon Elastic File System (Amazon EFS) file system. Before the migration cutover, the company must build a process that will replicate the newly created on-premises video files to the Amazon EFS file system.

Which of the following represents the MOST operationally efficient way to meet this requirement?

**Lựa chọn:**

<label for="q76-a"><input type="radio" id="q76-a" name="q76" value="A"> <strong>A.</strong> Configure an AWS DataSync agent on the on-premises server that has access to the NFS file system. Transfer data over the AWS Direct Connect connection to an AWS VPC peering endpoint for Amazon EFS by using a private VIF. Set up an AWS DataSync scheduled task to send the video files to the Amazon EFS file system every 24 hours</label><br>
<label for="q76-b"><input type="radio" id="q76-b" name="q76" value="B"> <strong>B.</strong> Configure an AWS DataSync agent on the on-premises server that has access to the NFS file system. Transfer data over the AWS Direct Connect connection to an Amazon S3 bucket by using public VIF. Set up an AWS Lambda function to process event notifications from Amazon S3 and copy the video files from Amazon S3 to the Amazon EFS file system</label><br>
<label for="q76-c"><input type="radio" id="q76-c" name="q76" value="C"> <strong>C.</strong> Configure an AWS DataSync agent on the on-premises server that has access to the NFS file system. Transfer data over the AWS Direct Connect connection to an AWS PrivateLink interface VPC endpoint for Amazon EFS by using a private VIF. Set up an AWS DataSync scheduled task to send the video files to the Amazon EFS file system every 24 hours</label><br>
<label for="q76-d"><input type="radio" id="q76-d" name="q76" value="D"> <strong>D.</strong> Configure an AWS DataSync agent on the on-premises server that has access to the NFS file system. Transfer data over the AWS Direct Connect connection to an Amazon S3 bucket by using a VPC gateway endpoint for Amazon S3. Set up an AWS Lambda function to process event notifications from Amazon S3 and copy the video files from Amazon S3 to the Amazon EFS file system</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Configure an AWS DataSync agent on the on-premises server that has access to the NFS file system. Transfer data over the AWS Direct Connect connection to an AWS PrivateLink interface VPC endpoint for Amazon EFS by using a private VIF. Set up an AWS DataSync scheduled task to send the video files to the Amazon EFS file system every 24 hours

</details>

---

## Câu 77

**Chủ đề:** Design High-Performing Architectures

A media production studio is building a content rendering and editing platform on AWS. The editing workstations and rendering tools require access to shared files over the SMB (Server Message Block) protocol. The studio wants a managed storage solution that is simple to set up, integrates easily with SMB clients, and minimizes ongoing operational tasks.

Which solution will best meet the requirements with the LEAST administrative overhead?

**Lựa chọn:**

<label for="q77-a"><input type="radio" id="q77-a" name="q77" value="A"> <strong>A.</strong> Use Amazon S3 with Transfer Acceleration enabled. Configure the application to upload and download files over HTTPS using signed URLs</label><br>
<label for="q77-b"><input type="radio" id="q77-b" name="q77" value="B"> <strong>B.</strong> Launch an Amazon EC2 Windows instance and manually configure a Windows file share. Use this instance to serve SMB access to application clients</label><br>
<label for="q77-c"><input type="radio" id="q77-c" name="q77" value="C"> <strong>C.</strong> Provision an Amazon FSx for Windows File Server file system. Mount the file system using the SMB protocol on the media servers</label><br>
<label for="q77-d"><input type="radio" id="q77-d" name="q77" value="D"> <strong>D.</strong> Set up an AWS Storage Gateway Volume Gateway in cached volume mode. Attach the volume as an iSCSI device to the application server and configure a file system with SMB sharing enabled</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Provision an Amazon FSx for Windows File Server file system. Mount the file system using the SMB protocol on the media servers

</details>

---

## Câu 78

**Chủ đề:** Design Resilient Architectures

An e-commerce application uses an Amazon Aurora Multi-AZ deployment for its database. While analyzing the performance metrics, the engineering team has found that the database reads are causing high input/output (I/O) and adding latency to the write requests against the database.

As an AWS Certified Solutions Architect Associate, what would you recommend to separate the read requests from the write requests?

**Lựa chọn:**

<label for="q78-a"><input type="radio" id="q78-a" name="q78" value="A"> <strong>A.</strong> Provision another Amazon Aurora database and link it to the primary database as a read replica</label><br>
<label for="q78-b"><input type="radio" id="q78-b" name="q78" value="B"> <strong>B.</strong> Set up a read replica and modify the application to use the appropriate endpoint</label><br>
<label for="q78-c"><input type="radio" id="q78-c" name="q78" value="C"> <strong>C.</strong> Configure the application to read from the Multi-AZ standby instance</label><br>
<label for="q78-d"><input type="radio" id="q78-d" name="q78" value="D"> <strong>D.</strong> Activate read-through caching on the Amazon Aurora database</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up a read replica and modify the application to use the appropriate endpoint

</details>

---

## Câu 79

**Chủ đề:** Design Cost-Optimized Architectures

A mobile app allows users to submit photos, which are stored in an Amazon S3 bucket. Currently, a batch of Amazon EC2 Spot Instances is launched nightly to process all the day’s uploads. Each photo requires approximately 3 minutes and 512 MB of memory to process. To improve responsiveness and minimize costs, the company wants to shift to near real-time image processing that begins as soon as an image is uploaded.

Which solution will provide the MOST cost-effective and scalable architecture to meet these new requirements?

**Lựa chọn:**

<label for="q79-a"><input type="radio" id="q79-a" name="q79" value="A"> <strong>A.</strong> Configure Amazon S3 to send event notifications to an Amazon SQS queue each time a photo is uploaded. Set up an AWS Lambda function to poll the queue and process images asynchronously</label><br>
<label for="q79-b"><input type="radio" id="q79-b" name="q79" value="B"> <strong>B.</strong> Set up Amazon S3 to push events to an Amazon SQS queue. Launch a single EC2 Reserved Instance that continuously polls the queue and processes each image upon receipt</label><br>
<label for="q79-c"><input type="radio" id="q79-c" name="q79" value="C"> <strong>C.</strong> Enable S3 event notifications to invoke an Amazon EventBridge rule. Configure an AWS Step Functions workflow to initiate an Fargate task in Amazon ECS to process the image</label><br>
<label for="q79-d"><input type="radio" id="q79-d" name="q79" value="D"> <strong>D.</strong> Configure S3 to trigger an AWS App Runner service directly. Deploy a containerized image-processing application to App Runner to automatically process each upload</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Configure Amazon S3 to send event notifications to an Amazon SQS queue each time a photo is uploaded. Set up an AWS Lambda function to poll the queue and process images asynchronously

</details>

---

## Câu 80

**Chủ đề:** Design High-Performing Architectures

A digital media company stores several terabytes of newly generated advertising interaction logs in an Amazon S3 bucket each day. The development team needs to inspect the new dataset quickly by running ad hoc queries before deciding whether the records should enter a downstream transformation workflow. The company wants to minimize infrastructure management and operational effort.

Which solution will meet these requirements with the LEAST operational overhead?

**Lựa chọn:**

<label for="q80-a"><input type="radio" id="q80-a" name="q80" value="A"> <strong>A.</strong> Create external tables in an Apache Hive metastore, and run Apache Spark jobs on an Amazon EMR cluster to analyze the data in Amazon S3</label><br>
<label for="q80-b"><input type="radio" id="q80-b" name="q80" value="B"> <strong>B.</strong> Create external tables in a Spark catalog, and configure AWS Glue ETL jobs to read and analyze the newly generated data in Amazon S3</label><br>
<label for="q80-c"><input type="radio" id="q80-c" name="q80" value="C"> <strong>C.</strong> Load the S3 objects into Amazon Redshift by using COPY commands, and run SQL queries against the loaded data before initiating additional processing</label><br>
<label for="q80-d"><input type="radio" id="q80-d" name="q80" value="D"> <strong>D.</strong> Configure an AWS Glue crawler to catalog the S3 dataset, and use Amazon Athena to run ad hoc SQL queries directly against the data</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Configure an AWS Glue crawler to catalog the S3 dataset, and use Amazon Athena to run ad hoc SQL queries directly against the data

</details>

---

## Câu 81

**Chủ đề:** Design Secure Architectures

A developer needs to implement an AWS Lambda function in AWS account A that accesses an Amazon Simple Storage Service (Amazon S3) bucket in AWS account B.

As a Solutions Architect, which of the following will you recommend to meet this requirement?

**Lựa chọn:**

<label for="q81-a"><input type="radio" id="q81-a" name="q81" value="A"> <strong>A.</strong> Create an IAM role for the AWS Lambda function that grants access to the Amazon S3 bucket. Set the IAM role as the AWS Lambda function's execution role. Make sure that the bucket policy also grants access to the AWS Lambda function's execution role</label><br>
<label for="q81-b"><input type="radio" id="q81-b" name="q81" value="B"> <strong>B.</strong> AWS Lambda cannot access resources across AWS accounts. Use Identity federation to work around this limitation of Lambda</label><br>
<label for="q81-c"><input type="radio" id="q81-c" name="q81" value="C"> <strong>C.</strong> Create an IAM role for the AWS Lambda function that grants access to the Amazon S3 bucket. Set the IAM role as the Lambda function's execution role and that would give the AWS Lambda function cross-account access to the Amazon S3 bucket</label><br>
<label for="q81-d"><input type="radio" id="q81-d" name="q81" value="D"> <strong>D.</strong> The Amazon S3 bucket owner should make the bucket public so that it can be accessed by the AWS Lambda function in the other AWS account</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an IAM role for the AWS Lambda function that grants access to the Amazon S3 bucket. Set the IAM role as the AWS Lambda function's execution role. Make sure that the bucket policy also grants access to the AWS Lambda function's execution role

</details>

---

## Câu 82

**Chủ đề:** Design Secure Architectures

A social media application is hosted on an Amazon EC2 fleet running behind an Application Load Balancer. The application traffic is fronted by an Amazon CloudFront distribution. The engineering team wants to decouple the user authentication process for the application, so that the application servers can just focus on the business logic.

As a Solutions Architect, which of the following solutions would you recommend to the development team so that it requires minimal development effort?

**Lựa chọn:**

<label for="q82-a"><input type="radio" id="q82-a" name="q82" value="A"> <strong>A.</strong> Use Amazon Cognito Authentication via Cognito User Pools for your Application Load Balancer</label><br>
<label for="q82-b"><input type="radio" id="q82-b" name="q82" value="B"> <strong>B.</strong> Use Amazon Cognito Authentication via Cognito Identity Pools for your Application Load Balancer</label><br>
<label for="q82-c"><input type="radio" id="q82-c" name="q82" value="C"> <strong>C.</strong> Use Amazon Cognito Authentication via Cognito User Pools for your Amazon CloudFront distribution</label><br>
<label for="q82-d"><input type="radio" id="q82-d" name="q82" value="D"> <strong>D.</strong> Use Amazon Cognito Authentication via Cognito Identity Pools for your Amazon CloudFront distribution</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon Cognito Authentication via Cognito User Pools for your Application Load Balancer

</details>

---

## Câu 83

**Chủ đề:** Design Resilient Architectures

The engineering team at a logistics company has noticed that the Auto Scaling group (ASG) is not terminating an unhealthy Amazon EC2 instance.

As a Solutions Architect, which of the following options would you suggest to troubleshoot the issue? (Select three)

**Lựa chọn:**

<label for="q83-a"><input type="checkbox" id="q83-a" name="q83" value="A"> <strong>A.</strong> A user might have updated the configuration of the Auto Scaling group (ASG) and increased the minimum number of instances forcing ASG to keep all instances alive</label><br>
<label for="q83-b"><input type="checkbox" id="q83-b" name="q83" value="B"> <strong>B.</strong> The Amazon EC2 instance could be a spot instance type, which cannot be terminated by the Auto Scaling group (ASG)</label><br>
<label for="q83-c"><input type="checkbox" id="q83-c" name="q83" value="C"> <strong>C.</strong> The health check grace period for the instance has not expired</label><br>
<label for="q83-d"><input type="checkbox" id="q83-d" name="q83" value="D"> <strong>D.</strong> The instance maybe in Impaired status</label><br>
<label for="q83-e"><input type="checkbox" id="q83-e" name="q83" value="E"> <strong>E.</strong> The instance has failed the Elastic Load Balancing (ELB) health check status</label><br>
<label for="q83-f"><input type="checkbox" id="q83-f" name="q83" value="F"> <strong>F.</strong> A custom health check might have failed. The Auto Scaling group (ASG) does not terminate instances that are set unhealthy by custom checks</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. The health check grace period for the instance has not expired

D. The instance maybe in Impaired status

E. The instance has failed the Elastic Load Balancing (ELB) health check status

</details>

---

## Câu 84

**Chủ đề:** Design High-Performing Architectures

An engineering team wants to examine the feasibility of the user data feature of Amazon EC2 for an upcoming project.

Which of the following are true about the Amazon EC2 user data configuration? (Select two)

**Lựa chọn:**

<label for="q84-a"><input type="checkbox" id="q84-a" name="q84" value="A"> <strong>A.</strong> By default, user data is executed every time an Amazon EC2 instance is re-started</label><br>
<label for="q84-b"><input type="checkbox" id="q84-b" name="q84" value="B"> <strong>B.</strong> When an instance is running, you can update user data by using root user credentials</label><br>
<label for="q84-c"><input type="checkbox" id="q84-c" name="q84" value="C"> <strong>C.</strong> By default, scripts entered as user data are executed with root user privileges</label><br>
<label for="q84-d"><input type="checkbox" id="q84-d" name="q84" value="D"> <strong>D.</strong> By default, user data runs only during the boot cycle when you first launch an instance</label><br>
<label for="q84-e"><input type="checkbox" id="q84-e" name="q84" value="E"> <strong>E.</strong> By default, scripts entered as user data do not have root user privileges for executing</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. By default, scripts entered as user data are executed with root user privileges

D. By default, user data runs only during the boot cycle when you first launch an instance

</details>

---

## Câu 85

**Chủ đề:** Design Secure Architectures

A systems administrator has created a private hosted zone and associated it with a Virtual Private Cloud (VPC). However, the Domain Name System (DNS) queries for the private hosted zone remain unresolved.

As a Solutions Architect, can you identify the Amazon Virtual Private Cloud (Amazon VPC) options to be configured in order to get the private hosted zone to work?

**Lựa chọn:**

<label for="q85-a"><input type="radio" id="q85-a" name="q85" value="A"> <strong>A.</strong> Remove any overlapping namespaces for the private and public hosted zones</label><br>
<label for="q85-b"><input type="radio" id="q85-b" name="q85" value="B"> <strong>B.</strong> Fix the Name server (NS) record and Start Of Authority (SOA) records that may have been created with wrong configurations</label><br>
<label for="q85-c"><input type="radio" id="q85-c" name="q85" value="C"> <strong>C.</strong> Fix conflicts between your private hosted zone and any Resolver rule that routes traffic to your network for the same domain name, as it results in ambiguity over the route to be taken</label><br>
<label for="q85-d"><input type="radio" id="q85-d" name="q85" value="D"> <strong>D.</strong> Enable DNS hostnames and DNS resolution for private hosted zones</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Enable DNS hostnames and DNS resolution for private hosted zones

</details>

---

## Câu 86

**Chủ đề:** Design Secure Architectures

An e-commerce company operates multiple AWS accounts and has interconnected these accounts in a hub-and-spoke style using the AWS Transit Gateway. Amazon Virtual Private Cloud (Amazon VPCs) have been provisioned across these AWS accounts to facilitate network isolation.

Which of the following solutions would reduce both the administrative overhead and the costs while providing shared access to services required by workloads in each of the VPCs?

**Lựa chọn:**

<label for="q86-a"><input type="radio" id="q86-a" name="q86" value="A"> <strong>A.</strong> Build a shared services Amazon Virtual Private Cloud (Amazon VPC)</label><br>
<label for="q86-b"><input type="radio" id="q86-b" name="q86" value="B"> <strong>B.</strong> Use Transit VPC to reduce cost and share the resources across Amazon Virtual Private Cloud (Amazon VPCs)</label><br>
<label for="q86-c"><input type="radio" id="q86-c" name="q86" value="C"> <strong>C.</strong> Use Fully meshed VPC Peering connection</label><br>
<label for="q86-d"><input type="radio" id="q86-d" name="q86" value="D"> <strong>D.</strong> Use VPCs connected with AWS Direct Connect</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Build a shared services Amazon Virtual Private Cloud (Amazon VPC)

</details>

---

## Câu 87

**Chủ đề:** Design Resilient Architectures

A retail company wants to rollout and test a blue-green deployment for its global application in the next 48 hours. Most of the customers use mobile phones which are prone to Domain Name System (DNS) caching. The company has only two days left for the annual Thanksgiving sale to commence.

As a Solutions Architect, which of the following options would you recommend to test the deployment on as many users as possible in the given time frame?

**Lựa chọn:**

<label for="q87-a"><input type="radio" id="q87-a" name="q87" value="A"> <strong>A.</strong> Use Amazon Route 53 weighted routing to spread traffic across different deployments</label><br>
<label for="q87-b"><input type="radio" id="q87-b" name="q87" value="B"> <strong>B.</strong> Use AWS Global Accelerator to distribute a portion of traffic to a particular deployment</label><br>
<label for="q87-c"><input type="radio" id="q87-c" name="q87" value="C"> <strong>C.</strong> Use Elastic Load Balancing (ELB) to distribute traffic across deployments</label><br>
<label for="q87-d"><input type="radio" id="q87-d" name="q87" value="D"> <strong>D.</strong> Use AWS CodeDeploy deployment options to choose the right deployment</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS Global Accelerator to distribute a portion of traffic to a particular deployment

</details>

---

## Câu 88

**Chủ đề:** Design Secure Architectures

A health-care solutions company wants to run their applications on single-tenant hardware to meet regulatory guidelines.

Which of the following is the MOST cost-effective way of isolating their Amazon Elastic Compute Cloud (Amazon EC2)instances to a single tenant?

**Lựa chọn:**

<label for="q88-a"><input type="radio" id="q88-a" name="q88" value="A"> <strong>A.</strong> Dedicated Instances</label><br>
<label for="q88-b"><input type="radio" id="q88-b" name="q88" value="B"> <strong>B.</strong> Spot Instances</label><br>
<label for="q88-c"><input type="radio" id="q88-c" name="q88" value="C"> <strong>C.</strong> Dedicated Hosts</label><br>
<label for="q88-d"><input type="radio" id="q88-d" name="q88" value="D"> <strong>D.</strong> On-Demand Instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Dedicated Instances

</details>

---

## Câu 89

**Chủ đề:** Design Secure Architectures

An enterprise uses a centralized Amazon S3 bucket to store logs and reports generated by multiple analytics services. Each service writes to and reads from a dedicated prefix (folder path) in the bucket. The company wants to enforce fine-grained access control so that each service can access only its own prefix, without being able to see or modify other services' data. The solution must support scalable and maintainable permissions management with minimal operational overhead.

Which approach will best meet these requirements?

**Lựa chọn:**

<label for="q89-a"><input type="radio" id="q89-a" name="q89" value="A"> <strong>A.</strong> Create separate IAM users for each service. Manually assign inline IAM policies to grant read/write permissions to the S3 bucket. Reference specific object names in the policy for each user</label><br>
<label for="q89-b"><input type="radio" id="q89-b" name="q89" value="B"> <strong>B.</strong> Configure individual S3 access points for each analytics service. Attach access point policies that restrict access to only the relevant prefix in the S3 bucket</label><br>
<label for="q89-c"><input type="radio" id="q89-c" name="q89" value="C"> <strong>C.</strong> Deploy Amazon Macie to classify the objects in the bucket by prefix and apply automated object-level access policies to each object based on service tags</label><br>
<label for="q89-d"><input type="radio" id="q89-d" name="q89" value="D"> <strong>D.</strong> Create a single S3 bucket policy that lists all object ARNs under each prefix and grants permissions accordingly. Use resource-level permissions to restrict access to individual services</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure individual S3 access points for each analytics service. Attach access point policies that restrict access to only the relevant prefix in the S3 bucket

</details>

---

## Câu 90

**Chủ đề:** Design Resilient Architectures

The DevOps team at a major financial services company uses Multi-Availability Zone (Multi-AZ) deployment for its MySQL Amazon RDS database in order to automate its database replication and augment data durability. The DevOps team has scheduled a maintenance window for a database engine level upgrade for the coming weekend.

Which of the following is the correct outcome during the maintenance window?

**Lựa chọn:**

<label for="q90-a"><input type="radio" id="q90-a" name="q90" value="A"> <strong>A.</strong> Any database engine level upgrade for an Amazon RDS database instance with Multi-AZ deployment triggers both the primary and standby database instances to be upgraded at the same time. However, this does not cause any downtime until the upgrade is complete</label><br>
<label for="q90-b"><input type="radio" id="q90-b" name="q90" value="B"> <strong>B.</strong> Any database engine level upgrade for an Amazon RDS database instance with Multi-AZ deployment triggers the standby database instance to be upgraded which is then followed by the upgrade of the primary database instance. This does not cause any downtime for the duration of the upgrade</label><br>
<label for="q90-c"><input type="radio" id="q90-c" name="q90" value="C"> <strong>C.</strong> Any database engine level upgrade for an Amazon RDS database instance with Multi-AZ deployment triggers the primary database instance to be upgraded which is then followed by the upgrade of the standby database instance. This does not cause any downtime for the duration of the upgrade</label><br>
<label for="q90-d"><input type="radio" id="q90-d" name="q90" value="D"> <strong>D.</strong> Any database engine level upgrade for an Amazon RDS database instance with Multi-AZ deployment triggers both the primary and standby database instances to be upgraded at the same time. This causes downtime until the upgrade is complete</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Any database engine level upgrade for an Amazon RDS database instance with Multi-AZ deployment triggers both the primary and standby database instances to be upgraded at the same time. This causes downtime until the upgrade is complete

</details>

---

## Câu 91

**Chủ đề:** Design High-Performing Architectures

A global media agency is developing a cultural analysis project to explore how major sports stories have evolved over the last five years. The team has collected thousands of archived news bulletins and magazine spreads stored in PDF format. These documents are rich in unstructured text and come from various sources with differing layouts and font styles. The agency wants to better understand how public tone and narrative have shifted over time. The team has chosen to use Amazon Textract for its ability to accurately extract printed and scanned text from complex PDF layouts. They need a solution that can then analyze the emotional tone and subject matter of the extracted text with the least possible operational burden, using fully managed AWS services where possible.

Which solution will best meet these requirements?

**Lựa chọn:**

<label for="q91-a"><input type="radio" id="q91-a" name="q91" value="A"> <strong>A.</strong> Use Amazon SageMaker to train a custom sentiment analysis model. Store the model outputs in Amazon DynamoDB for structured querying by analysts</label><br>
<label for="q91-b"><input type="radio" id="q91-b" name="q91" value="B"> <strong>B.</strong> Process the extracted output with AWS Lambda to convert the text into CSV format. Query the data using Amazon Athena and visualize it using Amazon QuickSight.</label><br>
<label for="q91-c"><input type="radio" id="q91-c" name="q91" value="C"> <strong>C.</strong> Ingest the extracted data into Amazon Redshift using AWS Glue, and use Amazon Rekognition to analyze the tone of the document layouts for sentiment classification.</label><br>
<label for="q91-d"><input type="radio" id="q91-d" name="q91" value="D"> <strong>D.</strong> Send the extracted text to Amazon Comprehend for entity detection and sentiment analysis. Store the results in Amazon S3 for further access or visualization.</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Send the extracted text to Amazon Comprehend for entity detection and sentiment analysis. Store the results in Amazon S3 for further access or visualization.

</details>

---

## Câu 92

**Chủ đề:** Design High-Performing Architectures

A manufacturing analytics company has a large collection of automated scripts that perform data cleanup, validation, and system integration tasks. These scripts are currently run by a local Linux cron scheduler and have an execution time of up to 30 minutes. The company wants to migrate these scripts to AWS without significant changes, and would prefer a containerized, serverless architecture that automatically scales and can respond to event-based triggers in the future. The solution must minimize infrastructure management.

Which solution will best meet these requirements with minimal refactoring and operational overhead?

**Lựa chọn:**

<label for="q92-a"><input type="radio" id="q92-a" name="q92" value="A"> <strong>A.</strong> Convert each script into a Lambda function and package it in a zip archive. Use Amazon EventBridge Scheduler to run the functions on a fixed schedule. Use Amazon S3 to store function outputs and logs</label><br>
<label for="q92-b"><input type="radio" id="q92-b" name="q92" value="B"> <strong>B.</strong> Package the scripts into a container image. Use Amazon EventBridge Scheduler to define cron-based recurring schedules. Configure EventBridge Scheduler to invoke AWS Fargate tasks using Amazon ECS</label><br>
<label for="q92-c"><input type="radio" id="q92-c" name="q92" value="C"> <strong>C.</strong> Package the scripts into a container image. Deploy the image to AWS Batch with a managed compute environment on Amazon EC2. Define scheduling policies in AWS Batch to trigger jobs according to cron expressions</label><br>
<label for="q92-d"><input type="radio" id="q92-d" name="q92" value="D"> <strong>D.</strong> Create a container image for each script. Use AWS Step Functions to define a workflow for all scheduled tasks. Use a Wait state to delay execution and run tasks using Step Functions’ RunTask integration with ECS Fargate</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Package the scripts into a container image. Use Amazon EventBridge Scheduler to define cron-based recurring schedules. Configure EventBridge Scheduler to invoke AWS Fargate tasks using Amazon ECS

</details>

---

## Câu 93

**Chủ đề:** Design Secure Architectures

A silicon valley based startup has a two-tier architecture using Amazon EC2 instances for its flagship application. The web servers (listening on port 443), which have been assigned security group A, are in public subnets across two Availability Zones (AZs) and the MSSQL based database instances (listening on port 1433), which have been assigned security group B, are in two private subnets across two Availability Zones (AZs). The DevOps team wants to review the security configurations of the application architecture.

As a solutions architect, which of the following options would you select as the MOST secure configuration? (Select two)

**Lựa chọn:**

<label for="q93-a"><input type="checkbox" id="q93-a" name="q93" value="A"> <strong>A.</strong> For security group A: Add an inbound rule that allows traffic from all sources on port 443. Add an outbound rule with the destination as security group B on port 443</label><br>
<label for="q93-b"><input type="checkbox" id="q93-b" name="q93" value="B"> <strong>B.</strong> For security group B: Add an inbound rule that allows traffic only from all sources on port 1433</label><br>
<label for="q93-c"><input type="checkbox" id="q93-c" name="q93" value="C"> <strong>C.</strong> For security group B: Add an inbound rule that allows traffic only from security group A on port 443</label><br>
<label for="q93-d"><input type="checkbox" id="q93-d" name="q93" value="D"> <strong>D.</strong> For security group A: Add an inbound rule that allows traffic from all sources on port 443. Add an outbound rule with the destination as security group B on port 1433</label><br>
<label for="q93-e"><input type="checkbox" id="q93-e" name="q93" value="E"> <strong>E.</strong> For security group B: Add an inbound rule that allows traffic only from security group A on port 1433</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. For security group A: Add an inbound rule that allows traffic from all sources on port 443. Add an outbound rule with the destination as security group B on port 1433

E. For security group B: Add an inbound rule that allows traffic only from security group A on port 1433

</details>

---

## Câu 94

**Chủ đề:** Design Resilient Architectures

A startup has just developed a video backup service hosted on a fleet of Amazon EC2 instances. The Amazon EC2 instances are behind an Application Load Balancer and the instances are using Amazon Elastic Block Store (Amazon EBS) Volumes for storage. The service provides authenticated users the ability to upload videos that are then saved on the EBS volume attached to a given instance. On the first day of the beta launch, users start complaining that they can see only some of the videos in their uploaded videos backup. Every time the users log into the website, they claim to see a different subset of their uploaded videos.

Which of the following is the MOST optimal solution to make sure that users can view all the uploaded videos? (Select two)

**Lựa chọn:**

<label for="q94-a"><input type="checkbox" id="q94-a" name="q94" value="A"> <strong>A.</strong> Write a one time job to copy the videos from all Amazon EBS volumes to Amazon S3 Glacier Deep Archive and then modify the application to use Amazon S3 Glacier Deep Archive for storing the videos</label><br>
<label for="q94-b"><input type="checkbox" id="q94-b" name="q94" value="B"> <strong>B.</strong> Write a one time job to copy the videos from all Amazon EBS volumes to Amazon S3 and then modify the application to use Amazon S3 standard for storing the videos</label><br>
<label for="q94-c"><input type="checkbox" id="q94-c" name="q94" value="C"> <strong>C.</strong> Write a one time job to copy the videos from all Amazon EBS volumes to Amazon RDS and then modify the application to use Amazon RDS for storing the videos</label><br>
<label for="q94-d"><input type="checkbox" id="q94-d" name="q94" value="D"> <strong>D.</strong> Mount Amazon Elastic File System (Amazon EFS) on all Amazon EC2 instances. Write a one time job to copy the videos from all Amazon EBS volumes to Amazon EFS. Modify the application to use Amazon EFS for storing the videos</label><br>
<label for="q94-e"><input type="checkbox" id="q94-e" name="q94" value="E"> <strong>E.</strong> Write a one time job to copy the videos from all Amazon EBS volumes to Amazon DynamoDB and then modify the application to use Amazon DynamoDB for storing the videos</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Write a one time job to copy the videos from all Amazon EBS volumes to Amazon S3 and then modify the application to use Amazon S3 standard for storing the videos

D. Mount Amazon Elastic File System (Amazon EFS) on all Amazon EC2 instances. Write a one time job to copy the videos from all Amazon EBS volumes to Amazon EFS. Modify the application to use Amazon EFS for storing the videos

</details>

---

## Câu 95

**Chủ đề:** Design Secure Architectures

To improve the performance and security of the application, the engineering team at a company has created an Amazon CloudFront distribution with an Application Load Balancer as the custom origin. The team has also set up an AWS Web Application Firewall (AWS WAF) with Amazon CloudFront distribution. The security team at the company has noticed a surge in malicious attacks from a specific IP address to steal sensitive data stored on the Amazon EC2 instances.

As a solutions architect, which of the following actions would you recommend to stop the attacks?

**Lựa chọn:**

<label for="q95-a"><input type="radio" id="q95-a" name="q95" value="A"> <strong>A.</strong> Create a deny rule for the malicious IP in the network access control list (network ACL) associated with each of the instances</label><br>
<label for="q95-b"><input type="radio" id="q95-b" name="q95" value="B"> <strong>B.</strong> Create a deny rule for the malicious IP in the Security Groups associated with each of the instances</label><br>
<label for="q95-c"><input type="radio" id="q95-c" name="q95" value="C"> <strong>C.</strong> Create an IP match condition in the AWS WAF to block the malicious IP address</label><br>
<label for="q95-d"><input type="radio" id="q95-d" name="q95" value="D"> <strong>D.</strong> Create a ticket with AWS support to take action against the malicious IP</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Create an IP match condition in the AWS WAF to block the malicious IP address

</details>

---

## Câu 96

**Chủ đề:** Design Cost-Optimized Architectures

An application is currently hosted on four Amazon EC2 instances (behind Application Load Balancer) deployed in a single Availability Zone (AZ). To maintain an acceptable level of end-user experience, the application needs at least 4 instances to be always available.

As a solutions architect, which of the following would you recommend so that the application achieves high availability with MINIMUM cost?

**Lựa chọn:**

<label for="q96-a"><input type="radio" id="q96-a" name="q96" value="A"> <strong>A.</strong> Deploy the instances in three Availability Zones (AZs). Launch two instances in each Availability Zone (AZ)</label><br>
<label for="q96-b"><input type="radio" id="q96-b" name="q96" value="B"> <strong>B.</strong> Deploy the instances in two Availability Zones (AZs). Launch two instances in each Availability Zone (AZ)</label><br>
<label for="q96-c"><input type="radio" id="q96-c" name="q96" value="C"> <strong>C.</strong> Deploy the instances in two Availability Zones (AZs). Launch four instances in each Availability Zone (AZ)</label><br>
<label for="q96-d"><input type="radio" id="q96-d" name="q96" value="D"> <strong>D.</strong> Deploy the instances in one Availability Zones. Launch two instances in the Availability Zone (AZ)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy the instances in three Availability Zones (AZs). Launch two instances in each Availability Zone (AZ)

</details>

---

## Câu 97

**Chủ đề:** Design Secure Architectures

A SaaS company is modernizing one of its legacy web applications by migrating it to AWS. The company aims to improve the availability of the application during both normal and peak traffic periods. Additionally, the company wants to implement protection against common web exploits and malicious traffic. The architecture must be scalable and integrate AWS WAF to secure incoming traffic.

Which solution will best meet these requirements with high availability and minimal configuration complexity?

**Lựa chọn:**

<label for="q97-a"><input type="radio" id="q97-a" name="q97" value="A"> <strong>A.</strong> Launch EC2 instances in a single Availability Zone and configure AWS Global Accelerator to route traffic to the instances. Attach AWS WAF to Global Accelerator for application protection</label><br>
<label for="q97-b"><input type="radio" id="q97-b" name="q97" value="B"> <strong>B.</strong> Deploy the application on multiple Amazon EC2 instances in an Auto Scaling group that spans two Availability Zones. Place an Application Load Balancer (ALB) in front of the group. Associate AWS WAF with the ALB</label><br>
<label for="q97-c"><input type="radio" id="q97-c" name="q97" value="C"> <strong>C.</strong> Launch two EC2 instances in separate Availability Zones and register them as targets of an Application Load Balancer. Associate the ALB with AWS WAF to filter incoming traffic</label><br>
<label for="q97-d"><input type="radio" id="q97-d" name="q97" value="D"> <strong>D.</strong> Create an Auto Scaling group with EC2 instances in multiple Availability Zones. Attach a Network Load Balancer (NLB) to distribute incoming traffic. Integrate AWS WAF directly with the Auto Scaling group for traffic filtering</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Deploy the application on multiple Amazon EC2 instances in an Auto Scaling group that spans two Availability Zones. Place an Application Load Balancer (ALB) in front of the group. Associate AWS WAF with the ALB

</details>

---

## Câu 98

**Chủ đề:** Design Cost-Optimized Architectures

An application runs big data workloads on Amazon Elastic Compute Cloud (Amazon EC2) instances. The application runs 24x7 all round the year and needs at least 20 instances to maintain a minimum acceptable performance threshold and the application needs 300 instances to handle spikes in the workload. Based on historical workloads processed by the application, it needs 80 instances 80% of the time.

As a solutions architect, which of the following would you recommend as the MOST cost-optimal solution so that it can meet the workload demand in a steady state?

**Lựa chọn:**

<label for="q98-a"><input type="radio" id="q98-a" name="q98" value="A"> <strong>A.</strong> Purchase 80 reserved instances (RIs). Provision additional on-demand and spot instances per the workload demand (Use Auto Scaling Group with launch template to provision the mix of on-demand and spot instances)</label><br>
<label for="q98-b"><input type="radio" id="q98-b" name="q98" value="B"> <strong>B.</strong> Purchase 20 on-demand instances. Use Auto Scaling Group to provision the remaining instances as spot instances per the workload demand</label><br>
<label for="q98-c"><input type="radio" id="q98-c" name="q98" value="C"> <strong>C.</strong> Purchase 80 spot instances. Use Auto Scaling Group to provision the remaining instances as on-demand instances per the workload demand</label><br>
<label for="q98-d"><input type="radio" id="q98-d" name="q98" value="D"> <strong>D.</strong> Purchase 80 on-demand instances. Provision additional on-demand and spot instances per the workload demand (Use Auto Scaling Group with launch template to provision the mix of on-demand and spot instances)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Purchase 80 reserved instances (RIs). Provision additional on-demand and spot instances per the workload demand (Use Auto Scaling Group with launch template to provision the mix of on-demand and spot instances)

</details>

---

## Câu 99

**Chủ đề:** Design High-Performing Architectures

A big data consulting firm needs to set up a data lake on Amazon S3 for a Health-Care client. The data lake is split in raw and refined zones. For compliance reasons, the source data needs to be kept for a minimum of 5 years. The source data arrives in the raw zone and is then processed via an AWS Glue based extract, transform, and load (ETL) job into the refined zone. The business analysts run ad-hoc queries only on the data in the refined zone using Amazon Athena. The team is concerned about the cost of data storage in both the raw and refined zones as the data is increasing at a rate of 1 terabyte daily in each zone.

As a solutions architect, which of the following would you recommend as the MOST cost-optimal solution? (Select two)

**Lựa chọn:**

<label for="q99-a"><input type="checkbox" id="q99-a" name="q99" value="A"> <strong>A.</strong> Setup a lifecycle policy to transition the raw zone data into Amazon S3 Glacier Deep Archive after 1 day of object creation</label><br>
<label for="q99-b"><input type="checkbox" id="q99-b" name="q99" value="B"> <strong>B.</strong> Create an AWS Lambda function based job to delete the raw zone data after 1 day</label><br>
<label for="q99-c"><input type="checkbox" id="q99-c" name="q99" value="C"> <strong>C.</strong> Setup a lifecycle policy to transition the refined zone data into Amazon S3 Glacier Deep Archive after 1 day of object creation</label><br>
<label for="q99-d"><input type="checkbox" id="q99-d" name="q99" value="D"> <strong>D.</strong> Use AWS Glue ETL job to write the transformed data in the refined zone using CSV format</label><br>
<label for="q99-e"><input type="checkbox" id="q99-e" name="q99" value="E"> <strong>E.</strong> Use AWS Glue ETL job to write the transformed data in the refined zone using a compressed file format</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Setup a lifecycle policy to transition the raw zone data into Amazon S3 Glacier Deep Archive after 1 day of object creation

E. Use AWS Glue ETL job to write the transformed data in the refined zone using a compressed file format

</details>

---

## Câu 100

**Chủ đề:** Design Cost-Optimized Architectures

An IT company wants to optimize the costs incurred on its fleet of 100 Amazon EC2 instances for the next year. Based on historical analyses, the engineering team observed that 70 of these instances handle the compute services of its flagship application and need to be always available. The other 30 instances are used to handle batch jobs that can afford a delay in processing.

As a solutions architect, which of the following would you recommend as the MOST cost-optimal solution?

**Lựa chọn:**

<label for="q100-a"><input type="radio" id="q100-a" name="q100" value="A"> <strong>A.</strong> Purchase 70 reserved instances (RIs) and 30 spot instances</label><br>
<label for="q100-b"><input type="radio" id="q100-b" name="q100" value="B"> <strong>B.</strong> Purchase 70 on-demand instances and 30 spot instances</label><br>
<label for="q100-c"><input type="radio" id="q100-c" name="q100" value="C"> <strong>C.</strong> Purchase 70 reserved instances and 30 on-demand instances</label><br>
<label for="q100-d"><input type="radio" id="q100-d" name="q100" value="D"> <strong>D.</strong> Purchase 70 on-demand instances and 30 reserved instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Purchase 70 reserved instances (RIs) and 30 spot instances

</details>

---

## Câu 101

**Chủ đề:** Design Cost-Optimized Architectures

You have multiple AWS accounts within a single AWS Region managed by AWS Organizations and you would like to ensure all Amazon EC2 instances in all these accounts can communicate privately. Which of the following solutions provides the capability at the CHEAPEST cost?

**Lựa chọn:**

<label for="q101-a"><input type="radio" id="q101-a" name="q101" value="A"> <strong>A.</strong> Create a virtual private cloud (VPC) in an account and share one or more of its subnets with the other accounts using Resource Access Manager</label><br>
<label for="q101-b"><input type="radio" id="q101-b" name="q101" value="B"> <strong>B.</strong> Create an AWS Transit Gateway and link all the virtual private cloud (VPCs) in all the accounts together</label><br>
<label for="q101-c"><input type="radio" id="q101-c" name="q101" value="C"> <strong>C.</strong> Create a VPC peering connection between all virtual private cloud (VPCs)</label><br>
<label for="q101-d"><input type="radio" id="q101-d" name="q101" value="D"> <strong>D.</strong> Create a Private Link between all the Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a virtual private cloud (VPC) in an account and share one or more of its subnets with the other accounts using Resource Access Manager

</details>

---

## Câu 102

**Chủ đề:** Design Secure Architectures

What does this IAM policy do?

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Mystery Policy",
      "Action": [
        "ec2:RunInstances"
      ],
      "Effect": "Allow",
      "Resource": "*",
      "Condition": {
        "IpAddress": {
          "aws:SourceIp": "34.50.31.0/24"
        }
      }
    }
  ]
}

**Lựa chọn:**

<label for="q102-a"><input type="radio" id="q102-a" name="q102" value="A"> <strong>A.</strong> It allows starting an Amazon EC2 instance only when the IP where the call originates is within the 34.50.31.0/24 CIDR block</label><br>
<label for="q102-b"><input type="radio" id="q102-b" name="q102" value="B"> <strong>B.</strong> It allows starting an Amazon EC2 instance only when they have a Public IP within the 34.50.31.0/24 CIDR block</label><br>
<label for="q102-c"><input type="radio" id="q102-c" name="q102" value="C"> <strong>C.</strong> It allows starting an Amazon EC2 instance only when they have an Elastic IP within the 34.50.31.0/24 CIDR block</label><br>
<label for="q102-d"><input type="radio" id="q102-d" name="q102" value="D"> <strong>D.</strong> It allows starting an Amazon EC2 instance only when they have a Private IP within the 34.50.31.0/24 CIDR block</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. It allows starting an Amazon EC2 instance only when the IP where the call originates is within the 34.50.31.0/24 CIDR block

</details>

---

## Câu 103

**Chủ đề:** Design Secure Architectures

What does this IAM policy do?

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Mystery Policy",
      "Action": [
        "ec2:RunInstances"
      ],
      "Effect": "Allow",
      "Resource": "*",
      "Condition": {
        "StringEquals": {
          "aws:RequestedRegion": "eu-west-1"
        }
      }
    }
  ]
}

**Lựa chọn:**

<label for="q103-a"><input type="radio" id="q103-a" name="q103" value="A"> <strong>A.</strong> It allows running Amazon EC2 instances only in the eu-west-1 region, and the API call can be made from anywhere in the world</label><br>
<label for="q103-b"><input type="radio" id="q103-b" name="q103" value="B"> <strong>B.</strong> It allows running Amazon EC2 instances anywhere but in the eu-west-1 region</label><br>
<label for="q103-c"><input type="radio" id="q103-c" name="q103" value="C"> <strong>C.</strong> It allows running Amazon EC2 instances in any region when the API call is originating from the eu-west-1 region</label><br>
<label for="q103-d"><input type="radio" id="q103-d" name="q103" value="D"> <strong>D.</strong> It allows running Amazon EC2 instances in the eu-west-1 region, when the API call is made from the eu-west-1 region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. It allows running Amazon EC2 instances only in the eu-west-1 region, and the API call can be made from anywhere in the world

</details>

---

## Câu 104

**Chủ đề:** Design Secure Architectures

You have a team of developers in your company, and you would like to ensure they can quickly experiment with AWS Managed Policies by attaching them to their accounts, but you would like to prevent them from doing an escalation of privileges, by granting themselves the AdministratorAccess managed policy. How should you proceed?

**Lựa chọn:**

<label for="q104-a"><input type="radio" id="q104-a" name="q104" value="A"> <strong>A.</strong> For each developer, define an IAM permission boundary that will restrict the managed policies they can attach to themselves</label><br>
<label for="q104-b"><input type="radio" id="q104-b" name="q104" value="B"> <strong>B.</strong> Put the developers into an IAM group, and then define an IAM permission boundary on the group that will restrict the managed policies they can attach to themselves</label><br>
<label for="q104-c"><input type="radio" id="q104-c" name="q104" value="C"> <strong>C.</strong> Create a Service Control Policy (SCP) on your AWS account that restricts developers from attaching themselves the AdministratorAccess policy</label><br>
<label for="q104-d"><input type="radio" id="q104-d" name="q104" value="D"> <strong>D.</strong> Attach an IAM policy to your developers, that prevents them from attaching the AdministratorAccess policy</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. For each developer, define an IAM permission boundary that will restrict the managed policies they can attach to themselves

</details>

---

## Câu 105

**Chủ đề:** Design Secure Architectures

A financial institution is transitioning its critical back-office systems to AWS. These systems currently rely on Microsoft SQL Server databases hosted on on-premises infrastructure. The data is highly sensitive and subject to regulatory compliance. The organization wants to enhance security and minimize database management tasks as part of the migration.

Which solution will best meet these goals with the least operational burden?

**Lựa chọn:**

<label for="q105-a"><input type="radio" id="q105-a" name="q105" value="A"> <strong>A.</strong> Migrate the SQL Server databases to a Multi-AZ Amazon RDS for SQL Server deployment. Enable encryption at rest by using an AWS Key Management Service (AWS KMS) managed key</label><br>
<label for="q105-b"><input type="radio" id="q105-b" name="q105" value="B"> <strong>B.</strong> Migrate the SQL Server databases to Amazon EC2 instances with encrypted EBS volumes. Use an AWS KMS customer managed key to enable encryption</label><br>
<label for="q105-c"><input type="radio" id="q105-c" name="q105" value="C"> <strong>C.</strong> Export the SQL Server databases to CSV format and store them in Amazon S3 with S3 bucket policies for access control. Use AWS Backup for data protection</label><br>
<label for="q105-d"><input type="radio" id="q105-d" name="q105" value="D"> <strong>D.</strong> Move the SQL Server data into Amazon Timestream to gain time series insights. Use AWS CloudTrail to monitor access to the data</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Migrate the SQL Server databases to a Multi-AZ Amazon RDS for SQL Server deployment. Enable encryption at rest by using an AWS Key Management Service (AWS KMS) managed key

</details>

---

## Câu 106

**Chủ đề:** Design Cost-Optimized Architectures

You would like to use AWS Snowball to move on-premises backups into a long term archival tier on AWS. Which solution provides the MOST cost savings?

**Lựa chọn:**

<label for="q106-a"><input type="radio" id="q106-a" name="q106" value="A"> <strong>A.</strong> Create an AWS Snowball job and target an Amazon S3 bucket. Create a lifecycle policy to transition this data to Amazon S3 Glacier Deep Archive on the same day</label><br>
<label for="q106-b"><input type="radio" id="q106-b" name="q106" value="B"> <strong>B.</strong> Create an AWS Snowball job and target a Amazon S3 Glacier Vault</label><br>
<label for="q106-c"><input type="radio" id="q106-c" name="q106" value="C"> <strong>C.</strong> Create an AWS Snowball job and target an Amazon S3 bucket. Create a lifecycle policy to transition this data to Amazon S3 Glacier on the same day</label><br>
<label for="q106-d"><input type="radio" id="q106-d" name="q106" value="D"> <strong>D.</strong> Create a AWS Snowball job and target an Amazon S3 Glacier Deep Archive Vault</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an AWS Snowball job and target an Amazon S3 bucket. Create a lifecycle policy to transition this data to Amazon S3 Glacier Deep Archive on the same day

</details>

---

## Câu 107

**Chủ đề:** Design High-Performing Architectures

You are establishing a monitoring solution for desktop systems, that will be sending telemetry data into AWS every 1 minute. Data for each system must be processed in order, independently, and you would like to scale the number of consumers to be possibly equal to the number of desktop systems that are being monitored.

What do you recommend?

**Lựa chọn:**

<label for="q107-a"><input type="radio" id="q107-a" name="q107" value="A"> <strong>A.</strong> Use an Amazon Simple Queue Service (Amazon SQS) FIFO (First-In-First-Out) queue, and make sure the telemetry data is sent with a Group ID attribute representing the value of the Desktop ID</label><br>
<label for="q107-b"><input type="radio" id="q107-b" name="q107" value="B"> <strong>B.</strong> Use an Amazon Simple Queue Service (Amazon SQS) FIFO (First-In-First-Out) queue, and send the telemetry data as is</label><br>
<label for="q107-c"><input type="radio" id="q107-c" name="q107" value="C"> <strong>C.</strong> Use an Amazon Simple Queue Service (Amazon SQS) standard queue, and send the telemetry data as is</label><br>
<label for="q107-d"><input type="radio" id="q107-d" name="q107" value="D"> <strong>D.</strong> Use an Amazon Kinesis Data Stream, and send the telemetry data with a Partition ID that uses the value of the Desktop ID</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use an Amazon Simple Queue Service (Amazon SQS) FIFO (First-In-First-Out) queue, and make sure the telemetry data is sent with a Group ID attribute representing the value of the Desktop ID

</details>

---

## Câu 108

**Chủ đề:** Design Secure Architectures

A security consultant is designing a solution for a company that wants to provide developers with individual AWS accounts through AWS Organizations, while also maintaining standard security controls. Since the individual developers will have AWS account root user-level access to their own accounts, the consultant wants to ensure that the mandatory AWS CloudTrail configuration that is applied to new developer accounts is not modified.

Which of the following actions meets the given requirements?

**Lựa chọn:**

<label for="q108-a"><input type="radio" id="q108-a" name="q108" value="A"> <strong>A.</strong> Configure a new trail in AWS CloudTrail from within the developer accounts with the organization trails option enabled</label><br>
<label for="q108-b"><input type="radio" id="q108-b" name="q108" value="B"> <strong>B.</strong> Set up a service control policy (SCP) that prohibits changes to AWS CloudTrail, and attach it to the developer accounts</label><br>
<label for="q108-c"><input type="radio" id="q108-c" name="q108" value="C"> <strong>C.</strong> Set up an IAM policy that prohibits changes to AWS CloudTrail and attach it to the root user</label><br>
<label for="q108-d"><input type="radio" id="q108-d" name="q108" value="D"> <strong>D.</strong> Set up a service-linked role for AWS CloudTrail with a policy condition that allows changes only from an Amazon Resource Name (ARN) in the master account</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up a service control policy (SCP) that prohibits changes to AWS CloudTrail, and attach it to the developer accounts

</details>

---

## Câu 109

**Chủ đề:** Design Secure Architectures

"An enterprise organization is expanding its cloud footprint and needs to centralize its security event data from various AWS accounts and services. The goal is to evaluate security posture across all environments and improve threat detection and response — without requiring significant custom code or manual integration.

Which solution will fulfill these needs with the least development effort?

**Lựa chọn:**

<label for="q109-a"><input type="radio" id="q109-a" name="q109" value="A"> <strong>A.</strong> Use Amazon Security Lake to create a centralized data lake that automatically collects security-related logs and events from AWS services and third-party sources. Store the data in an Amazon S3 bucket managed by Security Lake</label><br>
<label for="q109-b"><input type="radio" id="q109-b" name="q109" value="B"> <strong>B.</strong> Deploy a custom Lambda function to aggregate security logs from multiple AWS accounts. Format the data into CSV files and upload them to a central S3 bucket for analysis</label><br>
<label for="q109-c"><input type="radio" id="q109-c" name="q109" value="C"> <strong>C.</strong> Use Amazon Athena with predefined SQL queries to scan security logs stored in multiple S3 buckets. Visualize the findings by exporting results to an Amazon QuickSight dashboard</label><br>
<label for="q109-d"><input type="radio" id="q109-d" name="q109" value="D"> <strong>D.</strong> Set up a data lake using AWS Lake Formation to collect and organize security event logs. Use AWS Glue to perform ETL operations and standardize the log formats for centralized analysis</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon Security Lake to create a centralized data lake that automatically collects security-related logs and events from AWS services and third-party sources. Store the data in an Amazon S3 bucket managed by Security Lake

</details>

---

## Câu 110

**Chủ đề:** Design Secure Architectures

Upon a security review of your AWS account, an AWS consultant has found that a few Amazon RDS databases are unencrypted. As a Solutions Architect, what steps must be taken to encrypt the Amazon RDS databases?

**Lựa chọn:**

<label for="q110-a"><input type="radio" id="q110-a" name="q110" value="A"> <strong>A.</strong> Take a snapshot of the database, copy it as an encrypted snapshot, and restore a database from the encrypted snapshot. Terminate the previous database</label><br>
<label for="q110-b"><input type="radio" id="q110-b" name="q110" value="B"> <strong>B.</strong> Create a Read Replica of the database, and encrypt the read replica. Promote the read replica as a standalone database, and terminate the previous database</label><br>
<label for="q110-c"><input type="radio" id="q110-c" name="q110" value="C"> <strong>C.</strong> Enable Multi-AZ for the database, and make sure the standby instance is encrypted. Stop the main database to that the standby database kicks in, then disable Multi-AZ</label><br>
<label for="q110-d"><input type="radio" id="q110-d" name="q110" value="D"> <strong>D.</strong> Enable encryption on the Amazon RDS database using the AWS Console</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Take a snapshot of the database, copy it as an encrypted snapshot, and restore a database from the encrypted snapshot. Terminate the previous database

</details>

---

## Câu 111

**Chủ đề:** Design Secure Architectures

A company has historically operated only in the us-east-1 region and stores encrypted data in Amazon S3 using SSE-KMS. As part of enhancing its security posture as well as improving the backup and recovery architecture, the company wants to store the encrypted data in Amazon S3 that is replicated into the us-west-1 AWS region. The security policies mandate that the data must be encrypted and decrypted using the same key in both AWS regions.

Which of the following represents the best solution to address these requirements?

**Lựa chọn:**

<label for="q111-a"><input type="radio" id="q111-a" name="q111" value="A"> <strong>A.</strong> Create an Amazon CloudWatch scheduled rule to invoke an AWS Lambda function to copy the daily data from the source bucket in us-east-1 region to the destination bucket in us-west-1 region. Provide AWS KMS key access to the AWS Lambda function for encryption and decryption operations on the data in the source and destination Amazon S3 buckets</label><br>
<label for="q111-b"><input type="radio" id="q111-b" name="q111" value="B"> <strong>B.</strong> Create a new Amazon S3 bucket in the us-east-1 region with replication enabled from this new bucket into another bucket in us-west-1 region. Enable SSE-KMS encryption on the new bucket in us-east-1 region by using an AWS KMS multi-region key. Copy the existing data from the current Amazon S3 bucket in us-east-1 region into this new Amazon S3 bucket in us-east-1 region</label><br>
<label for="q111-c"><input type="radio" id="q111-c" name="q111" value="C"> <strong>C.</strong> Change the AWS KMS single region key used for the current Amazon S3 bucket into an AWS KMS multi-region key. Enable Amazon S3 batch replication for the existing data in the current bucket in us-east-1 region into another bucket in us-west-1 region</label><br>
<label for="q111-d"><input type="radio" id="q111-d" name="q111" value="D"> <strong>D.</strong> Enable replication for the current bucket in us-east-1 region into another bucket in us-west-1 region. Share the existing AWS KMS key from us-east-1 region to us-west-1 region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create a new Amazon S3 bucket in the us-east-1 region with replication enabled from this new bucket into another bucket in us-west-1 region. Enable SSE-KMS encryption on the new bucket in us-east-1 region by using an AWS KMS multi-region key. Copy the existing data from the current Amazon S3 bucket in us-east-1 region into this new Amazon S3 bucket in us-east-1 region

</details>

---

## Câu 112

**Chủ đề:** Design Resilient Architectures

A wildlife research organization uses IoT-based motion sensors attached to thousands of migrating animals to monitor their movement across regions. Every few minutes, a sensor checks for significant movement and sends updated location data to a backend application running on Amazon EC2 instances spread across multiple Availability Zones in a single AWS Region. Recently, an unexpected surge in motion data overwhelmed the application, leading to lost location records with no mechanism to replay missed data. A solutions architect must redesign the ingestion mechanism to prevent future data loss and to minimize operational overhead.

What should the solutions architect do to meet these requirements?

**Lựa chọn:**

<label for="q112-a"><input type="radio" id="q112-a" name="q112" value="A"> <strong>A.</strong> Create an Amazon Simple Queue Service (Amazon SQS) queue to buffer the incoming location data. Configure the backend application to poll the queue and process messages</label><br>
<label for="q112-b"><input type="radio" id="q112-b" name="q112" value="B"> <strong>B.</strong> Set up a containerized service using Amazon ECS with an internal queue built into the application layer. Configure the motion sensors to send location updates directly to the container endpoints</label><br>
<label for="q112-c"><input type="radio" id="q112-c" name="q112" value="C"> <strong>C.</strong> Deploy an Amazon Data Firehose delivery stream to collect the motion data. Configure it to deliver data to an S3 bucket where the application scans and processes the files periodically</label><br>
<label for="q112-d"><input type="radio" id="q112-d" name="q112" value="D"> <strong>D.</strong> Implement an AWS IoT Core rule to route location updates directly from each sensor to Amazon SNS. Configure the application to poll the SNS topic for new messages</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an Amazon Simple Queue Service (Amazon SQS) queue to buffer the incoming location data. Configure the backend application to poll the queue and process messages

</details>

---

## Câu 113

**Chủ đề:** Design Secure Architectures

Consider the following policy associated with an IAM group containing several users:

{
    "Version":"2012-10-17",
    "Id":"EC2TerminationPolicy",
    "Statement":[
        {
            "Effect":"Deny",
            "Action":"ec2:*",
            "Resource":"*",
            "Condition":{
                "StringNotEquals":{
                    "ec2:Region":"us-west-1"
                }
            }
        },
        {
            "Effect":"Allow",
            "Action":"ec2:TerminateInstances",
            "Resource":"*",
            "Condition":{
                "IpAddress":{
                    "aws:SourceIp":"10.200.200.0/24"
                }
            }
        }
    ]
}

Which of the following options is correct?

**Lựa chọn:**

<label for="q113-a"><input type="radio" id="q113-a" name="q113" value="A"> <strong>A.</strong> Users belonging to the IAM user group can terminate an Amazon EC2 instance in the us-west-1 region when the user's source IP is 10.200.200.200</label><br>
<label for="q113-b"><input type="radio" id="q113-b" name="q113" value="B"> <strong>B.</strong> Users belonging to the IAM user group cannot terminate an Amazon EC2 instance in the us-west-1 region when the user's source IP is 10.200.200.200</label><br>
<label for="q113-c"><input type="radio" id="q113-c" name="q113" value="C"> <strong>C.</strong> Users belonging to the IAM user group can terminate an Amazon EC2 instance in the us-west-1 region when the EC2 instance's IP address is 10.200.200.200</label><br>
<label for="q113-d"><input type="radio" id="q113-d" name="q113" value="D"> <strong>D.</strong> Users belonging to the IAM user group can terminate an Amazon EC2 instance belonging to any region except the us-west-1 region when the user's source IP is 10.200.200.200</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Users belonging to the IAM user group can terminate an Amazon EC2 instance in the us-west-1 region when the user's source IP is 10.200.200.200

</details>

---

## Câu 114

**Chủ đề:** Design Cost-Optimized Architectures

Your company has a monthly big data workload, running for about 2 hours, which can be efficiently distributed across multiple servers of various sizes, with a variable number of CPUs. The solution for the workload should be able to withstand server failures.

Which is the MOST cost-optimal solution for this workload?

**Lựa chọn:**

<label for="q114-a"><input type="radio" id="q114-a" name="q114" value="A"> <strong>A.</strong> Run the workload on a Spot Fleet</label><br>
<label for="q114-b"><input type="radio" id="q114-b" name="q114" value="B"> <strong>B.</strong> Run the workload on Spot Instances</label><br>
<label for="q114-c"><input type="radio" id="q114-c" name="q114" value="C"> <strong>C.</strong> Run the workload on Reserved Instances (RI)</label><br>
<label for="q114-d"><input type="radio" id="q114-d" name="q114" value="D"> <strong>D.</strong> Run the workload on Dedicated Hosts</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Run the workload on a Spot Fleet

</details>

---

## Câu 115

**Chủ đề:** Design Secure Architectures

A financial services company wants to store confidential data in Amazon S3 and it needs to meet the following data security and compliance norms:

Encryption key usage must be logged for auditing purposes
Encryption Keys must be rotated every year
The data must be encrypted at rest

Which is the MOST operationally efficient solution?

**Lựa chọn:**

<label for="q115-a"><input type="radio" id="q115-a" name="q115" value="A"> <strong>A.</strong> Server-side encryption (SSE-S3) with automatic key rotation</label><br>
<label for="q115-b"><input type="radio" id="q115-b" name="q115" value="B"> <strong>B.</strong> Server-side encryption with AWS Key Management Service (AWS KMS) keys (SSE-KMS) with automatic key rotation</label><br>
<label for="q115-c"><input type="radio" id="q115-c" name="q115" value="C"> <strong>C.</strong> Server-side encryption with AWS Key Management Service (AWS KMS) keys (SSE-KMS) with manual key rotation</label><br>
<label for="q115-d"><input type="radio" id="q115-d" name="q115" value="D"> <strong>D.</strong> Server-side encryption with customer-provided keys (SSE-C) with automatic key rotation</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Server-side encryption with AWS Key Management Service (AWS KMS) keys (SSE-KMS) with automatic key rotation

</details>

---

## Câu 116

**Chủ đề:** Design High-Performing Architectures

A Machine Learning research group uses a proprietary computer vision application hosted on an Amazon EC2 instance. Every time the instance needs to be stopped and started again, the application takes about 3 minutes to start as some auxiliary software programs need to be executed so that the application can function. The research group would like to minimize the application boostrap time whenever the system needs to be stopped and then started at a later point in time.

As a solutions architect, which of the following solutions would you recommend for this use-case?

**Lựa chọn:**

<label for="q116-a"><input type="radio" id="q116-a" name="q116" value="A"> <strong>A.</strong> Use Amazon EC2 Instance Hibernate</label><br>
<label for="q116-b"><input type="radio" id="q116-b" name="q116" value="B"> <strong>B.</strong> Use Amazon EC2 User-Data</label><br>
<label for="q116-c"><input type="radio" id="q116-c" name="q116" value="C"> <strong>C.</strong> Use Amazon EC2 Meta-Data</label><br>
<label for="q116-d"><input type="radio" id="q116-d" name="q116" value="D"> <strong>D.</strong> Create an Amazon Machine Image (AMI) and launch your Amazon EC2 instances from that</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon EC2 Instance Hibernate

</details>

---

## Câu 117

**Chủ đề:** Design Resilient Architectures

A media company is migrating its flagship application from its on-premises data center to AWS for improving the application's read-scaling capability as well as its availability. The existing architecture leverages a Microsoft SQL Server database that sees a heavy read load. The engineering team does a full copy of the production database at the start of the business day to populate a dev database. During this period, application users face high latency leading to a bad user experience.

The company is looking at alternate database options and migrating database engines if required. What would you suggest?

**Lựa chọn:**

<label for="q117-a"><input type="radio" id="q117-a" name="q117" value="A"> <strong>A.</strong> Leverage Amazon RDS for MySQL with a Multi-AZ deployment and use the standby instance as the dev database</label><br>
<label for="q117-b"><input type="radio" id="q117-b" name="q117" value="B"> <strong>B.</strong> Leverage Amazon RDS for SQL server with a Multi-AZ deployment and read replicas. Use the read replica as the dev database</label><br>
<label for="q117-c"><input type="radio" id="q117-c" name="q117" value="C"> <strong>C.</strong> Leverage Amazon Aurora MySQL with Multi-AZ Aurora Replicas and create the dev database by restoring from the automated backups of Amazon Aurora</label><br>
<label for="q117-d"><input type="radio" id="q117-d" name="q117" value="D"> <strong>D.</strong> Leverage Amazon Aurora MySQL with Multi-AZ Aurora Replicas and restore the dev database via mysqldump</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Leverage Amazon Aurora MySQL with Multi-AZ Aurora Replicas and create the dev database by restoring from the automated backups of Amazon Aurora

</details>

---

## Câu 118

**Chủ đề:** Design Resilient Architectures

A media publishing company is migrating its legacy content management application to AWS. Currently, the application and its MySQL database run on a single on-premises virtual machine, which creates a single point of failure and limits scalability. As traffic has increased due to growing reader engagement and video uploads, the company needs to redesign the solution to ensure automatic scaling, high availability, and separation of application and database layers. The company wants to continue using a MySQL-compatible engine and needs a cost-effective, managed solution that minimizes operational overhead.

Which AWS architecture will best fulfill these requirements?

**Lựa chọn:**

<label for="q118-a"><input type="radio" id="q118-a" name="q118" value="A"> <strong>A.</strong> Migrate the application to Amazon EC2 instances in an Auto Scaling group behind an Application Load Balancer. Use Amazon Aurora Serverless v2 for MySQL to manage the database layer with auto-scaling and built-in high availability</label><br>
<label for="q118-b"><input type="radio" id="q118-b" name="q118" value="B"> <strong>B.</strong> Deploy the application to EC2 instances registered in a Network Load Balancer target group. Use Amazon ElastiCache for Redis as the database and configure it with Redis Streams for persistent storage</label><br>
<label for="q118-c"><input type="radio" id="q118-c" name="q118" value="C"> <strong>C.</strong> Containerize the application and deploy it to Amazon ECS with EC2 launch type behind an Application Load Balancer. Use Amazon Neptune to store structured relational data with SQL-like queries</label><br>
<label for="q118-d"><input type="radio" id="q118-d" name="q118" value="D"> <strong>D.</strong> Host the application on EC2 instances that are part of a target group for an Application Load Balancer. Create an Amazon RDS for MySQL Multi-AZ DB instance to provide high availability and automatic failover for the database</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Migrate the application to Amazon EC2 instances in an Auto Scaling group behind an Application Load Balancer. Use Amazon Aurora Serverless v2 for MySQL to manage the database layer with auto-scaling and built-in high availability

</details>

---

## Câu 119

**Chủ đề:** Design Secure Architectures

Which of the following IAM policies provides read-only access to the Amazon S3 bucket mybucket and its content?

**Lựa chọn:**

<label for="q119-a"><input type="radio" id="q119-a" name="q119" value="A"> <strong>A.</strong> {
   "Version":"2012-10-17",
   "Statement":[
      {
         "Effect":"Allow",
         "Action":[
            "s3:ListBucket"
         ],
         "Resource":"arn:aws:s3:::mybucket"
      },
      {
         "Effect":"Allow",
         "Action":[
            "s3:GetObject"
         ],
         "Resource":"arn:aws:s3:::mybucket/*"
      }
   ]
}</label><br>
<label for="q119-b"><input type="radio" id="q119-b" name="q119" value="B"> <strong>B.</strong> {
   "Version":"2012-10-17",
   "Statement":[
      {
         "Effect":"Allow",
         "Action":[
            "s3:ListBucket",
            "s3:GetObject"
         ],
         "Resource":"arn:aws:s3:::mybucket"
      }
   ]
}</label><br>
<label for="q119-c"><input type="radio" id="q119-c" name="q119" value="C"> <strong>C.</strong> {
   "Version":"2012-10-17",
   "Statement":[
      {
         "Effect":"Allow",
         "Action":[
            "s3:ListBucket",
            "s3:GetObject"
         ],
         "Resource":"arn:aws:s3:::mybucket/*"
      }
   ]
}</label><br>
<label for="q119-d"><input type="radio" id="q119-d" name="q119" value="D"> <strong>D.</strong> {
   "Version":"2012-10-17",
   "Statement":[
      {
         "Effect":"Allow",
         "Action":[
            "s3:ListBucket"
         ],
         "Resource":"arn:aws:s3:::mybucket/*"
      },
      {
         "Effect":"Allow",
         "Action":[
            "s3:GetObject"
         ],
         "Resource":"arn:aws:s3:::mybucket"
      }
   ]
}</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. {
   "Version":"2012-10-17",
   "Statement":[
      {
         "Effect":"Allow",
         "Action":[
            "s3:ListBucket"
         ],
         "Resource":"arn:aws:s3:::mybucket"
      },
      {
         "Effect":"Allow",
         "Action":[
            "s3:GetObject"
         ],
         "Resource":"arn:aws:s3:::mybucket/*"
      }
   ]
}

</details>

---

## Câu 120

**Chủ đề:** Design Secure Architectures

An HTTP application is deployed on an Auto Scaling Group, is accessible from an Application Load Balancer (ALB) that provides HTTPS termination, and accesses a PostgreSQL database managed by Amazon RDS.

How should you configure the security groups? (Select three)

**Lựa chọn:**

<label for="q120-a"><input type="checkbox" id="q120-a" name="q120" value="A"> <strong>A.</strong> The security group of Amazon RDS should have an inbound rule from the security group of the Amazon EC2 instances in the Auto Scaling group on port 5432</label><br>
<label for="q120-b"><input type="checkbox" id="q120-b" name="q120" value="B"> <strong>B.</strong> The security group of the Amazon EC2 instances should have an inbound rule from the security group of the Application Load Balancer on port 80</label><br>
<label for="q120-c"><input type="checkbox" id="q120-c" name="q120" value="C"> <strong>C.</strong> The security group of the Application Load Balancer should have an inbound rule from anywhere on port 443</label><br>
<label for="q120-d"><input type="checkbox" id="q120-d" name="q120" value="D"> <strong>D.</strong> The security group of the Application Load Balancer should have an inbound rule from anywhere on port 80</label><br>
<label for="q120-e"><input type="checkbox" id="q120-e" name="q120" value="E"> <strong>E.</strong> The security group of the Amazon EC2 instances should have an inbound rule from the security group of the Amazon RDS database on port 5432</label><br>
<label for="q120-f"><input type="checkbox" id="q120-f" name="q120" value="F"> <strong>F.</strong> The security group of Amazon RDS should have an inbound rule from the security group of the Amazon EC2 instances in the Auto Scaling group on port 80</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The security group of Amazon RDS should have an inbound rule from the security group of the Amazon EC2 instances in the Auto Scaling group on port 5432

B. The security group of the Amazon EC2 instances should have an inbound rule from the security group of the Application Load Balancer on port 80

C. The security group of the Application Load Balancer should have an inbound rule from anywhere on port 443

</details>

---

## Câu 121

**Chủ đề:** Design High-Performing Architectures

Your company has an on-premises Distributed File System Replication (DFSR) service to keep files synchronized on multiple Windows servers, and would like to migrate to AWS cloud.

What do you recommend as a replacement for the DFSR?

**Lựa chọn:**

<label for="q121-a"><input type="radio" id="q121-a" name="q121" value="A"> <strong>A.</strong> Amazon FSx for Windows File Server</label><br>
<label for="q121-b"><input type="radio" id="q121-b" name="q121" value="B"> <strong>B.</strong> Amazon FSx for Lustre</label><br>
<label for="q121-c"><input type="radio" id="q121-c" name="q121" value="C"> <strong>C.</strong> Amazon Elastic File System (Amazon EFS)</label><br>
<label for="q121-d"><input type="radio" id="q121-d" name="q121" value="D"> <strong>D.</strong> Amazon Simple Storage Service (Amazon S3)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon FSx for Windows File Server

</details>

---

## Câu 122

**Chủ đề:** Design Secure Architectures

A retail company wants to share sensitive accounting data that is stored in an Amazon RDS database instance with an external auditor. The auditor has its own AWS account and needs its own copy of the database.

Which of the following would you recommend to securely share the database with the auditor?

**Lựa chọn:**

<label for="q122-a"><input type="radio" id="q122-a" name="q122" value="A"> <strong>A.</strong> Create an encrypted snapshot of the database, share the snapshot, and allow access to the AWS Key Management Service (AWS KMS) encryption key</label><br>
<label for="q122-b"><input type="radio" id="q122-b" name="q122" value="B"> <strong>B.</strong> Create a snapshot of the database in Amazon S3 and assign an IAM role to the auditor to grant access to the object in that bucket</label><br>
<label for="q122-c"><input type="radio" id="q122-c" name="q122" value="C"> <strong>C.</strong> Export the database contents to text files, store the files in Amazon S3, and create a new IAM user for the auditor with access to that bucket</label><br>
<label for="q122-d"><input type="radio" id="q122-d" name="q122" value="D"> <strong>D.</strong> Set up a read replica of the database and configure IAM standard database authentication to grant the auditor access</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an encrypted snapshot of the database, share the snapshot, and allow access to the AWS Key Management Service (AWS KMS) encryption key

</details>

---

## Câu 123

**Chủ đề:** Design Secure Architectures

An enterprise is building a secure business intelligence API using Amazon API Gateway to serve internal users with confidential analytics data. The API must be accessible only from a set of trusted IP addresses that are part of the organization's internal network ranges. No external IP traffic should be able to invoke the API. A solutions architect must design this access control mechanism with the least operational complexity.

What should the architect do to meet these requirements?

**Lựa chọn:**

<label for="q123-a"><input type="radio" id="q123-a" name="q123" value="A"> <strong>A.</strong> Create a resource policy for the API Gateway API that explicitly denies access to all IP addresses except those listed in an allow list</label><br>
<label for="q123-b"><input type="radio" id="q123-b" name="q123" value="B"> <strong>B.</strong> Deploy the API Gateway as a regional API in a public subnet and associate the subnet with a security group that permits inbound traffic only from trusted IP ranges</label><br>
<label for="q123-c"><input type="radio" id="q123-c" name="q123" value="C"> <strong>C.</strong> Deploy the API Gateway resource to an on-premises server using AWS Outposts. Apply host-based firewall rules to filter allowed IPs</label><br>
<label for="q123-d"><input type="radio" id="q123-d" name="q123" value="D"> <strong>D.</strong> Modify the security group that is attached to API Gateway to allow only traffic from specific IP addresses</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a resource policy for the API Gateway API that explicitly denies access to all IP addresses except those listed in an allow list

</details>

---

## Câu 124

**Chủ đề:** Design Resilient Architectures

A manufacturing company receives unreliable service from its data center provider because the company is located in an area prone to natural disasters. The company is not ready to fully migrate to the AWS Cloud, but it wants a failover environment on AWS in case the on-premises data center fails. The company runs web servers that connect to external vendors. The data available on AWS and on-premises must be uniform.

Which of the following solutions would have the LEAST amount of downtime?

**Lựa chọn:**

<label for="q124-a"><input type="radio" id="q124-a" name="q124" value="A"> <strong>A.</strong> Set up a Amazon Route 53 failover record. Execute an AWS CloudFormation template from a script to provision Amazon EC2 instances behind an Application Load Balancer. Set up AWS Storage Gateway with stored volumes to back up data to Amazon S3</label><br>
<label for="q124-b"><input type="radio" id="q124-b" name="q124" value="B"> <strong>B.</strong> Set up a Amazon Route 53 failover record. Run application servers on Amazon EC2 instances behind an Application Load Balancer in an Auto Scaling group. Set up AWS Storage Gateway with stored volumes to back up data to Amazon S3</label><br>
<label for="q124-c"><input type="radio" id="q124-c" name="q124" value="C"> <strong>C.</strong> Set up a Amazon Route 53 failover record. Set up an AWS Direct Connect connection between a VPC and the data center. Run application servers on Amazon EC2 in an Auto Scaling group. Run an AWS Lambda function to execute an AWS CloudFormation template to create an Application Load Balancer</label><br>
<label for="q124-d"><input type="radio" id="q124-d" name="q124" value="D"> <strong>D.</strong> Set up a Amazon Route 53 failover record. Run an AWS Lambda function to execute an AWS CloudFormation template to launch two Amazon EC2 instances. Set up AWS Storage Gateway with stored volumes to back up data to Amazon S3. Set up an AWS Direct Connect connection between a VPC and the data center</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up a Amazon Route 53 failover record. Run application servers on Amazon EC2 instances behind an Application Load Balancer in an Auto Scaling group. Set up AWS Storage Gateway with stored volumes to back up data to Amazon S3

</details>

---

## Câu 125

**Chủ đề:** Design Cost-Optimized Architectures

A company is looking at storing their less frequently accessed files on AWS that can be concurrently accessed by hundreds of Amazon EC2 instances. The company needs the most cost-effective file storage service that provides immediate access to data whenever needed.

Which of the following options represents the best solution for the given requirements?

**Lựa chọn:**

<label for="q125-a"><input type="radio" id="q125-a" name="q125" value="A"> <strong>A.</strong> Amazon Elastic File System (EFS) Standard–IA storage class</label><br>
<label for="q125-b"><input type="radio" id="q125-b" name="q125" value="B"> <strong>B.</strong> Amazon S3 Standard-Infrequent Access (S3 Standard-IA) storage class</label><br>
<label for="q125-c"><input type="radio" id="q125-c" name="q125" value="C"> <strong>C.</strong> Amazon Elastic File System (EFS) Standard storage class</label><br>
<label for="q125-d"><input type="radio" id="q125-d" name="q125" value="D"> <strong>D.</strong> Amazon Elastic Block Store (EBS)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon Elastic File System (EFS) Standard–IA storage class

</details>

---

## Câu 126

**Chủ đề:** Design High-Performing Architectures

A company is developing a global healthcare application that requires the least possible latency for database read/write operations from users in several geographies across the world. The company has hired you as an AWS Certified Solutions Architect Associate to build a solution using Amazon Aurora that offers an effective recovery point objective (RPO) of seconds and a recovery time objective (RTO) of a minute.

Which of the following options would you recommend?

**Lựa chọn:**

<label for="q126-a"><input type="radio" id="q126-a" name="q126" value="A"> <strong>A.</strong> Set up an Amazon Aurora serverless Database cluster</label><br>
<label for="q126-b"><input type="radio" id="q126-b" name="q126" value="B"> <strong>B.</strong> Set up an Amazon Aurora provisioned Database cluster</label><br>
<label for="q126-c"><input type="radio" id="q126-c" name="q126" value="C"> <strong>C.</strong> Set up an Amazon Aurora Global Database cluster</label><br>
<label for="q126-d"><input type="radio" id="q126-d" name="q126" value="D"> <strong>D.</strong> Set up an Amazon Aurora multi-master Database cluster</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set up an Amazon Aurora Global Database cluster

</details>

---

## Câu 127

**Chủ đề:** Design Cost-Optimized Architectures

The engineering manager for a content management application wants to set up Amazon RDS read replicas to provide enhanced performance and read scalability. The manager wants to understand the data transfer charges while setting up Amazon RDS read replicas.

Which of the following would you identify as correct regarding the data transfer charges for Amazon RDS read replicas?

**Lựa chọn:**

<label for="q127-a"><input type="radio" id="q127-a" name="q127" value="A"> <strong>A.</strong> There are data transfer charges for replicating data within the same Availability Zone (AZ)</label><br>
<label for="q127-b"><input type="radio" id="q127-b" name="q127" value="B"> <strong>B.</strong> There are data transfer charges for replicating data within the same AWS Region</label><br>
<label for="q127-c"><input type="radio" id="q127-c" name="q127" value="C"> <strong>C.</strong> There are data transfer charges for replicating data across AWS Regions</label><br>
<label for="q127-d"><input type="radio" id="q127-d" name="q127" value="D"> <strong>D.</strong> There are no data transfer charges for replicating data across AWS Regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. There are data transfer charges for replicating data across AWS Regions

</details>

---

## Câu 128

**Chủ đề:** Design Resilient Architectures

A company has recently launched a new mobile gaming application that the users are adopting rapidly. The company uses Amazon RDS MySQL as the database. The engineering team wants an urgent solution to this issue where the rapidly increasing workload might exceed the available database storage.

As a solutions architect, which of the following solutions would you recommend so that it requires minimum development and systems administration effort to address this requirement?

**Lựa chọn:**

<label for="q128-a"><input type="radio" id="q128-a" name="q128" value="A"> <strong>A.</strong> Enable storage auto-scaling for Amazon RDS MySQL</label><br>
<label for="q128-b"><input type="radio" id="q128-b" name="q128" value="B"> <strong>B.</strong> Migrate RDS MySQL database to Amazon Aurora which offers storage auto-scaling</label><br>
<label for="q128-c"><input type="radio" id="q128-c" name="q128" value="C"> <strong>C.</strong> Migrate Amazon RDS MySQL database to Amazon DynamoDB which automatically allocates storage space when required</label><br>
<label for="q128-d"><input type="radio" id="q128-d" name="q128" value="D"> <strong>D.</strong> Create read replica for Amazon RDS MySQL</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Enable storage auto-scaling for Amazon RDS MySQL

</details>

---

## Câu 129

**Chủ đề:** Design High-Performing Architectures

An analytics company wants to improve the performance of its big data processing workflows running on Amazon Elastic File System (Amazon EFS). Which of the following performance modes should be used for Amazon EFS to address this requirement?

**Lựa chọn:**

<label for="q129-a"><input type="radio" id="q129-a" name="q129" value="A"> <strong>A.</strong> Provisioned Throughput</label><br>
<label for="q129-b"><input type="radio" id="q129-b" name="q129" value="B"> <strong>B.</strong> Bursting Throughput</label><br>
<label for="q129-c"><input type="radio" id="q129-c" name="q129" value="C"> <strong>C.</strong> General Purpose</label><br>
<label for="q129-d"><input type="radio" id="q129-d" name="q129" value="D"> <strong>D.</strong> Max I/O</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Max I/O

</details>

---

## Câu 130

**Chủ đề:** Design Cost-Optimized Architectures

Amazon EC2 Auto Scaling needs to terminate an instance from Availability Zone (AZ) us-east-1a as it has the most number of instances amongst the Availability Zone (AZs) being used currently. There are 4 instances in the Availability Zone (AZ) us-east-1a like so: Instance A has the oldest launch template, Instance B has the oldest launch configuration, Instance C has the newest launch configuration and Instance D is closest to the next billing hour.

Which of the following instances would be terminated per the default termination policy?

**Lựa chọn:**

<label for="q130-a"><input type="radio" id="q130-a" name="q130" value="A"> <strong>A.</strong> Instance A</label><br>
<label for="q130-b"><input type="radio" id="q130-b" name="q130" value="B"> <strong>B.</strong> Instance B</label><br>
<label for="q130-c"><input type="radio" id="q130-c" name="q130" value="C"> <strong>C.</strong> Instance C</label><br>
<label for="q130-d"><input type="radio" id="q130-d" name="q130" value="D"> <strong>D.</strong> Instance D</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Instance B

</details>

---

## Câu 131

**Chủ đề:** Design Secure Architectures

A financial services company wants to identify any sensitive data stored on its Amazon S3 buckets. The company also wants to monitor and protect all data stored on Amazon S3 against any malicious activity.

As a solutions architect, which of the following solutions would you recommend to help address the given requirements?

**Lựa chọn:**

<label for="q131-a"><input type="radio" id="q131-a" name="q131" value="A"> <strong>A.</strong> Use Amazon GuardDuty to monitor any malicious activity on data stored in Amazon S3. Use Amazon Macie to identify any sensitive data stored on Amazon S3</label><br>
<label for="q131-b"><input type="radio" id="q131-b" name="q131" value="B"> <strong>B.</strong> Use Amazon GuardDuty to monitor any malicious activity on data stored in Amazon S3 as well as to identify any sensitive data stored on Amazon S3</label><br>
<label for="q131-c"><input type="radio" id="q131-c" name="q131" value="C"> <strong>C.</strong> Use Amazon Macie to monitor any malicious activity on data stored in Amazon S3 as well as to identify any sensitive data stored on Amazon S3</label><br>
<label for="q131-d"><input type="radio" id="q131-d" name="q131" value="D"> <strong>D.</strong> Use Amazon Macie to monitor any malicious activity on data stored in Amazon S3. Use Amazon GuardDuty to identify any sensitive data stored on Amazon S3</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon GuardDuty to monitor any malicious activity on data stored in Amazon S3. Use Amazon Macie to identify any sensitive data stored on Amazon S3

</details>

---

## Câu 132

**Chủ đề:** Design Resilient Architectures

The engineering team at an e-commerce company wants to migrate from Amazon Simple Queue Service (Amazon SQS) Standard queues to FIFO (First-In-First-Out) queues with batching.

As a solutions architect, which of the following steps would you have in the migration checklist? (Select three)

**Lựa chọn:**

<label for="q132-a"><input type="checkbox" id="q132-a" name="q132" value="A"> <strong>A.</strong> Delete the existing standard queue and recreate it as a FIFO (First-In-First-Out) queue</label><br>
<label for="q132-b"><input type="checkbox" id="q132-b" name="q132" value="B"> <strong>B.</strong> Convert the existing standard queue into a FIFO (First-In-First-Out) queue</label><br>
<label for="q132-c"><input type="checkbox" id="q132-c" name="q132" value="C"> <strong>C.</strong> Make sure that the name of the FIFO (First-In-First-Out) queue ends with the .fifo suffix</label><br>
<label for="q132-d"><input type="checkbox" id="q132-d" name="q132" value="D"> <strong>D.</strong> Make sure that the name of the FIFO (First-In-First-Out) queue is the same as the standard queue</label><br>
<label for="q132-e"><input type="checkbox" id="q132-e" name="q132" value="E"> <strong>E.</strong> Make sure that the throughput for the target FIFO (First-In-First-Out) queue does not exceed 3,000 messages per second</label><br>
<label for="q132-f"><input type="checkbox" id="q132-f" name="q132" value="F"> <strong>F.</strong> Make sure that the throughput for the target FIFO (First-In-First-Out) queue does not exceed 300 messages per second</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Delete the existing standard queue and recreate it as a FIFO (First-In-First-Out) queue

C. Make sure that the name of the FIFO (First-In-First-Out) queue ends with the .fifo suffix

E. Make sure that the throughput for the target FIFO (First-In-First-Out) queue does not exceed 3,000 messages per second

</details>

---

## Câu 133

**Chủ đề:** Design High-Performing Architectures

A global pharmaceutical company wants to move most of the on-premises data into Amazon S3, Amazon Elastic File System (Amazon EFS), and Amazon FSx for Windows File Server easily, quickly, and cost-effectively.

As a solutions architect, which of the following solutions would you recommend as the BEST fit to automate and accelerate online data transfers to these AWS storage services?

**Lựa chọn:**

<label for="q133-a"><input type="radio" id="q133-a" name="q133" value="A"> <strong>A.</strong> Use AWS DataSync to automate and accelerate online data transfers to the given AWS storage services</label><br>
<label for="q133-b"><input type="radio" id="q133-b" name="q133" value="B"> <strong>B.</strong> Use AWS Snowball Edge Storage Optimized device to automate and accelerate online data transfers to the given AWS storage services</label><br>
<label for="q133-c"><input type="radio" id="q133-c" name="q133" value="C"> <strong>C.</strong> Use AWS Transfer Family to automate and accelerate online data transfers to the given AWS storage services</label><br>
<label for="q133-d"><input type="radio" id="q133-d" name="q133" value="D"> <strong>D.</strong> Use File Gateway to automate and accelerate online data transfers to the given AWS storage services</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS DataSync to automate and accelerate online data transfers to the given AWS storage services

</details>

---

## Câu 134

**Chủ đề:** Design Cost-Optimized Architectures

A company has a license-based, expensive, legacy commercial database solution deployed at its on-premises data center. The company wants to migrate this database to a more efficient, open-source, and cost-effective option on AWS Cloud. The CTO at the company wants a solution that can handle complex database configurations such as secondary indexes, foreign keys, and stored procedures.

As a solutions architect, which of the following AWS services should be combined to handle this use-case? (Select two)

**Lựa chọn:**

<label for="q134-a"><input type="checkbox" id="q134-a" name="q134" value="A"> <strong>A.</strong> AWS Snowball Edge</label><br>
<label for="q134-b"><input type="checkbox" id="q134-b" name="q134" value="B"> <strong>B.</strong> AWS Schema Conversion Tool (AWS SCT)</label><br>
<label for="q134-c"><input type="checkbox" id="q134-c" name="q134" value="C"> <strong>C.</strong> AWS Database Migration Service (AWS DMS)</label><br>
<label for="q134-d"><input type="checkbox" id="q134-d" name="q134" value="D"> <strong>D.</strong> AWS Glue</label><br>
<label for="q134-e"><input type="checkbox" id="q134-e" name="q134" value="E"> <strong>E.</strong> Basic Schema Copy</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. AWS Schema Conversion Tool (AWS SCT)

C. AWS Database Migration Service (AWS DMS)

</details>

---

## Câu 135

**Chủ đề:** Design High-Performing Architectures

A financial services company is modernizing its analytics platform on AWS. Their legacy data processing scripts, built for both Windows and Linux environments, require shared access to a file system that supports Windows ACLs and SMB protocol for compatibility with existing Windows workloads. At the same time, their Linux-based applications need to read from and write to the same shared storage to maintain cross-platform consistency. The solutions architect needs to design a storage solution that allows both Windows and Linux EC2 instances to access the shared file system simultaneously, while preserving Windows-specific features like NTFS permissions and Active Directory (AD) integration.

Which solution will best meet these requirements?

**Lựa chọn:**

<label for="q135-a"><input type="radio" id="q135-a" name="q135" value="A"> <strong>A.</strong> Deploy Amazon FSx for Windows File Server and mount it using the SMB protocol from both Windows and Linux EC2 instances</label><br>
<label for="q135-b"><input type="radio" id="q135-b" name="q135" value="B"> <strong>B.</strong> Use Amazon EFS with the Standard storage class and mount the file system using NFS from both Windows and Linux instances</label><br>
<label for="q135-c"><input type="radio" id="q135-c" name="q135" value="C"> <strong>C.</strong> Deploy Amazon FSx for Lustre and mount the file system using a POSIX-compliant client from both platforms</label><br>
<label for="q135-d"><input type="radio" id="q135-d" name="q135" value="D"> <strong>D.</strong> Create an S3 bucket and mount it on EC2 instances using Mountpoint for Amazon S3, managing access through IAM policies to support both Windows and Linux workloads</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy Amazon FSx for Windows File Server and mount it using the SMB protocol from both Windows and Linux EC2 instances

</details>

---

## Câu 136

**Chủ đề:** Design Resilient Architectures

A software company manages a fleet of Amazon EC2 instances that support internal analytics applications. These instances use an IAM role with custom policies to connect to Amazon RDS and AWS Secrets Manager for secure access to credentials and database endpoints. The IT operations team wants to implement a centralized patch management solution that simplifies compliance and security tasks. Their goal is to automate OS patching across EC2 instances without disrupting the running applications.

Which approach will allow the company to meet these goals with the least administrative overhead?

**Lựa chọn:**

<label for="q136-a"><input type="radio" id="q136-a" name="q136" value="A"> <strong>A.</strong> Enable Default Host Management Configuration in AWS Systems Manager Quick Setup</label><br>
<label for="q136-b"><input type="radio" id="q136-b" name="q136" value="B"> <strong>B.</strong> Create a second IAM role with the AmazonSSMManagedInstanceCore policy and attach both the new and the existing IAM roles to each EC2 instance using Systems Manager Hybrid Activation</label><br>
<label for="q136-c"><input type="radio" id="q136-c" name="q136" value="C"> <strong>C.</strong> Manually install the Systems Manager Agent (SSM Agent) on each EC2 instance. Schedule daily patch jobs using cron scripts</label><br>
<label for="q136-d"><input type="radio" id="q136-d" name="q136" value="D"> <strong>D.</strong> Detach the existing IAM role from all EC2 instances. Replace it with a new role that has both the original permissions and the AmazonSSMManagedInstanceCore policy to enable Systems Manager features</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Enable Default Host Management Configuration in AWS Systems Manager Quick Setup

</details>

---

## Câu 137

**Chủ đề:** Design Secure Architectures

The engineering team at a company wants to use Amazon Simple Queue Service (Amazon SQS) to decouple components of the underlying application architecture. However, the team is concerned about the VPC-bound components accessing Amazon Simple Queue Service (Amazon SQS) over the public internet.

As a solutions architect, which of the following solutions would you recommend to address this use-case?

**Lựa chọn:**

<label for="q137-a"><input type="radio" id="q137-a" name="q137" value="A"> <strong>A.</strong> Use VPC endpoint to access Amazon SQS</label><br>
<label for="q137-b"><input type="radio" id="q137-b" name="q137" value="B"> <strong>B.</strong> Use Internet Gateway to access Amazon SQS</label><br>
<label for="q137-c"><input type="radio" id="q137-c" name="q137" value="C"> <strong>C.</strong> Use Network Address Translation (NAT) instance to access Amazon SQS</label><br>
<label for="q137-d"><input type="radio" id="q137-d" name="q137" value="D"> <strong>D.</strong> Use VPN connection to access Amazon SQS</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use VPC endpoint to access Amazon SQS

</details>

---

## Câu 138

**Chủ đề:** Design High-Performing Architectures

A media company wants a low-latency way to distribute live sports results which are delivered via a proprietary application using UDP protocol.

As a solutions architect, which of the following solutions would you recommend such that it offers the BEST performance for this use case?

**Lựa chọn:**

<label for="q138-a"><input type="radio" id="q138-a" name="q138" value="A"> <strong>A.</strong> Use Elastic Load Balancing (ELB) to provide a low latency way to distribute live sports results</label><br>
<label for="q138-b"><input type="radio" id="q138-b" name="q138" value="B"> <strong>B.</strong> Use Amazon CloudFront to provide a low latency way to distribute live sports results</label><br>
<label for="q138-c"><input type="radio" id="q138-c" name="q138" value="C"> <strong>C.</strong> Use AWS Global Accelerator to provide a low latency way to distribute live sports results</label><br>
<label for="q138-d"><input type="radio" id="q138-d" name="q138" value="D"> <strong>D.</strong> Use Auto Scaling group to provide a low latency way to distribute live sports results</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use AWS Global Accelerator to provide a low latency way to distribute live sports results

</details>

---

## Câu 139

**Chủ đề:** Design Resilient Architectures

The DevOps team at an IT company has created a custom VPC (V1) and attached an Internet Gateway (I1) to the VPC. The team has also created a subnet (S1) in this custom VPC and added a route to this subnet's route table (R1) that directs internet-bound traffic to the Internet Gateway. Now the team launches an Amazon EC2 instance (E1) in the subnet S1 and assigns a public IPv4 address to this instance. Next the team also launches a Network Address Translation (NAT) instance (N1) in the subnet S1.

Under the given infrastructure setup, which of the following entities is doing the Network Address Translation for the Amazon EC2 instance E1?

**Lựa chọn:**

<label for="q139-a"><input type="radio" id="q139-a" name="q139" value="A"> <strong>A.</strong> Network Address Translation (NAT) instance (N1)</label><br>
<label for="q139-b"><input type="radio" id="q139-b" name="q139" value="B"> <strong>B.</strong> Internet Gateway (I1)</label><br>
<label for="q139-c"><input type="radio" id="q139-c" name="q139" value="C"> <strong>C.</strong> Subnet (S1)</label><br>
<label for="q139-d"><input type="radio" id="q139-d" name="q139" value="D"> <strong>D.</strong> Route Table (R1)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Internet Gateway (I1)

</details>

---

## Câu 140

**Chủ đề:** Design Resilient Architectures

A company has hired you as an AWS Certified Solutions Architect – Associate to help with redesigning a real-time data processor. The company wants to build custom applications that process and analyze the streaming data for its specialized needs.

Which solution will you recommend to address this use-case?

**Lựa chọn:**

<label for="q140-a"><input type="radio" id="q140-a" name="q140" value="A"> <strong>A.</strong> Use Amazon Simple Queue Service (Amazon SQS) to process the data streams as well as decouple the producers and consumers for the real-time data processor</label><br>
<label for="q140-b"><input type="radio" id="q140-b" name="q140" value="B"> <strong>B.</strong> Use Amazon Simple Notification Service (Amazon SNS) to process the data streams as well as decouple the producers and consumers for the real-time data processor</label><br>
<label for="q140-c"><input type="radio" id="q140-c" name="q140" value="C"> <strong>C.</strong> Use Amazon Kinesis Data Streams to process the data streams as well as decouple the producers and consumers for the real-time data processor</label><br>
<label for="q140-d"><input type="radio" id="q140-d" name="q140" value="D"> <strong>D.</strong> Use Amazon Kinesis Data Firehose to process the data streams as well as decouple the producers and consumers for the real-time data processor</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Amazon Kinesis Data Streams to process the data streams as well as decouple the producers and consumers for the real-time data processor

</details>

---

## Câu 141

**Chủ đề:** Design High-Performing Architectures

An engineering team wants to orchestrate multiple Amazon ECS task types running on Amazon EC2 instances that are part of the Amazon ECS cluster. The output and state data for all tasks need to be stored. The amount of data output by each task is approximately 20 megabytes and there could be hundreds of tasks running at a time. As old outputs are archived, the storage size is not expected to exceed 1 terabyte.

As a solutions architect, which of the following would you recommend as an optimized solution for high-frequency reading and writing?

**Lựa chọn:**

<label for="q141-a"><input type="radio" id="q141-a" name="q141" value="A"> <strong>A.</strong> Use Amazon EFS with Provisioned Throughput mode</label><br>
<label for="q141-b"><input type="radio" id="q141-b" name="q141" value="B"> <strong>B.</strong> Use Amazon EFS with Bursting Throughput mode</label><br>
<label for="q141-c"><input type="radio" id="q141-c" name="q141" value="C"> <strong>C.</strong> Use Amazon DynamoDB table that is accessible by all ECS cluster instances</label><br>
<label for="q141-d"><input type="radio" id="q141-d" name="q141" value="D"> <strong>D.</strong> Use an Amazon EBS volume mounted to the Amazon ECS cluster instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon EFS with Provisioned Throughput mode

</details>

---

## Câu 142

**Chủ đề:** Design High-Performing Architectures

The DevOps team at an IT company is provisioning a two-tier application in a VPC with a public subnet and a private subnet. The team wants to use either a Network Address Translation (NAT) instance or a Network Address Translation (NAT) gateway in the public subnet to enable instances in the private subnet to initiate outbound IPv4 traffic to the internet but needs some technical assistance in terms of the configuration options available for the Network Address Translation (NAT) instance and the Network Address Translation (NAT) gateway.

As a solutions architect, which of the following options would you identify as CORRECT? (Select three)

**Lựa chọn:**

<label for="q142-a"><input type="checkbox" id="q142-a" name="q142" value="A"> <strong>A.</strong> NAT gateway supports port forwarding</label><br>
<label for="q142-b"><input type="checkbox" id="q142-b" name="q142" value="B"> <strong>B.</strong> Security Groups can be associated with a NAT gateway</label><br>
<label for="q142-c"><input type="checkbox" id="q142-c" name="q142" value="C"> <strong>C.</strong> NAT gateway can be used as a bastion server</label><br>
<label for="q142-d"><input type="checkbox" id="q142-d" name="q142" value="D"> <strong>D.</strong> NAT instance can be used as a bastion server</label><br>
<label for="q142-e"><input type="checkbox" id="q142-e" name="q142" value="E"> <strong>E.</strong> Security Groups can be associated with a NAT instance</label><br>
<label for="q142-f"><input type="checkbox" id="q142-f" name="q142" value="F"> <strong>F.</strong> NAT instance supports port forwarding</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. NAT instance can be used as a bastion server

E. Security Groups can be associated with a NAT instance

F. NAT instance supports port forwarding

</details>

---

## Câu 143

**Chủ đề:** Design High-Performing Architectures

A leading online gaming company is migrating its flagship application to AWS Cloud for delivering its online games to users across the world. The company would like to use a Network Load Balancer to handle millions of requests per second. The engineering team has provisioned multiple instances in a public subnet and specified these instance IDs as the targets for the NLB.

As a solutions architect, can you help the engineering team understand the correct routing mechanism for these target instances?

**Lựa chọn:**

<label for="q143-a"><input type="radio" id="q143-a" name="q143" value="A"> <strong>A.</strong> Traffic is routed to instances using the primary private IP address specified in the primary network interface for the instance</label><br>
<label for="q143-b"><input type="radio" id="q143-b" name="q143" value="B"> <strong>B.</strong> Traffic is routed to instances using the primary public IP address specified in the primary network interface for the instance</label><br>
<label for="q143-c"><input type="radio" id="q143-c" name="q143" value="C"> <strong>C.</strong> Traffic is routed to instances using the primary elastic IP address specified in the primary network interface for the instance</label><br>
<label for="q143-d"><input type="radio" id="q143-d" name="q143" value="D"> <strong>D.</strong> Traffic is routed to instances using the instance ID specified in the primary network interface for the instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Traffic is routed to instances using the primary private IP address specified in the primary network interface for the instance

</details>

---

## Câu 144

**Chủ đề:** Design Resilient Architectures

An e-commerce company is using Elastic Load Balancing (ELB) for its fleet of Amazon EC2 instances spread across two Availability Zones (AZs), with one instance as a target in Availability Zone A and four instances as targets in Availability Zone B. The company is doing benchmarking for server performance when cross-zone load balancing is enabled compared to the case when cross-zone load balancing is disabled.

As a solutions architect, which of the following traffic distribution outcomes would you identify as correct?

**Lựa chọn:**

<label for="q144-a"><input type="radio" id="q144-a" name="q144" value="A"> <strong>A.</strong> With cross-zone load balancing enabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each</label><br>
<label for="q144-b"><input type="radio" id="q144-b" name="q144" value="B"> <strong>B.</strong> With cross-zone load balancing enabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each</label><br>
<label for="q144-c"><input type="radio" id="q144-c" name="q144" value="C"> <strong>C.</strong> With cross-zone load balancing enabled, one instance in Availability Zone A receives no traffic and four instances in Availability Zone B receive 25% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each</label><br>
<label for="q144-d"><input type="radio" id="q144-d" name="q144" value="D"> <strong>D.</strong> With cross-zone load balancing enabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives no traffic and four instances in Availability Zone B receive 25% traffic each</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. With cross-zone load balancing enabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each

</details>

---

## Câu 145

**Chủ đề:** Design High-Performing Architectures

A healthcare company has deployed its web application on Amazon Elastic Container Service (Amazon ECS) container instances running behind an Application Load Balancer. The website slows down when the traffic spikes and the website availability is also reduced. The development team has configured Amazon CloudWatch alarms to receive notifications whenever there is an availability constraint so the team can scale out resources. The company wants an automated solution to respond to such events.

Which of the following addresses the given use case?

**Lựa chọn:**

<label for="q145-a"><input type="radio" id="q145-a" name="q145" value="A"> <strong>A.</strong> Configure AWS Auto Scaling to scale out the Amazon ECS cluster when the ECS service's CPU utilization rises above a threshold</label><br>
<label for="q145-b"><input type="radio" id="q145-b" name="q145" value="B"> <strong>B.</strong> Configure AWS Auto Scaling to scale out the Amazon ECS cluster when the Application Load Balancer's target group's CPU utilization rises above a threshold</label><br>
<label for="q145-c"><input type="radio" id="q145-c" name="q145" value="C"> <strong>C.</strong> Configure AWS Auto Scaling to scale out the Amazon ECS cluster when the Application Load Balancer's CPU utilization rises above a threshold</label><br>
<label for="q145-d"><input type="radio" id="q145-d" name="q145" value="D"> <strong>D.</strong> Configure AWS Auto Scaling to scale out the Amazon ECS cluster when the CloudWatch alarm's CPU utilization rises above a threshold</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Configure AWS Auto Scaling to scale out the Amazon ECS cluster when the ECS service's CPU utilization rises above a threshold

</details>

---

## Câu 146

**Chủ đề:** Design Secure Architectures

A national logistics company has a dedicated AWS Direct Connect connection from its corporate data center to AWS. Within its AWS account, the company operates 25 Amazon VPCs in the same Region, each supporting different regional distribution services. The VPCs were configured with non-overlapping CIDR blocks and currently use private VIFs for Direct Connect access to on-premises resources. As the architecture scales, the company wants to enable communication across all VPCs and the on-premises environment. The solution must scale efficiently, support full-mesh connectivity, and reduce the complexity of maintaining separate private VIFs for each VPC.

Which combination of solutions will best fulfill these requirements with the least amount of operational overhead? (Select two)

**Lựa chọn:**

<label for="q146-a"><input type="checkbox" id="q146-a" name="q146" value="A"> <strong>A.</strong> Create an AWS Transit Gateway and attach all 25 VPCs to it. Enable route propagation for each attachment to automatically manage inter-VPC routing</label><br>
<label for="q146-b"><input type="checkbox" id="q146-b" name="q146" value="B"> <strong>B.</strong> Create a transit virtual interface (VIF) from the Direct Connect connection and associate it with the transit gateway</label><br>
<label for="q146-c"><input type="checkbox" id="q146-c" name="q146" value="C"> <strong>C.</strong> Create individual Site-to-Site VPN connections from the data center to each VPC. Set up BGP route propagation for every tunnel to facilitate on-premises-to-VPC routing</label><br>
<label for="q146-d"><input type="checkbox" id="q146-d" name="q146" value="D"> <strong>D.</strong> Reconfigure each VPC to connect through AWS PrivateLink endpoints to a central networking service VPC. Share the service with other VPCs using VPC endpoint services</label><br>
<label for="q146-e"><input type="checkbox" id="q146-e" name="q146" value="E"> <strong>E.</strong> Convert each existing private VIF into a new Direct Connect gateway association by attaching a virtual private gateway (VGW) to each VPC. Manually configure routing between VGWs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an AWS Transit Gateway and attach all 25 VPCs to it. Enable route propagation for each attachment to automatically manage inter-VPC routing

B. Create a transit virtual interface (VIF) from the Direct Connect connection and associate it with the transit gateway

</details>

---

## Câu 147

**Chủ đề:** Design Secure Architectures

A retail company uses AWS Cloud to manage its IT infrastructure. The company has set up AWS Organizations to manage several departments running their AWS accounts and using resources such as Amazon EC2 instances and Amazon RDS databases. The company wants to provide shared and centrally-managed VPCs to all departments using applications that need a high degree of interconnectivity.

As a solutions architect, which of the following options would you choose to facilitate this use-case?

**Lựa chọn:**

<label for="q147-a"><input type="radio" id="q147-a" name="q147" value="A"> <strong>A.</strong> Use VPC sharing to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations</label><br>
<label for="q147-b"><input type="radio" id="q147-b" name="q147" value="B"> <strong>B.</strong> Use VPC sharing to share a VPC with other AWS accounts belonging to the same parent organization from AWS Organizations</label><br>
<label for="q147-c"><input type="radio" id="q147-c" name="q147" value="C"> <strong>C.</strong> Use VPC peering to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations</label><br>
<label for="q147-d"><input type="radio" id="q147-d" name="q147" value="D"> <strong>D.</strong> Use VPC peering to share a VPC with other AWS accounts belonging to the same parent organization from AWS Organizations</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use VPC sharing to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations

</details>

---

## Câu 148

**Chủ đề:** Design Secure Architectures

A retail organization is moving some of its on-premises data to AWS Cloud. The DevOps team at the organization has set up an AWS Managed IPSec VPN Connection between their remote on-premises network and their Amazon VPC over the internet.

Which of the following represents the correct configuration for the IPSec VPN Connection?

**Lựa chọn:**

<label for="q148-a"><input type="radio" id="q148-a" name="q148" value="A"> <strong>A.</strong> Create a virtual private gateway (VGW) on the on-premises side of the VPN and a Customer Gateway on the AWS side of the VPN</label><br>
<label for="q148-b"><input type="radio" id="q148-b" name="q148" value="B"> <strong>B.</strong> Create a Customer Gateway on both the AWS side of the VPN as well as the on-premises side of the VPN</label><br>
<label for="q148-c"><input type="radio" id="q148-c" name="q148" value="C"> <strong>C.</strong> Create a virtual private gateway (VGW) on the AWS side of the VPN and a Customer Gateway on the on-premises side of the VPN</label><br>
<label for="q148-d"><input type="radio" id="q148-d" name="q148" value="D"> <strong>D.</strong> Create a virtual private gateway (VGW) on both the AWS side of the VPN as well as the on-premises side of the VPN</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Create a virtual private gateway (VGW) on the AWS side of the VPN and a Customer Gateway on the on-premises side of the VPN

</details>

---

## Câu 149

**Chủ đề:** Design Cost-Optimized Architectures

A startup has created a new web application for users to complete a risk assessment survey for COVID-19 symptoms via a self-administered questionnaire. The startup has purchased the domain covid19survey.com using Amazon Route 53. The web development team would like to create Amazon Route 53 record so that all traffic for covid19survey.com is routed to www.covid19survey.com.

As a solutions architect, which of the following is the MOST cost-effective solution that you would recommend to the web development team?

**Lựa chọn:**

<label for="q149-a"><input type="radio" id="q149-a" name="q149" value="A"> <strong>A.</strong> Create a CNAME record for covid19survey.com that routes traffic to www.covid19survey.com</label><br>
<label for="q149-b"><input type="radio" id="q149-b" name="q149" value="B"> <strong>B.</strong> Create an alias record for covid19survey.com that routes traffic to www.covid19survey.com</label><br>
<label for="q149-c"><input type="radio" id="q149-c" name="q149" value="C"> <strong>C.</strong> Create an MX record for covid19survey.com that routes traffic to www.covid19survey.com</label><br>
<label for="q149-d"><input type="radio" id="q149-d" name="q149" value="D"> <strong>D.</strong> Create an NS record for covid19survey.com that routes traffic to www.covid19survey.com</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create an alias record for covid19survey.com that routes traffic to www.covid19survey.com

</details>

---

## Câu 150

**Chủ đề:** Design High-Performing Architectures

A healthcare startup is modernizing its monolithic Python-based analytics application by transitioning to a microservices architecture on AWS. As a pilot, the team wants to refactor one module into a standalone microservice that can handle hundreds of requests per second. They are seeking an AWS-native solution that supports Python, scales automatically with traffic, and requires minimal infrastructure management and operational overhead to build, test, and deploy the service efficiently.

Which AWS solution best meets these requirements?

**Lựa chọn:**

<label for="q150-a"><input type="radio" id="q150-a" name="q150" value="A"> <strong>A.</strong> Deploy the microservice in an AWS Fargate task using Amazon ECS. Package the code in a Docker container image with a Python runtime and configure ECS Service Auto Scaling to respond to CPU utilization metrics</label><br>
<label for="q150-b"><input type="radio" id="q150-b" name="q150" value="B"> <strong>B.</strong> Use AWS App Runner to build and deploy the Python application directly from a GitHub repository. Allow App Runner to manage traffic scaling and deployments</label><br>
<label for="q150-c"><input type="radio" id="q150-c" name="q150" value="C"> <strong>C.</strong> Use Amazon EC2 Spot Instances in an Auto Scaling group. Launch the Python application as a background service and install all required dependencies at instance startup</label><br>
<label for="q150-d"><input type="radio" id="q150-d" name="q150" value="D"> <strong>D.</strong> Use AWS Lambda to run the Python-based microservice. Integrate it with Amazon API Gateway for HTTP access and enable provisioned concurrency for performance during peak loads</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Lambda to run the Python-based microservice. Integrate it with Amazon API Gateway for HTTP access and enable provisioned concurrency for performance during peak loads

</details>

---

## Câu 151

**Chủ đề:** Design High-Performing Architectures

A video conferencing application is hosted on a fleet of EC2 instances which are part of an Auto Scaling group. The Auto Scaling group uses a Launch Template (LT1) with "dedicated" instance tenancy but the VPC (V1) used by the Launch Template LT1 has the instance tenancy set to default. Later the DevOps team creates a new Launch Template (LT2) with shared (default) instance tenancy but the VPC (V2) used by the Launch Template LT2 has the instance tenancy set to dedicated.

Which of the following is correct regarding the instances launched via Launch Template LT1 and Launch Template LT2?

**Lựa chọn:**

<label for="q151-a"><input type="radio" id="q151-a" name="q151" value="A"> <strong>A.</strong> The instances launched by Launch Template LT1 will have dedicated instance tenancy while the instances launched by the Launch Template LT2 will have shared (default) instance tenancy</label><br>
<label for="q151-b"><input type="radio" id="q151-b" name="q151" value="B"> <strong>B.</strong> The instances launched by Launch Template LT1 will have default instance tenancy while the instances launched by the Launch Template LT2 will have dedicated instance tenancy</label><br>
<label for="q151-c"><input type="radio" id="q151-c" name="q151" value="C"> <strong>C.</strong> The instances launched by both Launch Template LT1 and Launch Template LT2 will have default instance tenancy</label><br>
<label for="q151-d"><input type="radio" id="q151-d" name="q151" value="D"> <strong>D.</strong> The instances launched by both Launch Template LT1 and Launch Template LT2 will have dedicated instance tenancy</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. The instances launched by both Launch Template LT1 and Launch Template LT2 will have dedicated instance tenancy

</details>

---

## Câu 152

**Chủ đề:** Design High-Performing Architectures

An IT consultant is helping a small business revamp their technology infrastructure on the AWS Cloud. The business has two AWS accounts and all resources are provisioned in the us-west-2 region. The IT consultant is trying to launch an Amazon EC2 instance in each of the two AWS accounts such that the instances are in the same Availability Zone (AZ) of the us-west-2 region. Even after selecting the same default subnet (us-west-2a) while launching the instances in each of the AWS accounts, the IT consultant notices that the Availability Zones (AZs) are still different.

As a solutions architect, which of the following would you suggest resolving this issue?

**Lựa chọn:**

<label for="q152-a"><input type="radio" id="q152-a" name="q152" value="A"> <strong>A.</strong> Reach out to AWS Support for creating the Amazon EC2 instances in the same Availability Zone (AZ) across the two AWS accounts</label><br>
<label for="q152-b"><input type="radio" id="q152-b" name="q152" value="B"> <strong>B.</strong> Use Availability Zone (AZ) ID to uniquely identify the Availability Zones across the two AWS Accounts</label><br>
<label for="q152-c"><input type="radio" id="q152-c" name="q152" value="C"> <strong>C.</strong> Use the default subnet to uniquely identify the Availability Zones across the two AWS Accounts</label><br>
<label for="q152-d"><input type="radio" id="q152-d" name="q152" value="D"> <strong>D.</strong> Use the default VPC to uniquely identify the Availability Zones across the two AWS Accounts</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Availability Zone (AZ) ID to uniquely identify the Availability Zones across the two AWS Accounts

</details>

---

## Câu 153

**Chủ đề:** Design Secure Architectures

An application running on an Amazon EC2 instance needs to access a Amazon DynamoDB table in the same AWS account.

Which of the following solutions should a solutions architect configure for the necessary permissions?

**Lựa chọn:**

<label for="q153-a"><input type="radio" id="q153-a" name="q153" value="A"> <strong>A.</strong> Set up an IAM user with the appropriate permissions to allow access to the Amazon DynamoDB table. Store the access credentials in an Amazon S3 bucket and read them from within the application code directly</label><br>
<label for="q153-b"><input type="radio" id="q153-b" name="q153" value="B"> <strong>B.</strong> Set up an IAM user with the appropriate permissions to allow access to the Amazon DynamoDB table. Store the access credentials in the local storage and read them from within the application code directly</label><br>
<label for="q153-c"><input type="radio" id="q153-c" name="q153" value="C"> <strong>C.</strong> Set up an IAM service role with the appropriate permissions to allow access to the Amazon DynamoDB table. Add the Amazon EC2 instance to the trust relationship policy document so that the instance can assume the role</label><br>
<label for="q153-d"><input type="radio" id="q153-d" name="q153" value="D"> <strong>D.</strong> Set up an IAM service role with the appropriate permissions to allow access to the Amazon DynamoDB table. Configure an instance profile to assign this IAM role to the Amazon EC2 instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up an IAM service role with the appropriate permissions to allow access to the Amazon DynamoDB table. Configure an instance profile to assign this IAM role to the Amazon EC2 instance

</details>

---

## Câu 154

**Chủ đề:** Design Secure Architectures

A company maintains its business-critical customer data on an on-premises system in an encrypted format. Over the years, the company has transitioned from using a single encryption key to multiple encryption keys by dividing the data into logical chunks. With the decision to move all the data to an Amazon S3 bucket, the company is now looking for a technique to encrypt each file with a different encryption key to provide maximum security to the migrated on-premises data.

How will you implement this requirement without adding the overhead of splitting the data into logical groups?

**Lựa chọn:**

<label for="q154-a"><input type="radio" id="q154-a" name="q154" value="A"> <strong>A.</strong> Store the logically divided data into different Amazon S3 buckets. Use server-side encryption with Amazon S3 managed keys (SSE-S3) to encrypt the data</label><br>
<label for="q154-b"><input type="radio" id="q154-b" name="q154" value="B"> <strong>B.</strong> Configure a single Amazon S3 bucket to hold all data. Use server-side encryption with Amazon S3 managed keys (SSE-S3) to encrypt the data</label><br>
<label for="q154-c"><input type="radio" id="q154-c" name="q154" value="C"> <strong>C.</strong> Use Multi-Region keys for client-side encryption in the AWS S3 Encryption Client to generate unique keys for each file of data</label><br>
<label for="q154-d"><input type="radio" id="q154-d" name="q154" value="D"> <strong>D.</strong> Configure a single Amazon S3 bucket to hold all data. Use server-side encryption with AWS KMS (SSE-KMS) and use encryption context to generate a different key for each file/object that you store in the S3 bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure a single Amazon S3 bucket to hold all data. Use server-side encryption with Amazon S3 managed keys (SSE-S3) to encrypt the data

</details>

---

## Câu 155

**Chủ đề:** Design Secure Architectures

A developer has configured inbound traffic for the relevant ports in both the Security Group of the Amazon EC2 instance as well as the Network Access Control List (Network ACL) of the subnet for the Amazon EC2 instance. The developer is, however, unable to connect to the service running on the Amazon EC2 instance.

As a solutions architect, how will you fix this issue?

**Lựa chọn:**

<label for="q155-a"><input type="radio" id="q155-a" name="q155" value="A"> <strong>A.</strong> Network ACLs are stateful, so allowing inbound traffic to the necessary ports enables the connection. Security Groups are stateless, so you must allow both inbound and outbound traffic</label><br>
<label for="q155-b"><input type="radio" id="q155-b" name="q155" value="B"> <strong>B.</strong> IAM Role defined in the Security Group is different from the IAM Role that is given access in the Network ACLs</label><br>
<label for="q155-c"><input type="radio" id="q155-c" name="q155" value="C"> <strong>C.</strong> Security Groups are stateful, so allowing inbound traffic to the necessary ports enables the connection. Network ACLs are stateless, so you must allow both inbound and outbound traffic</label><br>
<label for="q155-d"><input type="radio" id="q155-d" name="q155" value="D"> <strong>D.</strong> Rules associated with Network ACLs should never be modified from command line. An attempt to modify rules from command line blocks the rule and results in an erratic behavior</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Security Groups are stateful, so allowing inbound traffic to the necessary ports enables the connection. Network ACLs are stateless, so you must allow both inbound and outbound traffic

</details>

---

## Câu 156

**Chủ đề:** Design Secure Architectures

A company is transferring a significant volume of data from on-site storage to AWS, where it will be accessed by Windows, Mac, and Linux-based Amazon EC2 instances within the same AWS region using both SMB and NFS protocols. Part of this data will be accessed regularly, while the rest will be accessed less frequently. The company requires a hosting solution for this data that minimizes operational overhead.

What solution would best meet these requirements?

**Lựa chọn:**

<label for="q156-a"><input type="radio" id="q156-a" name="q156" value="A"> <strong>A.</strong> Set up an Amazon FSx for ONTAP instance. Configure an FSx for ONTAP file system on the root volume and migrate the data to the FSx for ONTAP volume</label><br>
<label for="q156-b"><input type="radio" id="q156-b" name="q156" value="B"> <strong>B.</strong> Set up an Amazon FSx for OpenZFS instance. Configure an FSx for OpenZFS file ystem on the root volume and migrate the data to the FSx for OpenZFS volume</label><br>
<label for="q156-c"><input type="radio" id="q156-c" name="q156" value="C"> <strong>C.</strong> Set up an Amazon Elastic File System (Amazon EFS) volume that uses EFS Intelligent-Tiering. Use AWS DataSync to migrate the data to the EFS volume</label><br>
<label for="q156-d"><input type="radio" id="q156-d" name="q156" value="D"> <strong>D.</strong> Set up an Amazon Elastic File System (Amazon EFS) volume that uses EFS Infrequent Access. Use AWS DataSync to migrate the data to the EFS volume</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Set up an Amazon FSx for ONTAP instance. Configure an FSx for ONTAP file system on the root volume and migrate the data to the FSx for ONTAP volume

</details>

---

## Câu 157

**Chủ đề:** Design High-Performing Architectures

A big data analytics company is working on a real-time vehicle tracking solution. The data processing workflow involves both I/O intensive and throughput intensive database workloads. The development team needs to store this real-time data in a NoSQL database hosted on an Amazon EC2 instance and needs to support up to 25,000 IOPS per volume.

As a solutions architect, which of the following Amazon Elastic Block Store (Amazon EBS) volume types would you recommend for this use-case?

**Lựa chọn:**

<label for="q157-a"><input type="radio" id="q157-a" name="q157" value="A"> <strong>A.</strong> General Purpose SSD (gp2)</label><br>
<label for="q157-b"><input type="radio" id="q157-b" name="q157" value="B"> <strong>B.</strong> Cold HDD (sc1)</label><br>
<label for="q157-c"><input type="radio" id="q157-c" name="q157" value="C"> <strong>C.</strong> Provisioned IOPS SSD (io1)</label><br>
<label for="q157-d"><input type="radio" id="q157-d" name="q157" value="D"> <strong>D.</strong> Throughput Optimized HDD (st1)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Provisioned IOPS SSD (io1)

</details>

---

## Câu 158

**Chủ đề:** Design High-Performing Architectures

An e-commerce company uses Microsoft Active Directory to provide users and groups with access to resources on the on-premises infrastructure. The company has extended its IT infrastructure to AWS in the form of a hybrid cloud. The engineering team at the company wants to run directory-aware workloads on AWS for a SQL Server-based application. The team also wants to configure a trust relationship to enable single sign-on (SSO) for its users to access resources in either domain.

As a solutions architect, which of the following AWS services would you recommend for this use-case?

**Lựa chọn:**

<label for="q158-a"><input type="radio" id="q158-a" name="q158" value="A"> <strong>A.</strong> Active Directory Connector</label><br>
<label for="q158-b"><input type="radio" id="q158-b" name="q158" value="B"> <strong>B.</strong> AWS Directory Service for Microsoft Active Directory (AWS Managed Microsoft AD)</label><br>
<label for="q158-c"><input type="radio" id="q158-c" name="q158" value="C"> <strong>C.</strong> Simple Active Directory (Simple AD)</label><br>
<label for="q158-d"><input type="radio" id="q158-d" name="q158" value="D"> <strong>D.</strong> Amazon Cloud Directory</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. AWS Directory Service for Microsoft Active Directory (AWS Managed Microsoft AD)

</details>

---

## Câu 159

**Chủ đề:** Design Secure Architectures

A financial services company has recently migrated from on-premises infrastructure to AWS Cloud. The DevOps team wants to implement a solution that allows all resource configurations to be reviewed and make sure that they meet compliance guidelines. Also, the solution should be able to offer the capability to look into the resource configuration history across the application stack.

As a solutions architect, which of the following solutions would you recommend to the team?

**Lựa chọn:**

<label for="q159-a"><input type="radio" id="q159-a" name="q159" value="A"> <strong>A.</strong> Use AWS Config to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes</label><br>
<label for="q159-b"><input type="radio" id="q159-b" name="q159" value="B"> <strong>B.</strong> Use Amazon CloudWatch to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes</label><br>
<label for="q159-c"><input type="radio" id="q159-c" name="q159" value="C"> <strong>C.</strong> Use AWS CloudTrail to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes</label><br>
<label for="q159-d"><input type="radio" id="q159-d" name="q159" value="D"> <strong>D.</strong> Use AWS Systems Manager to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS Config to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes

</details>

---

## Câu 160

**Chủ đề:** Design Cost-Optimized Architectures

A social media startup uses AWS Cloud to manage its IT infrastructure. The engineering team at the startup wants to perform weekly database rollovers for a MySQL database server using a serverless cron job that typically takes about 5 minutes to execute the database rollover script written in Python. The database rollover will archive the past week’s data from the production database to keep the database small while still keeping its data accessible.

As a solutions architect, which of the following would you recommend as the MOST cost-efficient and reliable solution?

**Lựa chọn:**

<label for="q160-a"><input type="radio" id="q160-a" name="q160" value="A"> <strong>A.</strong> Create a time-based schedule option within an AWS Glue job to invoke itself every week and run the database rollover script</label><br>
<label for="q160-b"><input type="radio" id="q160-b" name="q160" value="B"> <strong>B.</strong> Schedule a weekly Amazon EventBridge event cron expression to invoke an AWS Lambda function that runs the database rollover job</label><br>
<label for="q160-c"><input type="radio" id="q160-c" name="q160" value="C"> <strong>C.</strong> Provision an Amazon EC2 spot instance to run the database rollover script to be run via an OS-based weekly cron expression</label><br>
<label for="q160-d"><input type="radio" id="q160-d" name="q160" value="D"> <strong>D.</strong> Provision an Amazon EC2 scheduled reserved instance to run the database rollover script to be run via an OS-based weekly cron expression</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Schedule a weekly Amazon EventBridge event cron expression to invoke an AWS Lambda function that runs the database rollover job

</details>

---

## Câu 161

**Chủ đề:** Design High-Performing Architectures

A company has a hybrid cloud structure for its on-premises data center and AWS Cloud infrastructure. The company wants to build a web log archival solution such that only the most frequently accessed logs are available as cached data locally while backing up all logs on Amazon S3.

As a solutions architect, which of the following solutions would you recommend for this use-case?

**Lựa chọn:**

<label for="q161-a"><input type="radio" id="q161-a" name="q161" value="A"> <strong>A.</strong> Use AWS Direct Connect to store the most frequently accessed logs locally for low-latency access while storing the full backup of logs in an Amazon S3 bucket</label><br>
<label for="q161-b"><input type="radio" id="q161-b" name="q161" value="B"> <strong>B.</strong> Use AWS Volume Gateway - Stored Volume - to store the most frequently accessed logs locally for low-latency access while storing the full volume with all logs in its Amazon S3 service bucket</label><br>
<label for="q161-c"><input type="radio" id="q161-c" name="q161" value="C"> <strong>C.</strong> Use AWS Snowball Edge Storage Optimized device to store the most frequently accessed logs locally for low-latency access while storing the full backup of logs in an Amazon S3 bucket</label><br>
<label for="q161-d"><input type="radio" id="q161-d" name="q161" value="D"> <strong>D.</strong> Use AWS Volume Gateway - Cached Volume - to store the most frequently accessed logs locally for low-latency access while storing the full volume with all logs in its Amazon S3 service bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Volume Gateway - Cached Volume - to store the most frequently accessed logs locally for low-latency access while storing the full volume with all logs in its Amazon S3 service bucket

</details>

---

## Câu 162

**Chủ đề:** Design High-Performing Architectures

A financial services firm runs a containerized risk analytics tool in its on-premises data center using Docker. The tool depends on persistent data storage for maintaining customer simulation results and operates on a single host machine where the volume is locally mounted. The infrastructure team is looking to replatform the tool to AWS using a fully managed service because they want to avoid managing EC2 instances, volumes, or underlying servers.

Which AWS solution best meets these requirements?

**Lựa chọn:**

<label for="q162-a"><input type="radio" id="q162-a" name="q162" value="A"> <strong>A.</strong> Use Amazon ECS with Fargate launch type. Provision an Amazon Elastic File System (Amazon EFS) file system. Mount the EFS volume inside the container at runtime to provide persistent storage access</label><br>
<label for="q162-b"><input type="radio" id="q162-b" name="q162" value="B"> <strong>B.</strong> Use Amazon EKS with managed node groups. Provision an Amazon EBS volume and mount it inside the container by creating a Kubernetes persistent volume and claim. Manage storage lifecycle manually</label><br>
<label for="q162-c"><input type="radio" id="q162-c" name="q162" value="C"> <strong>C.</strong> Use Amazon ECS with Fargate launch type. Attach an Amazon S3 bucket using a shared access script that mounts the S3 bucket into the container for data storage</label><br>
<label for="q162-d"><input type="radio" id="q162-d" name="q162" value="D"> <strong>D.</strong> Use AWS Lambda with a container image runtime. Store stateful data in temporary local storage (/tmp) and sync with Amazon S3 periodically</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon ECS with Fargate launch type. Provision an Amazon Elastic File System (Amazon EFS) file system. Mount the EFS volume inside the container at runtime to provide persistent storage access

</details>

---

## Câu 163

**Chủ đề:** Design High-Performing Architectures

A company wants to improve its gaming application by adding a leaderboard that uses a complex proprietary algorithm based on the participating user's performance metrics to identify the top users on a real-time basis. The technical requirements mandate high elasticity, low latency, and real-time processing to deliver customizable user data for the community of users. The leaderboard would be accessed by millions of users simultaneously.

Which of the following options support the case for using Amazon ElastiCache to meet the given requirements? (Select two)

**Lựa chọn:**

<label for="q163-a"><input type="checkbox" id="q163-a" name="q163" value="A"> <strong>A.</strong> Use Amazon ElastiCache to improve latency and throughput for read-heavy application workloads</label><br>
<label for="q163-b"><input type="checkbox" id="q163-b" name="q163" value="B"> <strong>B.</strong> Use Amazon ElastiCache to improve latency and throughput for write-heavy application workloads</label><br>
<label for="q163-c"><input type="checkbox" id="q163-c" name="q163" value="C"> <strong>C.</strong> Use Amazon ElastiCache to improve the performance of Extract-Transform-Load (ETL) workloads</label><br>
<label for="q163-d"><input type="checkbox" id="q163-d" name="q163" value="D"> <strong>D.</strong> Use Amazon ElastiCache to improve the performance of compute-intensive workloads</label><br>
<label for="q163-e"><input type="checkbox" id="q163-e" name="q163" value="E"> <strong>E.</strong> Use Amazon ElastiCache to run highly complex JOIN queries</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon ElastiCache to improve latency and throughput for read-heavy application workloads

D. Use Amazon ElastiCache to improve the performance of compute-intensive workloads

</details>

---

## Câu 164

**Chủ đề:** Design Cost-Optimized Architectures

A financial services company is migrating their messaging queues from self-managed message-oriented middleware systems to Amazon Simple Queue Service (Amazon SQS). The development team at the company wants to minimize the costs of using Amazon SQS.

As a solutions architect, which of the following options would you recommend for the given use-case?

**Lựa chọn:**

<label for="q164-a"><input type="radio" id="q164-a" name="q164" value="A"> <strong>A.</strong> Use SQS short polling to retrieve messages from your Amazon SQS queues</label><br>
<label for="q164-b"><input type="radio" id="q164-b" name="q164" value="B"> <strong>B.</strong> Use SQS visibility timeout to retrieve messages from your Amazon SQS queues</label><br>
<label for="q164-c"><input type="radio" id="q164-c" name="q164" value="C"> <strong>C.</strong> Use SQS long polling to retrieve messages from your Amazon SQS queues</label><br>
<label for="q164-d"><input type="radio" id="q164-d" name="q164" value="D"> <strong>D.</strong> Use SQS message timer to retrieve messages from your Amazon SQS queues</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use SQS long polling to retrieve messages from your Amazon SQS queues

</details>

---

## Câu 165

**Chủ đề:** Design Secure Architectures

A retail company has connected its on-premises data center to the AWS Cloud via AWS Direct Connect. The company wants to be able to resolve Domain Name System (DNS) queries for any resources in the on-premises network from the AWS VPC and also resolve any DNS queries for resources in the AWS VPC from the on-premises network.

As a solutions architect, which of the following solutions can be combined to address the given use case? (Select two)

**Lựa chọn:**

<label for="q165-a"><input type="checkbox" id="q165-a" name="q165" value="A"> <strong>A.</strong> Create an outbound endpoint on Amazon Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Amazon Route 53 Resolver via this endpoint</label><br>
<label for="q165-b"><input type="checkbox" id="q165-b" name="q165" value="B"> <strong>B.</strong> Create an inbound endpoint on Amazon Route 53 Resolver and then Amazon Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint</label><br>
<label for="q165-c"><input type="checkbox" id="q165-c" name="q165" value="C"> <strong>C.</strong> Create a universal endpoint on Amazon Route 53 Resolver and then Amazon Route 53 Resolver can receive and forward queries to resolvers on the on-premises network via this endpoint</label><br>
<label for="q165-d"><input type="checkbox" id="q165-d" name="q165" value="D"> <strong>D.</strong> Create an inbound endpoint on Amazon Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Amazon Route 53 Resolver via this endpoint</label><br>
<label for="q165-e"><input type="checkbox" id="q165-e" name="q165" value="E"> <strong>E.</strong> Create an outbound endpoint on Amazon Route 53 Resolver and then Amazon Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Create an inbound endpoint on Amazon Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Amazon Route 53 Resolver via this endpoint

E. Create an outbound endpoint on Amazon Route 53 Resolver and then Amazon Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint

</details>

---

## Câu 166

**Chủ đề:** Design High-Performing Architectures

A company has set up AWS Organizations to manage several departments running their own AWS accounts. The departments operate from different countries and are spread across various AWS Regions. The company wants to set up a consistent resource provisioning process across departments so that each resource follows pre-defined configurations such as using a specific type of Amazon EC2 instances, specific IAM roles for AWS Lambda functions, etc.

As a solutions architect, which of the following options would you recommend for this use-case?

**Lựa chọn:**

<label for="q166-a"><input type="radio" id="q166-a" name="q166" value="A"> <strong>A.</strong> Use AWS CloudFormation StackSets to deploy the same template across AWS accounts and regions</label><br>
<label for="q166-b"><input type="radio" id="q166-b" name="q166" value="B"> <strong>B.</strong> Use AWS CloudFormation templates to deploy the same template across AWS accounts and regions</label><br>
<label for="q166-c"><input type="radio" id="q166-c" name="q166" value="C"> <strong>C.</strong> Use AWS CloudFormation stacks to deploy the same template across AWS accounts and regions</label><br>
<label for="q166-d"><input type="radio" id="q166-d" name="q166" value="D"> <strong>D.</strong> Use AWS Resource Access Manager (AWS RAM) to deploy the same template across AWS accounts and regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS CloudFormation StackSets to deploy the same template across AWS accounts and regions

</details>

---

## Câu 167

**Chủ đề:** Design High-Performing Architectures

A media startup is looking at hosting their web application on AWS Cloud. The application will be accessed by users from different geographic regions of the world to upload and download video files that can reach a maximum size of 10 gigabytes. The startup wants the solution to be cost-effective and scalable with the lowest possible latency for a great user experience.

As a Solutions Architect, which of the following will you suggest as an optimal solution to meet the given requirements?

**Lựa chọn:**

<label for="q167-a"><input type="radio" id="q167-a" name="q167" value="A"> <strong>A.</strong> Use Amazon S3 for hosting the web application and use Amazon CloudFront for faster distribution of content to geographically dispersed users</label><br>
<label for="q167-b"><input type="radio" id="q167-b" name="q167" value="B"> <strong>B.</strong> Use Amazon EC2 with AWS Global Accelerator for faster distribution of content, while using Amazon S3 as storage service</label><br>
<label for="q167-c"><input type="radio" id="q167-c" name="q167" value="C"> <strong>C.</strong> Use Amazon EC2 with Amazon ElastiCache for faster distribution of content, while Amazon S3 can be used as a storage service</label><br>
<label for="q167-d"><input type="radio" id="q167-d" name="q167" value="D"> <strong>D.</strong> Use Amazon S3 for hosting the web application and use Amazon S3 Transfer Acceleration (Amazon S3TA) to reduce the latency that geographically dispersed users might face</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon S3 for hosting the web application and use Amazon S3 Transfer Acceleration (Amazon S3TA) to reduce the latency that geographically dispersed users might face

</details>

---

## Câu 168

**Chủ đề:** Design Resilient Architectures

A startup has recently moved their monolithic web application to AWS Cloud. The application runs on a single Amazon EC2 instance. Currently, the user base is small and the startup does not want to spend effort on elaborate disaster recovery strategies or Auto Scaling Group. The application can afford a maximum downtime of 10 minutes.

In case of a failure, which of these options would you suggest as a cost-effective and automatic recovery procedure for the instance?

**Lựa chọn:**

<label for="q168-a"><input type="radio" id="q168-a" name="q168" value="A"> <strong>A.</strong> Configure Amazon EventBridge events that can trigger the recovery of the Amazon EC2 instance, in case the instance or the application fails</label><br>
<label for="q168-b"><input type="radio" id="q168-b" name="q168" value="B"> <strong>B.</strong> Configure an Amazon CloudWatch alarm that triggers the recovery of the Amazon EC2 instance, in case the instance fails. The instance can be configured with Amazon Elastic Block Store (Amazon EBS) or with instance store volumes</label><br>
<label for="q168-c"><input type="radio" id="q168-c" name="q168" value="C"> <strong>C.</strong> Configure an Amazon CloudWatch alarm that triggers the recovery of the Amazon EC2 instance, in case the instance fails. The instance, however, should only be configured with an Amazon EBS volume</label><br>
<label for="q168-d"><input type="radio" id="q168-d" name="q168" value="D"> <strong>D.</strong> Configure AWS Trusted Advisor to monitor the health check of Amazon EC2 instance and provide a remedial action in case an unhealthy flag is detected</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Configure an Amazon CloudWatch alarm that triggers the recovery of the Amazon EC2 instance, in case the instance fails. The instance, however, should only be configured with an Amazon EBS volume

</details>

---

## Câu 169

**Chủ đề:** Design Resilient Architectures

A legacy application is built using a tightly-coupled monolithic architecture. Due to a sharp increase in the number of users, the application performance has degraded. The company now wants to decouple the architecture and adopt AWS microservices architecture. Some of these microservices need to handle fast running processes whereas other microservices need to handle slower processes.

Which of these options would you identify as the right way of connecting these microservices?

**Lựa chọn:**

<label for="q169-a"><input type="radio" id="q169-a" name="q169" value="A"> <strong>A.</strong> Use Amazon Simple Notification Service (Amazon SNS) to decouple microservices running faster processes from the microservices running slower ones</label><br>
<label for="q169-b"><input type="radio" id="q169-b" name="q169" value="B"> <strong>B.</strong> Configure Amazon Kinesis Data Streams to decouple microservices running faster processes from the microservices running slower ones</label><br>
<label for="q169-c"><input type="radio" id="q169-c" name="q169" value="C"> <strong>C.</strong> Add Amazon EventBridge to decouple the complex architecture</label><br>
<label for="q169-d"><input type="radio" id="q169-d" name="q169" value="D"> <strong>D.</strong> Configure Amazon Simple Queue Service (Amazon SQS) queue to decouple microservices running faster processes from the microservices running slower ones</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Configure Amazon Simple Queue Service (Amazon SQS) queue to decouple microservices running faster processes from the microservices running slower ones

</details>

---

## Câu 170

**Chủ đề:** Design High-Performing Architectures

A small business has been running its IT systems on the on-premises infrastructure but the business now plans to migrate to AWS Cloud for operational efficiencies.

As a Solutions Architect, can you suggest a cost-effective serverless solution for its flagship application that has both static and dynamic content?

**Lựa chọn:**

<label for="q170-a"><input type="radio" id="q170-a" name="q170" value="A"> <strong>A.</strong> Host both the static and dynamic content of the web application on Amazon S3 and use Amazon CloudFront for distribution across diverse regions/countries</label><br>
<label for="q170-b"><input type="radio" id="q170-b" name="q170" value="B"> <strong>B.</strong> Host the static content on Amazon S3 and use AWS Lambda with Amazon DynamoDB for the serverless web application that handles dynamic content. Amazon CloudFront will sit in front of AWS Lambda for distribution across diverse regions</label><br>
<label for="q170-c"><input type="radio" id="q170-c" name="q170" value="C"> <strong>C.</strong> Host the static content on Amazon S3 and use Amazon EC2 with Amazon RDS for generating the dynamic content. Amazon CloudFront can be configured in front of Amazon EC2 instance, to make global distribution easy</label><br>
<label for="q170-d"><input type="radio" id="q170-d" name="q170" value="D"> <strong>D.</strong> Host both the static and dynamic content of the web application on Amazon EC2 with Amazon RDS as database. Amazon CloudFront should be configured to distribute the content across geographically disperse regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Host the static content on Amazon S3 and use AWS Lambda with Amazon DynamoDB for the serverless web application that handles dynamic content. Amazon CloudFront will sit in front of AWS Lambda for distribution across diverse regions

</details>

---

## Câu 171

**Chủ đề:** Design High-Performing Architectures

The application maintenance team at a company has noticed that the production application is very slow when the business reports are run on the Amazon RDS database. These reports fetch a large amount of data and have complex queries with multiple joins, spanning across multiple business-critical core tables. CPU, memory, and storage metrics are around 50% of the total capacity.

Can you recommend an improved and cost-effective way of generating the business reports while keeping the production application unaffected?

**Lựa chọn:**

<label for="q171-a"><input type="radio" id="q171-a" name="q171" value="A"> <strong>A.</strong> Increase the size of Amazon RDS instance</label><br>
<label for="q171-b"><input type="radio" id="q171-b" name="q171" value="B"> <strong>B.</strong> Migrate from General Purpose SSD to magnetic storage to enhance IOPS</label><br>
<label for="q171-c"><input type="radio" id="q171-c" name="q171" value="C"> <strong>C.</strong> Create a read replica and connect the report generation tool/application to it</label><br>
<label for="q171-d"><input type="radio" id="q171-d" name="q171" value="D"> <strong>D.</strong> Configure the Amazon RDS instance to be Multi-AZ DB instance, and connect the report generation tool to the DB instance in a different AZ</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Create a read replica and connect the report generation tool/application to it

</details>

---

## Câu 172

**Chủ đề:** Design High-Performing Architectures

An online gaming application has a large chunk of its traffic coming from users who download static assets such as historic leaderboard reports and the game tactics for various games. The current infrastructure and design are unable to cope up with the traffic and application freezes on most of the pages.

Which of the following is a cost-optimal solution that does not need provisioning of infrastructure?

**Lựa chọn:**

<label for="q172-a"><input type="radio" id="q172-a" name="q172" value="A"> <strong>A.</strong> Configure AWS Lambda with an Amazon RDS database to provide a serverless architecture</label><br>
<label for="q172-b"><input type="radio" id="q172-b" name="q172" value="B"> <strong>B.</strong> Use Amazon CloudFront with Amazon DynamoDB for greater speed and low latency access to static assets</label><br>
<label for="q172-c"><input type="radio" id="q172-c" name="q172" value="C"> <strong>C.</strong> Use AWS Lambda with Amazon ElastiCache and Amazon RDS for serving static assets at high speed and low latency</label><br>
<label for="q172-d"><input type="radio" id="q172-d" name="q172" value="D"> <strong>D.</strong> Use Amazon CloudFront with Amazon S3 as the storage solution for the static assets</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon CloudFront with Amazon S3 as the storage solution for the static assets

</details>

---

## Câu 173

**Chủ đề:** Design Resilient Architectures

An IT company hosts windows based applications on its on-premises data center. The company is looking at moving the business to the AWS Cloud. The cloud solution should offer shared storage space that multiple applications can access without a need for replication. Also, the solution should integrate with the company's self-managed Active Directory domain.

Which of the following solutions addresses these requirements with the minimal integration effort?

**Lựa chọn:**

<label for="q173-a"><input type="radio" id="q173-a" name="q173" value="A"> <strong>A.</strong> Use Amazon FSx for Windows File Server as a shared storage solution</label><br>
<label for="q173-b"><input type="radio" id="q173-b" name="q173" value="B"> <strong>B.</strong> Use File Gateway of AWS Storage Gateway to create a hybrid storage solution</label><br>
<label for="q173-c"><input type="radio" id="q173-c" name="q173" value="C"> <strong>C.</strong> Use Amazon FSx for Lustre as a shared storage solution with millisecond latencies</label><br>
<label for="q173-d"><input type="radio" id="q173-d" name="q173" value="D"> <strong>D.</strong> Use Amazon Elastic File System (Amazon EFS) as a shared storage solution</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon FSx for Windows File Server as a shared storage solution

</details>

---

## Câu 174

**Chủ đề:** Design Secure Architectures

A company has its application servers in the public subnet that connect to the database instances in the private subnet. For regular maintenance, the database instances need patch fixes that need to be downloaded from the internet.

Considering the company uses only IPv4 addressing and is looking for a fully managed service, which of the following would you suggest as an optimal solution?

**Lựa chọn:**

<label for="q174-a"><input type="radio" id="q174-a" name="q174" value="A"> <strong>A.</strong> Configure a Network Address Translation instance (NAT instance) in the public subnet of the VPC</label><br>
<label for="q174-b"><input type="radio" id="q174-b" name="q174" value="B"> <strong>B.</strong> Configure a Network Address Translation gateway (NAT gateway) in the public subnet of the VPC</label><br>
<label for="q174-c"><input type="radio" id="q174-c" name="q174" value="C"> <strong>C.</strong> Configure the Internet Gateway of the VPC to be accessible to the private subnet resources by changing the route tables</label><br>
<label for="q174-d"><input type="radio" id="q174-d" name="q174" value="D"> <strong>D.</strong> Configure an Egress-only internet gateway for the resources in the private subnet of the VPC</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure a Network Address Translation gateway (NAT gateway) in the public subnet of the VPC

</details>

---

## Câu 175

**Chủ đề:** Design High-Performing Architectures

A gaming company uses Application Load Balancers in front of Amazon EC2 instances for different services and microservices. The architecture has now become complex with too many Application Load Balancers in multiple AWS Regions. Security updates, firewall configurations, and traffic routing logic have become complex with too many IP addresses and configurations.

The company is looking at an easy and effective way to bring down the number of IP addresses allowed by the firewall and easily manage the entire network infrastructure. Which of these options represents an appropriate solution for this requirement?

**Lựa chọn:**

<label for="q175-a"><input type="radio" id="q175-a" name="q175" value="A"> <strong>A.</strong> Configure Elastic IPs for each of the Application Load Balancers in each Region</label><br>
<label for="q175-b"><input type="radio" id="q175-b" name="q175" value="B"> <strong>B.</strong> Set up a Network Load Balancer with elastic IP address. Register the private IPs of all the Application Load Balancers as targets of this Network Load Balancer</label><br>
<label for="q175-c"><input type="radio" id="q175-c" name="q175" value="C"> <strong>C.</strong> Launch AWS Global Accelerator and create endpoints for all the Regions. Register the Application Load Balancers of each Region to the corresponding endpoints</label><br>
<label for="q175-d"><input type="radio" id="q175-d" name="q175" value="D"> <strong>D.</strong> Assign an Elastic IP to an Auto Scaling Group (ASG), and set up multiple Amazon EC2 instances to run behind the Auto Scaling Groups, for each of the Regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Launch AWS Global Accelerator and create endpoints for all the Regions. Register the Application Load Balancers of each Region to the corresponding endpoints

</details>

---

## Câu 176

**Chủ đề:** Design Resilient Architectures

A health care application processes the real-time health data of the patients into an analytics workflow. With a sharp increase in the number of users, the system has become slow and sometimes even unresponsive as it does not have a retry mechanism. The startup is looking at a scalable solution that has minimal implementation overhead.

Which of the following would you recommend as a scalable alternative to the current solution?

**Lựa chọn:**

<label for="q176-a"><input type="radio" id="q176-a" name="q176" value="A"> <strong>A.</strong> Use Amazon Simple Notification Service (Amazon SNS) for data ingestion and configure AWS Lambda to trigger logic for downstream processing</label><br>
<label for="q176-b"><input type="radio" id="q176-b" name="q176" value="B"> <strong>B.</strong> Use Amazon Simple Queue Service (Amazon SQS) for data ingestion and configure AWS Lambda to trigger logic for downstream processing</label><br>
<label for="q176-c"><input type="radio" id="q176-c" name="q176" value="C"> <strong>C.</strong> Use Amazon API Gateway with the existing REST-based interface to create a high performing architecture</label><br>
<label for="q176-d"><input type="radio" id="q176-d" name="q176" value="D"> <strong>D.</strong> Use Amazon Kinesis Data Streams to ingest the data, process it using AWS Lambda or run analytics using Amazon Kinesis Data Analytics</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon Kinesis Data Streams to ingest the data, process it using AWS Lambda or run analytics using Amazon Kinesis Data Analytics

</details>

---

## Câu 177

**Chủ đề:** Design Cost-Optimized Architectures

An e-commerce company has deployed its application on several Amazon EC2 instances that are configured in a private subnet using IPv4. These Amazon EC2 instances read and write a huge volume of data to and from Amazon S3 in the same AWS region. The company has set up subnet routing to direct all the internet-bound traffic through a Network Address Translation gateway (NAT gateway). The company wants to build the most cost-optimal solution without impacting the application's ability to communicate with Amazon S3 or the internet.

As an AWS Certified Solutions Architect Associate, which of the following would you recommend?

**Lựa chọn:**

<label for="q177-a"><input type="radio" id="q177-a" name="q177" value="A"> <strong>A.</strong> Set up a VPC gateway endpoint for Amazon S3. Attach an endpoint policy to the endpoint. Update the route table to direct the S3-bound traffic to the VPC endpoint</label><br>
<label for="q177-b"><input type="radio" id="q177-b" name="q177" value="B"> <strong>B.</strong> Provision an internet gateway. Update the route table in the private subnet to route traffic to the internet gateway. Update the network ACL (NACL) to allow the S3-bound traffic</label><br>
<label for="q177-c"><input type="radio" id="q177-c" name="q177" value="C"> <strong>C.</strong> Set up an egress-only internet gateway in the public subnet. Update the route table in the private subnet to route traffic to the internet gateway. Update the network ACL to allow the S3-bound traffic</label><br>
<label for="q177-d"><input type="radio" id="q177-d" name="q177" value="D"> <strong>D.</strong> Set up a Gateway Load Balancer (GWLB) endpoint for Amazon S3. Update the route table in the private subnet to direct the S3-bound traffic via the Gateway Load Balancer (GWLB) endpoint</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Set up a VPC gateway endpoint for Amazon S3. Attach an endpoint policy to the endpoint. Update the route table to direct the S3-bound traffic to the VPC endpoint

</details>

---

## Câu 178

**Chủ đề:** Design Cost-Optimized Architectures

An IT training company hosted its website on Amazon S3 a couple of years ago. Due to COVID-19 related travel restrictions, the training website has suddenly gained traction. With an almost 300% increase in the requests served per day, the company's AWS costs have sky-rocketed for just the Amazon S3 outbound data costs.

As a Solutions Architect, can you suggest an alternate method to reduce costs while keeping the latency low?

**Lựa chọn:**

<label for="q178-a"><input type="radio" id="q178-a" name="q178" value="A"> <strong>A.</strong> To reduce Amazon S3 cost, the data can be saved on an Amazon EBS volume connected to an Amazon EC2 instance that can host the application</label><br>
<label for="q178-b"><input type="radio" id="q178-b" name="q178" value="B"> <strong>B.</strong> Use Amazon EFS service, as it provides a shared, scalable, fully managed elastic NFS file system for storing AWS Cloud or on-premises data</label><br>
<label for="q178-c"><input type="radio" id="q178-c" name="q178" value="C"> <strong>C.</strong> Configure Amazon CloudFront to distribute the data hosted on Amazon S3 cost-effectively</label><br>
<label for="q178-d"><input type="radio" id="q178-d" name="q178" value="D"> <strong>D.</strong> Configure Amazon S3 Batch Operations to read data in bulk at one go, to reduce the number of calls made to Amazon S3 buckets</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Configure Amazon CloudFront to distribute the data hosted on Amazon S3 cost-effectively

</details>

---

## Câu 179

**Chủ đề:** Design Resilient Architectures

A data analytics company manages an application that stores user data in a Amazon DynamoDB table. The development team has observed that once in a while, the application writes corrupted data in the Amazon DynamoDB table. As soon as the issue is detected, the team needs to remove the corrupted data at the earliest.

What do you recommend?

**Lựa chọn:**

<label for="q179-a"><input type="radio" id="q179-a" name="q179" value="A"> <strong>A.</strong> Configure the Amazon DynamoDB table as a global table and point the application to use the table from another AWS region that has no corrupted data</label><br>
<label for="q179-b"><input type="radio" id="q179-b" name="q179" value="B"> <strong>B.</strong> Use Amazon DynamoDB Streams to restore the table to the state just before corrupted data was written</label><br>
<label for="q179-c"><input type="radio" id="q179-c" name="q179" value="C"> <strong>C.</strong> Use Amazon DynamoDB on-demand backup to restore the table to the state just before corrupted data was written</label><br>
<label for="q179-d"><input type="radio" id="q179-d" name="q179" value="D"> <strong>D.</strong> Use Amazon DynamoDB point in time recovery to restore the table to the state just before corrupted data was written</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon DynamoDB point in time recovery to restore the table to the state just before corrupted data was written

</details>

---

## Câu 180

**Chủ đề:** Design High-Performing Architectures

The database backend for a retail company's website is hosted on Amazon RDS for MySQL having a primary instance and three read replicas to support read scalability. The company has mandated that the read replicas should lag no more than 1 second behind the primary instance to provide the best possible user experience. The read replicas are falling further behind during periods of peak traffic spikes, resulting in a bad user experience as the searches produce inconsistent results.

You have been hired as an AWS Certified Solutions Architect - Associate to reduce the replication lag as much as possible with minimal changes to the application code or the effort required to manage the underlying resources.

Which of the following will you recommend?

**Lựa chọn:**

<label for="q180-a"><input type="radio" id="q180-a" name="q180" value="A"> <strong>A.</strong> Host the MySQL primary database on a memory-optimized Amazon EC2 instance. Spin up additional compute-optimized Amazon EC2 instances to host the read replicas</label><br>
<label for="q180-b"><input type="radio" id="q180-b" name="q180" value="B"> <strong>B.</strong> Set up an Amazon ElastiCache for Redis cluster in front of the MySQL database. Update the website to check the cache before querying the read replicas</label><br>
<label for="q180-c"><input type="radio" id="q180-c" name="q180" value="C"> <strong>C.</strong> Set up database migration from Amazon RDS MySQL to Amazon DynamoDB. Provision a large number of read capacity units (RCUs) to support the required throughput and enable Auto-Scaling</label><br>
<label for="q180-d"><input type="radio" id="q180-d" name="q180" value="D"> <strong>D.</strong> Set up database migration from Amazon RDS MySQL to Amazon Aurora MySQL. Swap out the MySQL read replicas with Aurora Replicas. Configure Aurora Auto Scaling</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up database migration from Amazon RDS MySQL to Amazon Aurora MySQL. Swap out the MySQL read replicas with Aurora Replicas. Configure Aurora Auto Scaling

</details>

---

## Câu 181

**Chủ đề:** Design Cost-Optimized Architectures

The development team at a retail company wants to optimize the cost of Amazon EC2 instances. The team wants to move certain nightly batch jobs to spot instances. The team has hired you as a solutions architect to provide the initial guidance.

Which of the following would you identify as CORRECT regarding the capabilities of spot instances? (Select three)

**Lựa chọn:**

<label for="q181-a"><input type="checkbox" id="q181-a" name="q181" value="A"> <strong>A.</strong> When you cancel an active spot request, it terminates the associated instance as well</label><br>
<label for="q181-b"><input type="checkbox" id="q181-b" name="q181" value="B"> <strong>B.</strong> If a spot request is persistent, then it is opened again after your Spot Instance is interrupted</label><br>
<label for="q181-c"><input type="checkbox" id="q181-c" name="q181" value="C"> <strong>C.</strong> If a spot request is persistent, then it is opened again after you stop the Spot Instance</label><br>
<label for="q181-d"><input type="checkbox" id="q181-d" name="q181" value="D"> <strong>D.</strong> Spot Fleets can maintain target capacity by launching replacement instances after Spot Instances in the fleet are terminated</label><br>
<label for="q181-e"><input type="checkbox" id="q181-e" name="q181" value="E"> <strong>E.</strong> When you cancel an active spot request, it does not terminate the associated instance</label><br>
<label for="q181-f"><input type="checkbox" id="q181-f" name="q181" value="F"> <strong>F.</strong> Spot Fleets cannot maintain target capacity by launching replacement instances after Spot Instances in the fleet are terminated</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. If a spot request is persistent, then it is opened again after your Spot Instance is interrupted

D. Spot Fleets can maintain target capacity by launching replacement instances after Spot Instances in the fleet are terminated

E. When you cancel an active spot request, it does not terminate the associated instance

</details>

---

## Câu 182

**Chủ đề:** Design High-Performing Architectures

A startup is building a serverless microservices architecture where client applications (web and mobile) authenticate users via a third-party OIDC-compliant identity provider. The backend APIs must validate JSON Web Tokens (JWTs) issued by this provider, enforce scope-based access control, and be cost-effective with minimal latency. The development team wants to use a fully managed service that supports JWT validation natively, without writing custom authentication logic.

Which solution should the team implement to meet these requirements?

**Lựa chọn:**

<label for="q182-a"><input type="radio" id="q182-a" name="q182" value="A"> <strong>A.</strong> Use Amazon API Gateway HTTP API with a native JWT authorizer configured to validate tokens from the OIDC provider</label><br>
<label for="q182-b"><input type="radio" id="q182-b" name="q182" value="B"> <strong>B.</strong> Use Amazon API Gateway REST API with a Lambda function that manually validates JWT tokens</label><br>
<label for="q182-c"><input type="radio" id="q182-c" name="q182" value="C"> <strong>C.</strong> Use Amazon API Gateway WebSocket API with JWT claims validated by a Lambda authorizer</label><br>
<label for="q182-d"><input type="radio" id="q182-d" name="q182" value="D"> <strong>D.</strong> Deploy a gRPC backend on Amazon ECS Fargate and expose it through AWS App Runner, handling JWT validation inside the containerized services</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon API Gateway HTTP API with a native JWT authorizer configured to validate tokens from the OIDC provider

</details>

---

## Câu 183

**Chủ đề:** Design High-Performing Architectures

A media streaming startup is building a set of backend APIs that will be consumed by external mobile applications. To prevent API abuse, protect downstream resources, and ensure fair usage across clients, the architecture must enforce rate limiting and throttling on a per-client basis. The team also wants to define usage quotas and apply different limits to different API consumers.

Which solution should the team implement to enforce rate limiting and usage quotas at the API layer?

**Lựa chọn:**

<label for="q183-a"><input type="radio" id="q183-a" name="q183" value="A"> <strong>A.</strong> Use an Application Load Balancer (ALB) with path-based routing and configure listener rules to enforce request limits</label><br>
<label for="q183-b"><input type="radio" id="q183-b" name="q183" value="B"> <strong>B.</strong> Use Amazon API Gateway and configure usage plans with API keys to apply rate limits and quotas per client</label><br>
<label for="q183-c"><input type="radio" id="q183-c" name="q183" value="C"> <strong>C.</strong> Use a Gateway Load Balancer to inspect and control incoming HTTP traffic and throttle requests by integrating with third-party firewall appliances</label><br>
<label for="q183-d"><input type="radio" id="q183-d" name="q183" value="D"> <strong>D.</strong> Use a Network Load Balancer (NLB) to terminate TLS and apply rate-limiting logic within backend EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon API Gateway and configure usage plans with API keys to apply rate limits and quotas per client

</details>

---

## Câu 184

**Chủ đề:** Design Secure Architectures

An e-commerce company runs its web application on Amazon EC2 instances in an Auto Scaling group and it's configured to handle consumer orders in an Amazon Simple Queue Service (Amazon SQS) queue for downstream processing. The DevOps team has observed that the performance of the application goes down in case of a sudden spike in orders received.

As a solutions architect, which of the following solutions would you recommend to address this use-case?

**Lựa chọn:**

<label for="q184-a"><input type="radio" id="q184-a" name="q184" value="A"> <strong>A.</strong> Use a target tracking scaling policy based on a custom Amazon SQS queue metric</label><br>
<label for="q184-b"><input type="radio" id="q184-b" name="q184" value="B"> <strong>B.</strong> Use a simple scaling policy based on a custom Amazon SQS queue metric</label><br>
<label for="q184-c"><input type="radio" id="q184-c" name="q184" value="C"> <strong>C.</strong> Use a step scaling policy based on a custom Amazon SQS queue metric</label><br>
<label for="q184-d"><input type="radio" id="q184-d" name="q184" value="D"> <strong>D.</strong> Use a scheduled scaling policy based on a custom Amazon SQS queue metric</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use a target tracking scaling policy based on a custom Amazon SQS queue metric

</details>

---

## Câu 185

**Chủ đề:** Design Secure Architectures

The DevOps team at a multi-national company is helping its subsidiaries standardize Amazon EC2 instances by using the same Amazon Machine Image (AMI). Some of these subsidiaries are in the same AWS region but use different AWS accounts whereas others are in different AWS regions but use the same AWS account as the parent company. The DevOps team has hired you as a solutions architect for this project.

Which of the following would you identify as CORRECT regarding the capabilities of an Amazon Machine Image (AMI)? (Select three)

**Lựa chọn:**

<label for="q185-a"><input type="checkbox" id="q185-a" name="q185" value="A"> <strong>A.</strong> You cannot copy an Amazon Machine Image (AMI) across AWS Regions</label><br>
<label for="q185-b"><input type="checkbox" id="q185-b" name="q185" value="B"> <strong>B.</strong> You cannot share an Amazon Machine Image (AMI) with another AWS account</label><br>
<label for="q185-c"><input type="checkbox" id="q185-c" name="q185" value="C"> <strong>C.</strong> Copying an Amazon Machine Image (AMI) backed by an encrypted snapshot results in an unencrypted target snapshot</label><br>
<label for="q185-d"><input type="checkbox" id="q185-d" name="q185" value="D"> <strong>D.</strong> You can copy an Amazon Machine Image (AMI) across AWS Regions</label><br>
<label for="q185-e"><input type="checkbox" id="q185-e" name="q185" value="E"> <strong>E.</strong> You can share an Amazon Machine Image (AMI) with another AWS account</label><br>
<label for="q185-f"><input type="checkbox" id="q185-f" name="q185" value="F"> <strong>F.</strong> Copying an Amazon Machine Image (AMI) backed by an encrypted snapshot cannot result in an unencrypted target snapshot</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. You can copy an Amazon Machine Image (AMI) across AWS Regions

E. You can share an Amazon Machine Image (AMI) with another AWS account

F. Copying an Amazon Machine Image (AMI) backed by an encrypted snapshot cannot result in an unencrypted target snapshot

</details>

---

## Câu 186

**Chủ đề:** Design Resilient Architectures

A financial services company wants to move the Windows file server clusters out of their datacenters. They are looking for cloud file storage offerings that provide full Windows compatibility. Can you identify the AWS storage services that provide highly reliable file storage that is accessible over the industry-standard Server Message Block (SMB) protocol compatible with Windows systems? (Select two)

**Lựa chọn:**

<label for="q186-a"><input type="checkbox" id="q186-a" name="q186" value="A"> <strong>A.</strong> Amazon Elastic File System (Amazon EFS)</label><br>
<label for="q186-b"><input type="checkbox" id="q186-b" name="q186" value="B"> <strong>B.</strong> Amazon Elastic Block Store (Amazon EBS)</label><br>
<label for="q186-c"><input type="checkbox" id="q186-c" name="q186" value="C"> <strong>C.</strong> Amazon FSx for Windows File Server</label><br>
<label for="q186-d"><input type="checkbox" id="q186-d" name="q186" value="D"> <strong>D.</strong> Amazon Simple Storage Service (Amazon S3)</label><br>
<label for="q186-e"><input type="checkbox" id="q186-e" name="q186" value="E"> <strong>E.</strong> File Gateway Configuration of AWS Storage Gateway</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Amazon FSx for Windows File Server

E. File Gateway Configuration of AWS Storage Gateway

</details>

---

## Câu 187

**Chủ đề:** Design Resilient Architectures

The engineering team at a social media company wants to use Amazon CloudWatch alarms to automatically recover Amazon EC2 instances if they become impaired. The team has hired you as a solutions architect to provide subject matter expertise.

As a solutions architect, which of the following statements would you identify as CORRECT regarding this automatic recovery process? (Select two)

**Lựa chọn:**

<label for="q187-a"><input type="checkbox" id="q187-a" name="q187" value="A"> <strong>A.</strong> Terminated Amazon EC2 instances can be recovered if they are configured at the launch of instance</label><br>
<label for="q187-b"><input type="checkbox" id="q187-b" name="q187" value="B"> <strong>B.</strong> A recovered instance is identical to the original instance, including the instance ID, private IP addresses, Elastic IP addresses, and all instance metadata</label><br>
<label for="q187-c"><input type="checkbox" id="q187-c" name="q187" value="C"> <strong>C.</strong> If your instance has a public IPv4 address, it retains the public IPv4 address after recovery</label><br>
<label for="q187-d"><input type="checkbox" id="q187-d" name="q187" value="D"> <strong>D.</strong> During instance recovery, the instance is migrated during an instance reboot, and any data that is in-memory is retained</label><br>
<label for="q187-e"><input type="checkbox" id="q187-e" name="q187" value="E"> <strong>E.</strong> If your instance has a public IPv4 address, it does not retain the public IPv4 address after recovery</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. A recovered instance is identical to the original instance, including the instance ID, private IP addresses, Elastic IP addresses, and all instance metadata

C. If your instance has a public IPv4 address, it retains the public IPv4 address after recovery

</details>

---

## Câu 188

**Chủ đề:** Design Secure Architectures

A regional transportation authority operates a high-traffic public information portal hosted on AWS. The backend consists of Amazon EC2 instances behind an Application Load Balancer (ALB). In recent weeks, the operations team has observed intermittent slowdowns and performance issues. After investigation, the team suspect the application is being targeted by distributed denial-of-service (DDoS) attacks coming from a wide range of IP addresses. The team needs a solution that provides DDoS mitigation, detailed logs for audit purposes, and requires minimal changes to the existing architecture.

Which solution best addresses these needs?

**Lựa chọn:**

<label for="q188-a"><input type="radio" id="q188-a" name="q188" value="A"> <strong>A.</strong> Deploy Amazon GuardDuty and integrate with the EC2 environment. Use GuardDuty findings to manually block suspected IP addresses at the ALB level or within EC2 security groups</label><br>
<label for="q188-b"><input type="radio" id="q188-b" name="q188" value="B"> <strong>B.</strong> Enable Amazon Inspector for the EC2 instances. Use its vulnerability findings to detect potential DDoS attack vectors and patch the EC2 environments accordingly</label><br>
<label for="q188-c"><input type="radio" id="q188-c" name="q188" value="C"> <strong>C.</strong> Subscribe to AWS Shield Advanced to gain proactive DDoS protection. Engage the AWS DDoS Response Team (DRT) to analyze traffic patterns and apply mitigations. Use the built-in logging and reporting to maintain an audit trail of detected events</label><br>
<label for="q188-d"><input type="radio" id="q188-d" name="q188" value="D"> <strong>D.</strong> Create an Amazon CloudFront distribution in front of the ALB. Enable AWS WAF on the distribution and configure custom rules to filter traffic from known malicious IP ranges and geographies. Use CloudFront access logs for analysis</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Subscribe to AWS Shield Advanced to gain proactive DDoS protection. Engage the AWS DDoS Response Team (DRT) to analyze traffic patterns and apply mitigations. Use the built-in logging and reporting to maintain an audit trail of detected events

</details>

---

## Câu 189

**Chủ đề:** Design Secure Architectures

An AWS Organization is using Service Control Policies (SCPs) for central control over the maximum available permissions for all accounts in their organization. This allows the organization to ensure that all accounts stay within the organization’s access control guidelines.

Which of the given scenarios are correct regarding the permissions described below? (Select three)

**Lựa chọn:**

<label for="q189-a"><input type="checkbox" id="q189-a" name="q189" value="A"> <strong>A.</strong> If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable service control policy (SCP), the user or role can't perform that action</label><br>
<label for="q189-b"><input type="checkbox" id="q189-b" name="q189" value="B"> <strong>B.</strong> If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable service control policy (SCP), the user or role can still perform that action</label><br>
<label for="q189-c"><input type="checkbox" id="q189-c" name="q189" value="C"> <strong>C.</strong> Service control policy (SCP) affects all users and roles in the member accounts, including root user of the member accounts</label><br>
<label for="q189-d"><input type="checkbox" id="q189-d" name="q189" value="D"> <strong>D.</strong> Service control policy (SCP) affects all users and roles in the member accounts, excluding root user of the member accounts</label><br>
<label for="q189-e"><input type="checkbox" id="q189-e" name="q189" value="E"> <strong>E.</strong> Service control policy (SCP) affects service-linked roles</label><br>
<label for="q189-f"><input type="checkbox" id="q189-f" name="q189" value="F"> <strong>F.</strong> Service control policy (SCP) does not affect service-linked role</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable service control policy (SCP), the user or role can't perform that action

C. Service control policy (SCP) affects all users and roles in the member accounts, including root user of the member accounts

F. Service control policy (SCP) does not affect service-linked role

</details>

---

## Câu 190

**Chủ đề:** Design Secure Architectures

The engineering team at a company is moving the static content from the company's logistics website hosted on Amazon EC2 instances to an Amazon S3 bucket. The team wants to use an Amazon CloudFront distribution to deliver the static content. The security group used by the Amazon EC2 instances allows the website to be accessed by a limited set of IP ranges from the company's suppliers. Post-migration to Amazon CloudFront, access to the static content should only be allowed from the aforementioned IP addresses.

Which options would you combine to build a solution to meet these requirements? (Select two)

**Lựa chọn:**

<label for="q190-a"><input type="checkbox" id="q190-a" name="q190" value="A"> <strong>A.</strong> Create an AWS Web Application Firewall (AWS WAF) ACL and use an IP match condition to allow traffic only from those IPs that are allowed in the Amazon EC2 security group. Associate this new AWS WAF ACL with the Amazon S3 bucket policy</label><br>
<label for="q190-b"><input type="checkbox" id="q190-b" name="q190" value="B"> <strong>B.</strong> Create a new NACL that allows traffic from the same IPs as specified in the current Amazon EC2 security group. Associate this new NACL with the Amazon CloudFront distribution</label><br>
<label for="q190-c"><input type="checkbox" id="q190-c" name="q190" value="C"> <strong>C.</strong> Create a new security group that allows traffic from the same IPs as specified in the current Amazon EC2 security group. Associate this new security group with the Amazon CloudFront distribution</label><br>
<label for="q190-d"><input type="checkbox" id="q190-d" name="q190" value="D"> <strong>D.</strong> Configure an origin access identity (OAI) and associate it with the Amazon CloudFront distribution. Set up the permissions in the Amazon S3 bucket policy so that only the OAI can read the objects</label><br>
<label for="q190-e"><input type="checkbox" id="q190-e" name="q190" value="E"> <strong>E.</strong> Create an AWS WAF ACL and use an IP match condition to allow traffic only from those IPs that are allowed in the Amazon EC2 security group. Associate this new AWS WAF ACL with the Amazon CloudFront distribution</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Configure an origin access identity (OAI) and associate it with the Amazon CloudFront distribution. Set up the permissions in the Amazon S3 bucket policy so that only the OAI can read the objects

E. Create an AWS WAF ACL and use an IP match condition to allow traffic only from those IPs that are allowed in the Amazon EC2 security group. Associate this new AWS WAF ACL with the Amazon CloudFront distribution

</details>

---

## Câu 191

**Chủ đề:** Design High-Performing Architectures

A company is migrating a legacy workload from on premises to AWS. The application receives customer order files from an on premises ERP system by using the SFTP protocol. After files arrive, the application must process them immediately rather than relying on periodic polling. The company already has secure network connectivity between AWS and the on premises environment. The new solution must remain highly available, secure, and resilient across infrastructure failures.

Which solution should you implement to meet these requirements?

**Lựa chọn:**

<label for="q191-a"><input type="radio" id="q191-a" name="q191" value="A"> <strong>A.</strong> Deploy an internal AWS Transfer Family SFTP server across two Availability Zones backed by Amazon S3. Configure a Transfer Family managed workflow to invoke an AWS Lambda function immediately after file upload completes</label><br>
<label for="q191-b"><input type="radio" id="q191-b" name="q191" value="B"> <strong>B.</strong> Deploy an internal AWS Transfer Family SFTP server across two Availability Zones backed by Amazon EFS. Use Amazon EventBridge Scheduler to periodically trigger an AWS Step Functions state machine that scans for new files</label><br>
<label for="q191-c"><input type="radio" id="q191-c" name="q191" value="C"> <strong>C.</strong> Deploy an internet facing AWS Transfer Family SFTP server in a single Availability Zone backed by Amazon EFS. Configure a Transfer Family managed workflow to invoke an AWS Lambda function after file upload completes</label><br>
<label for="q191-d"><input type="radio" id="q191-d" name="q191" value="D"> <strong>D.</strong> Deploy an internet facing AWS Transfer Family SFTP server across two Availability Zones backed by Amazon S3. Configure Amazon S3 Event Notifications to invoke an AWS Lambda function when new objects are created</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy an internal AWS Transfer Family SFTP server across two Availability Zones backed by Amazon S3. Configure a Transfer Family managed workflow to invoke an AWS Lambda function immediately after file upload completes

</details>

---

## Câu 192

**Chủ đề:** Design Secure Architectures

An engineering lead is designing a VPC with public and private subnets. The VPC and subnets use IPv4 CIDR blocks. There is one public subnet and one private subnet in each of three Availability Zones (AZs) for high availability. An internet gateway is used to provide internet access for the public subnets. The private subnets require access to the internet to allow Amazon EC2 instances to download software updates.

Which of the following options represents the correct solution to set up internet access for the private subnets?

**Lựa chọn:**

<label for="q192-a"><input type="radio" id="q192-a" name="q192" value="A"> <strong>A.</strong> Set up three NAT gateways, one in each private subnet in each AZ. Create a custom route table for each AZ that forwards non-local traffic to the NAT gateway in its AZ</label><br>
<label for="q192-b"><input type="radio" id="q192-b" name="q192" value="B"> <strong>B.</strong> Set up three Internet gateways, one in each private subnet in each AZ. Create a custom route table for each AZ that forwards non-local traffic to the Internet gateway in its AZ</label><br>
<label for="q192-c"><input type="radio" id="q192-c" name="q192" value="C"> <strong>C.</strong> Set up three NAT gateways, one in each public subnet in each AZ. Create a custom route table for each AZ that forwards non-local traffic to the NAT gateway in its AZ</label><br>
<label for="q192-d"><input type="radio" id="q192-d" name="q192" value="D"> <strong>D.</strong> Set up three egress-only internet gateways, one in each public subnet in each AZ. Create a custom route table for each AZ that forwards non-local traffic to the egress-only internet gateway in its AZ</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set up three NAT gateways, one in each public subnet in each AZ. Create a custom route table for each AZ that forwards non-local traffic to the NAT gateway in its AZ

</details>

---

## Câu 193

**Chủ đề:** Design Resilient Architectures

A company recently experienced a database outage in its on-premises data center. The company now wants to migrate to a reliable database solution on AWS that minimizes data loss and stores every transaction on at least two nodes.

Which of the following solutions meets these requirements?

**Lựa chọn:**

<label for="q193-a"><input type="radio" id="q193-a" name="q193" value="A"> <strong>A.</strong> Set up an Amazon RDS MySQL DB instance and then create a read replica in another Availability Zone that synchronously replicates the data</label><br>
<label for="q193-b"><input type="radio" id="q193-b" name="q193" value="B"> <strong>B.</strong> Set up an Amazon RDS MySQL DB instance and then create a read replica in a separate AWS Region that synchronously replicates the data</label><br>
<label for="q193-c"><input type="radio" id="q193-c" name="q193" value="C"> <strong>C.</strong> Set up an Amazon RDS MySQL DB instance with Multi-AZ functionality enabled to synchronously replicate the data</label><br>
<label for="q193-d"><input type="radio" id="q193-d" name="q193" value="D"> <strong>D.</strong> Set up an Amazon EC2 instance with a MySQL DB engine installed that triggers an AWS Lambda function to synchronously replicate the data to an Amazon RDS MySQL DB instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set up an Amazon RDS MySQL DB instance with Multi-AZ functionality enabled to synchronously replicate the data

</details>

---

## Câu 194

**Chủ đề:** Design Cost-Optimized Architectures

Your application is hosted by a provider on yourapp.provider.com. You would like to have your users access your application using www.your-domain.com, which you own and manage under Amazon Route 53.

Which Amazon Route 53 record should you create?

**Lựa chọn:**

<label for="q194-a"><input type="radio" id="q194-a" name="q194" value="A"> <strong>A.</strong> Create an A record</label><br>
<label for="q194-b"><input type="radio" id="q194-b" name="q194" value="B"> <strong>B.</strong> Create a CNAME record</label><br>
<label for="q194-c"><input type="radio" id="q194-c" name="q194" value="C"> <strong>C.</strong> Create a PTR record</label><br>
<label for="q194-d"><input type="radio" id="q194-d" name="q194" value="D"> <strong>D.</strong> Create an Alias Record</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create a CNAME record

</details>

---

## Câu 195

**Chủ đề:** Design Secure Architectures

The DevOps team at an IT company has recently migrated to AWS and they are configuring security groups for their two-tier application with public web servers and private database servers. The team wants to understand the allowed configuration options for an inbound rule for a security group.

As a solutions architect, which of the following would you identify as an INVALID option for setting up such a configuration?

**Lựa chọn:**

<label for="q195-a"><input type="radio" id="q195-a" name="q195" value="A"> <strong>A.</strong> You can use a security group as the custom source for the inbound rule</label><br>
<label for="q195-b"><input type="radio" id="q195-b" name="q195" value="B"> <strong>B.</strong> You can use a range of IP addresses in CIDR block notation as the custom source for the inbound rule</label><br>
<label for="q195-c"><input type="radio" id="q195-c" name="q195" value="C"> <strong>C.</strong> You can use an IP address as the custom source for the inbound rule</label><br>
<label for="q195-d"><input type="radio" id="q195-d" name="q195" value="D"> <strong>D.</strong> You can use an Internet Gateway ID as the custom source for the inbound rule</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. You can use an Internet Gateway ID as the custom source for the inbound rule

</details>

---

## Câu 196

**Chủ đề:** Design Resilient Architectures

Your company is deploying a website running on AWS Elastic Beanstalk. The website takes over 45 minutes for the installation and contains both static as well as dynamic files that must be generated during the installation process.

As a Solutions Architect, you would like to bring the time to create a new instance in your AWS Elastic Beanstalk deployment to be less than 2 minutes. Which of the following options should be combined to build a solution for this requirement? (Select two)

**Lựa chọn:**

<label for="q196-a"><input type="checkbox" id="q196-a" name="q196" value="A"> <strong>A.</strong> Use Amazon EC2 user data to customize the dynamic installation parts at boot time</label><br>
<label for="q196-b"><input type="checkbox" id="q196-b" name="q196" value="B"> <strong>B.</strong> Create a Golden Amazon Machine Image (AMI) with the static installation components already setup</label><br>
<label for="q196-c"><input type="checkbox" id="q196-c" name="q196" value="C"> <strong>C.</strong> Store the installation files in Amazon S3 so they can be quickly retrieved</label><br>
<label for="q196-d"><input type="checkbox" id="q196-d" name="q196" value="D"> <strong>D.</strong> Use Amazon EC2 user data to install the application at boot time</label><br>
<label for="q196-e"><input type="checkbox" id="q196-e" name="q196" value="E"> <strong>E.</strong> Use AWS Elastic Beanstalk deployment caching feature</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon EC2 user data to customize the dynamic installation parts at boot time

B. Create a Golden Amazon Machine Image (AMI) with the static installation components already setup

</details>

---

## Câu 197

**Chủ đề:** Design High-Performing Architectures

A digital media platform is preparing to launch a new interactive content service that is expected to receive sudden spikes in user engagement, especially during live events and media releases. The backend uses an Amazon Aurora PostgreSQL Serverless v2 cluster to handle dynamic workloads. The architecture must be capable of scaling both compute and storage performance to maintain low latency and avoid bottlenecks under load. The engineering team is evaluating storage configuration options and wants a solution that will scale automatically with traffic, optimize I/O performance, and remain cost-effective without manual provisioning or tuning.

Which configuration will best meet these requirements?

**Lựa chọn:**

<label for="q197-a"><input type="radio" id="q197-a" name="q197" value="A"> <strong>A.</strong> Configure the Aurora cluster to use General Purpose SSD (gp2) storage. Increase performance by scaling database compute capacity to reduce IOPS bottlenecks</label><br>
<label for="q197-b"><input type="radio" id="q197-b" name="q197" value="B"> <strong>B.</strong> Configure the Aurora cluster to use Aurora I/O-Optimized storage. This configuration delivers high throughput and low-latency I/O performance with predictable pricing and no I/O-based charges</label><br>
<label for="q197-c"><input type="radio" id="q197-c" name="q197" value="C"> <strong>C.</strong> Select Provisioned IOPS (io1) as the storage type for the Aurora cluster. Manually adjust IOPS based on expected traffic during peak usage</label><br>
<label for="q197-d"><input type="radio" id="q197-d" name="q197" value="D"> <strong>D.</strong> Configure the cluster with Magnetic (Standard) storage to minimize baseline storage costs and rely on Aurora’s autoscaling to handle demand spikes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure the Aurora cluster to use Aurora I/O-Optimized storage. This configuration delivers high throughput and low-latency I/O performance with predictable pricing and no I/O-based charges

</details>

---

## Câu 198

**Chủ đề:** Design Resilient Architectures

A company has migrated its application from a monolith architecture to a microservices based architecture. The development team has updated the Amazon Route 53 simple record to point "myapp.mydomain.com" from the old Load Balancer to the new one.

The users are still not redirected to the new Load Balancer. What has gone wrong in the configuration?

**Lựa chọn:**

<label for="q198-a"><input type="radio" id="q198-a" name="q198" value="A"> <strong>A.</strong> The Time To Live (TTL) is still in effect</label><br>
<label for="q198-b"><input type="radio" id="q198-b" name="q198" value="B"> <strong>B.</strong> The health checks are failing</label><br>
<label for="q198-c"><input type="radio" id="q198-c" name="q198" value="C"> <strong>C.</strong> The Alias Record is misconfigured</label><br>
<label for="q198-d"><input type="radio" id="q198-d" name="q198" value="D"> <strong>D.</strong> The CNAME Record is misconfigured</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The Time To Live (TTL) is still in effect

</details>

---

## Câu 199

**Chủ đề:** Design Secure Architectures

A global insurance company is modernizing its infrastructure by migrating multiple line-of-business applications from its on-premises data centers to AWS. These applications will be deployed across several AWS accounts, all governed under a centralized AWS Organizations structure. The company manages all user identities, groups, and access policies within its on-premises Microsoft Active Directory and wants to continue doing so. The goal is to enable seamless single sign-in across all AWS accounts without duplicating user identity stores or manually provisioning accounts.

Which solution best meets these requirements in the most operationally efficient manner?

**Lựa chọn:**

<label for="q199-a"><input type="radio" id="q199-a" name="q199" value="A"> <strong>A.</strong> Deploy AWS IAM Identity Center and configure it to use AWS Directory Service for Microsoft Active Directory (Enterprise Edition). Establish a two-way trust relationship between the managed directory and the on-premises Active Directory to enable federated authentication across all AWS accounts</label><br>
<label for="q199-b"><input type="radio" id="q199-b" name="q199" value="B"> <strong>B.</strong> Enable AWS IAM Identity Center and manually create user accounts and groups within it. Assign these users permission sets in each AWS account. Manage synchronization with on-premises Active Directory using custom PowerShell scripts</label><br>
<label for="q199-c"><input type="radio" id="q199-c" name="q199" value="C"> <strong>C.</strong> Use Amazon Cognito as the primary identity store and create a custom OpenID Connect (OIDC) federation with the on-premises Active Directory. Assign IAM roles using Cognito identity pools and propagate access to multiple AWS accounts using resource policies</label><br>
<label for="q199-d"><input type="radio" id="q199-d" name="q199" value="D"> <strong>D.</strong> Deploy an OpenLDAP server on Amazon EC2, sync it with the on-premises Active Directory, and integrate it with each AWS account by creating IAM roles that trust the EC2-hosted LDAP server as a SAML provider</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy AWS IAM Identity Center and configure it to use AWS Directory Service for Microsoft Active Directory (Enterprise Edition). Establish a two-way trust relationship between the managed directory and the on-premises Active Directory to enable federated authentication across all AWS accounts

</details>

---

## Câu 200

**Chủ đề:** Design Resilient Architectures

The engineering team at a global e-commerce company is currently reviewing their disaster recovery strategy. The team has outlined that they need to be able to quickly recover their application stack with a Recovery Time Objective (RTO) of 5 minutes, in all of the AWS Regions that the application runs. The application stack currently takes over 45 minutes to install on a Linux system.

As a Solutions architect, which of the following options would you recommend as the disaster recovery strategy?

**Lựa chọn:**

<label for="q200-a"><input type="radio" id="q200-a" name="q200" value="A"> <strong>A.</strong> Store the installation files in Amazon S3 for quicker retrieval</label><br>
<label for="q200-b"><input type="radio" id="q200-b" name="q200" value="B"> <strong>B.</strong> Use Amazon EC2 user data to speed up the installation process</label><br>
<label for="q200-c"><input type="radio" id="q200-c" name="q200" value="C"> <strong>C.</strong> Create an Amazon Machine Image (AMI) after installing the software and use this AMI to run the recovery process in other Regions</label><br>
<label for="q200-d"><input type="radio" id="q200-d" name="q200" value="D"> <strong>D.</strong> Create an Amazon Machine Image (AMI) after installing the software and copy the AMI across all Regions. Use this Region-specific AMI to run the recovery process in the respective Regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Create an Amazon Machine Image (AMI) after installing the software and copy the AMI across all Regions. Use this Region-specific AMI to run the recovery process in the respective Regions

</details>

---

## Câu 201

**Chủ đề:** Design Cost-Optimized Architectures

An e-commerce analytics company is preparing to archive several years of transaction records and customer analytics reports in Amazon S3 for long-term storage. To meet compliance requirements, the archived data must be encrypted at rest. Additionally, the solution must be cost-effective and ensure that key rotation occurs automatically every 12 months to comply with the company’s internal data governance policy.

Which solution will meet these requirements with the least operational overhead?

**Lựa chọn:**

<label for="q201-a"><input type="radio" id="q201-a" name="q201" value="A"> <strong>A.</strong> Use Amazon S3 server-side encryption with S3-managed keys (SSE-S3). Upload data with default encryption enabled. Rely on the built-in key management and rotation behavior of SSE-S3</label><br>
<label for="q201-b"><input type="radio" id="q201-b" name="q201" value="B"> <strong>B.</strong> Encrypt the data locally using client-side encryption libraries and upload the encrypted files to S3. Create a KMS key with imported key material and configure key rotation settings</label><br>
<label for="q201-c"><input type="radio" id="q201-c" name="q201" value="C"> <strong>C.</strong> Use AWS CloudHSM to generate encryption keys. Configure S3 to use these custom encryption keys via client-side encryption and rotate the keys annually using an on-premises key management workflow</label><br>
<label for="q201-d"><input type="radio" id="q201-d" name="q201" value="D"> <strong>D.</strong> Use AWS Key Management Service (KMS) to create a customer managed key with automatic rotation enabled. Configure the S3 bucket’s default encryption to use the customer managed key. Migrate the data to the S3 bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Key Management Service (KMS) to create a customer managed key with automatic rotation enabled. Configure the S3 bucket’s default encryption to use the customer managed key. Migrate the data to the S3 bucket

</details>

---

## Câu 202

**Chủ đề:** Design Secure Architectures

A global pharmaceutical company operates a hybrid cloud network. Its primary AWS workloads run in the us-west-2 Region, connected to its on-premises data center via an AWS Direct Connect connection. After acquiring a biotech firm headquartered in Europe, the company must integrate the biotech’s workloads, which are hosted in several VPCs in the eu-central-1 Region and connected to the biotech's on-premises facility through a separate Direct Connect link. All CIDR blocks are non-overlapping, and the business requires full connectivity between both data centers and all VPCs across the two Regions. The company also wants a scalable solution that minimizes manual network configuration and long-term operational overhead.

Which solution will best meet these requirements?

**Lựa chọn:**

<label for="q202-a"><input type="radio" id="q202-a" name="q202" value="A"> <strong>A.</strong> Establish inter-Region VPC peering between each VPC in the us-west-2 and eu-central-1 Regions. Use static routing tables in each VPC to define peer relationships and enable cross-Region communication</label><br>
<label for="q202-b"><input type="radio" id="q202-b" name="q202" value="B"> <strong>B.</strong> Connect both Direct Connect links to a shared Direct Connect gateway. Attach each Region's virtual private gateway (VGW) to the Direct Connect gateway, enabling transitive routing between the VPCs and the on-premises networks across Regions</label><br>
<label for="q202-c"><input type="radio" id="q202-c" name="q202" value="C"> <strong>C.</strong> Deploy EC2-based VPN appliances in each VPC. Configure a full mesh VPN topology between all VPCs and data centers using CloudHub-style routing across Regions</label><br>
<label for="q202-d"><input type="radio" id="q202-d" name="q202" value="D"> <strong>D.</strong> Create private VIFs (virtual interfaces) in each Region and associate them directly with foreign-region VPCs using routing table entries and BGP. Use VPC endpoints in each account to forward cross-Region traffic</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Connect both Direct Connect links to a shared Direct Connect gateway. Attach each Region's virtual private gateway (VGW) to the Direct Connect gateway, enabling transitive routing between the VPCs and the on-premises networks across Regions

</details>

---

## Câu 203

**Chủ đề:** Design Secure Architectures

A junior developer has downloaded a sample Amazon S3 bucket policy to make changes to it based on new company-wide access policies. He has requested your help in understanding this bucket policy.

As a Solutions Architect, which of the following would you identify as the correct description for the given policy?

{
 "Version": "2012-10-17",
 "Id": "S3PolicyId1",
 "Statement": [
   {
     "Sid": "IPAllow",
     "Effect": "Allow",
     "Principal": "*",
     "Action": "s3:*",
     "Resource": "arn:aws:s3:::examplebucket/*",
     "Condition": {
        "IpAddress": {"aws:SourceIp": "54.240.143.0/24"},
        "NotIpAddress": {"aws:SourceIp": "54.240.143.188/32"}
     }
   }
 ]
}

**Lựa chọn:**

<label for="q203-a"><input type="radio" id="q203-a" name="q203" value="A"> <strong>A.</strong> It ensures the Amazon S3 bucket is exposing an external IP within the Classless Inter-Domain Routing (CIDR) range specified, except one IP</label><br>
<label for="q203-b"><input type="radio" id="q203-b" name="q203" value="B"> <strong>B.</strong> It authorizes an entire Classless Inter-Domain Routing (CIDR) except one IP address to access the Amazon S3 bucket</label><br>
<label for="q203-c"><input type="radio" id="q203-c" name="q203" value="C"> <strong>C.</strong> It ensures Amazon EC2 instances that have inherited a security group can access the bucket</label><br>
<label for="q203-d"><input type="radio" id="q203-d" name="q203" value="D"> <strong>D.</strong> It authorizes an IP address and a Classless Inter-Domain Routing (CIDR) to access the S3 bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. It authorizes an entire Classless Inter-Domain Routing (CIDR) except one IP address to access the Amazon S3 bucket

</details>

---

## Câu 204

**Chủ đề:** Design Resilient Architectures

You are working for a software as a service (SaaS) company as a solutions architect and help design solutions for the company's customers. One of the customers is a bank and has a requirement to whitelist a public IP when the bank is accessing external services across the internet.

Which architectural choice do you recommend to maintain high availability, support scaling-up to 10 instances and comply with the bank's requirements?

**Lựa chọn:**

<label for="q204-a"><input type="radio" id="q204-a" name="q204" value="A"> <strong>A.</strong> Use a Network Load Balancer with an Auto Scaling Group</label><br>
<label for="q204-b"><input type="radio" id="q204-b" name="q204" value="B"> <strong>B.</strong> Use a Classic Load Balancer with an Auto Scaling Group</label><br>
<label for="q204-c"><input type="radio" id="q204-c" name="q204" value="C"> <strong>C.</strong> Use an Application Load Balancer with an Auto Scaling Group</label><br>
<label for="q204-d"><input type="radio" id="q204-d" name="q204" value="D"> <strong>D.</strong> Use an Auto Scaling Group with Dynamic Elastic IPs attachment</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use a Network Load Balancer with an Auto Scaling Group

</details>

---

## Câu 205

**Chủ đề:** Design Resilient Architectures

A ride-sharing company wants to improve the ride-tracking system that stores GPS coordinates for all rides. The engineering team at the company is looking for a NoSQL database that has single-digit millisecond latency, can scale horizontally, and is serverless, so that they can perform high-frequency lookups reliably.

As a Solutions Architect, which database do you recommend for their requirements?

**Lựa chọn:**

<label for="q205-a"><input type="radio" id="q205-a" name="q205" value="A"> <strong>A.</strong> Amazon Neptune</label><br>
<label for="q205-b"><input type="radio" id="q205-b" name="q205" value="B"> <strong>B.</strong> Amazon Relational Database Service (Amazon RDS)</label><br>
<label for="q205-c"><input type="radio" id="q205-c" name="q205" value="C"> <strong>C.</strong> Amazon ElastiCache</label><br>
<label for="q205-d"><input type="radio" id="q205-d" name="q205" value="D"> <strong>D.</strong> Amazon DynamoDB</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Amazon DynamoDB

</details>

---

## Câu 206

**Chủ đề:** Design High-Performing Architectures

The development team at a social media company wants to handle some complicated queries such as "What are the number of likes on the videos that have been posted by friends of a user A?".

As a solutions architect, which of the following AWS database services would you suggest as the BEST fit to handle such use cases?

**Lựa chọn:**

<label for="q206-a"><input type="radio" id="q206-a" name="q206" value="A"> <strong>A.</strong> Amazon Neptune</label><br>
<label for="q206-b"><input type="radio" id="q206-b" name="q206" value="B"> <strong>B.</strong> Amazon Redshift</label><br>
<label for="q206-c"><input type="radio" id="q206-c" name="q206" value="C"> <strong>C.</strong> Amazon OpenSearch Service</label><br>
<label for="q206-d"><input type="radio" id="q206-d" name="q206" value="D"> <strong>D.</strong> Amazon Aurora</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon Neptune

</details>

---

## Câu 207

**Chủ đề:** Design Cost-Optimized Architectures

A transportation logistics company runs a shipment tracking application on Amazon EC2 instances with an Amazon Aurora MySQL database cluster. The application is experiencing rapid growth due to increased demand from mobile app users querying package delivery statuses. Although the compute layer (EC2) has remained stable, the Aurora DB cluster is under growing read pressure, especially from frequent repeated queries about package locations and delivery history. The company added an Aurora read replica, which temporarily alleviated the load, but read traffic continues to spike as user queries grow. The company wants to reduce the repeated reads pressure on the DB cluster.

Which solution will best meet these requirements in a cost-effective manner?

**Lựa chọn:**

<label for="q207-a"><input type="radio" id="q207-a" name="q207" value="A"> <strong>A.</strong> Integrate Amazon ElastiCache for Redis between the application and Aurora. Cache frequently accessed query results in Redis to reduce the number of identical read requests hitting the database</label><br>
<label for="q207-b"><input type="radio" id="q207-b" name="q207" value="B"> <strong>B.</strong> Enable Aurora Serverless v2 for the DB cluster to automatically scale read and write capacity in response to usage spikes. Route all traffic through the cluster endpoint</label><br>
<label for="q207-c"><input type="radio" id="q207-c" name="q207" value="C"> <strong>C.</strong> Add another Aurora read replica to distribute the increasing read load across more read nodes. Adjust the application to perform client-side load balancing across the read replicas</label><br>
<label for="q207-d"><input type="radio" id="q207-d" name="q207" value="D"> <strong>D.</strong> Convert the Aurora MySQL DB cluster into a multi-writer setup using Aurora global database. Allow concurrent writes from multiple application nodes across Regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Integrate Amazon ElastiCache for Redis between the application and Aurora. Cache frequently accessed query results in Redis to reduce the number of identical read requests hitting the database

</details>

---

## Câu 208

**Chủ đề:** Design Resilient Architectures

A company has developed a popular photo-sharing website using a serverless pattern on the AWS Cloud using Amazon API Gateway and AWS Lambda. The backend uses an Amazon RDS PostgreSQL database. The website is experiencing high read traffic and the AWS Lambda functions are putting an increased read load on the Amazon RDS database.

The architecture team is planning to increase the read throughput of the database, without changing the application's core logic. As a Solutions Architect, what do you recommend?

**Lựa chọn:**

<label for="q208-a"><input type="radio" id="q208-a" name="q208" value="A"> <strong>A.</strong> Use Amazon RDS Multi-AZ feature</label><br>
<label for="q208-b"><input type="radio" id="q208-b" name="q208" value="B"> <strong>B.</strong> Use Amazon RDS Read Replicas</label><br>
<label for="q208-c"><input type="radio" id="q208-c" name="q208" value="C"> <strong>C.</strong> Use Amazon ElastiCache</label><br>
<label for="q208-d"><input type="radio" id="q208-d" name="q208" value="D"> <strong>D.</strong> Use Amazon DynamoDB</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon RDS Read Replicas

</details>

---

## Câu 209

**Chủ đề:** Design Resilient Architectures

A digital media company needs to manage uploads of around 1 terabyte each from an application being used by a partner company.

As a Solutions Architect, how will you handle the upload of these files to Amazon S3?

**Lựa chọn:**

<label for="q209-a"><input type="radio" id="q209-a" name="q209" value="A"> <strong>A.</strong> Use multi-part upload feature of Amazon S3</label><br>
<label for="q209-b"><input type="radio" id="q209-b" name="q209" value="B"> <strong>B.</strong> Use Amazon S3 Versioning</label><br>
<label for="q209-c"><input type="radio" id="q209-c" name="q209" value="C"> <strong>C.</strong> Use AWS Snowball</label><br>
<label for="q209-d"><input type="radio" id="q209-d" name="q209" value="D"> <strong>D.</strong> Use AWS Direct Connect to provide extra bandwidth</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use multi-part upload feature of Amazon S3

</details>

---

## Câu 210

**Chủ đề:** Design Cost-Optimized Architectures

A company has noticed that its Amazon EBS Elastic Volume (io1) accounts for 90% of the cost and the remaining 10% cost can be attributed to the Amazon EC2 instance. The Amazon CloudWatch metrics report that both the Amazon EC2 instance and the Amazon EBS volume are under-utilized. The Amazon CloudWatch metrics also show that the Amazon EBS volume has occasional I/O bursts. The entire infrastructure is managed by AWS CloudFormation.

As a Solutions Architect, what do you propose to reduce the costs?

**Lựa chọn:**

<label for="q210-a"><input type="radio" id="q210-a" name="q210" value="A"> <strong>A.</strong> Don't use a AWS CloudFormation template to create the database as the AWS CloudFormation service incurs greater service charges</label><br>
<label for="q210-b"><input type="radio" id="q210-b" name="q210" value="B"> <strong>B.</strong> Keep the Amazon EBS volume to io1 and reduce the IOPS</label><br>
<label for="q210-c"><input type="radio" id="q210-c" name="q210" value="C"> <strong>C.</strong> Convert the Amazon EC2 instance EBS volume to gp2</label><br>
<label for="q210-d"><input type="radio" id="q210-d" name="q210" value="D"> <strong>D.</strong> Change the Amazon EC2 instance type to something much smaller</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Convert the Amazon EC2 instance EBS volume to gp2

</details>

---

## Câu 211

**Chủ đề:** Design Resilient Architectures

As a solutions architect, you have created a solution that utilizes an Application Load Balancer with stickiness and an Auto Scaling Group (ASG). The Auto Scaling Group spans across 2 Availability Zones (AZs). AZ-A has 3 Amazon EC2 instances and AZ-B has 4 Amazon EC2 instances. The Auto Scaling Group is about to go into a scale-in event due to the triggering of a Amazon CloudWatch alarm.

What will happen under the default Auto Scaling Group configuration?

**Lựa chọn:**

<label for="q211-a"><input type="radio" id="q211-a" name="q211" value="A"> <strong>A.</strong> The instance with the oldest launch template or launch configuration will be terminated in AZ-B</label><br>
<label for="q211-b"><input type="radio" id="q211-b" name="q211" value="B"> <strong>B.</strong> A random instance in the AZ-A will be terminated</label><br>
<label for="q211-c"><input type="radio" id="q211-c" name="q211" value="C"> <strong>C.</strong> An instance in the AZ-A will be created</label><br>
<label for="q211-d"><input type="radio" id="q211-d" name="q211" value="D"> <strong>D.</strong> A random instance will be terminated in AZ-B</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The instance with the oldest launch template or launch configuration will be terminated in AZ-B

</details>

---

## Câu 212

**Chủ đề:** Design Secure Architectures

What does this AWS CloudFormation snippet do? (Select three)

SecurityGroupIngress:
     - IpProtocol: tcp
       FromPort: 80
       ToPort: 80
       CidrIp: 0.0.0.0/0
     - IpProtocol: tcp
       FromPort: 22
       ToPort: 22
       CidrIp: 192.168.1.1/32

**Lựa chọn:**

<label for="q212-a"><input type="checkbox" id="q212-a" name="q212" value="A"> <strong>A.</strong> It configures the inbound rules of a network access control list (network ACL)</label><br>
<label for="q212-b"><input type="checkbox" id="q212-b" name="q212" value="B"> <strong>B.</strong> It allows any IP to pass through on the HTTP port</label><br>
<label for="q212-c"><input type="checkbox" id="q212-c" name="q212" value="C"> <strong>C.</strong> It only allows the IP 0.0.0.0 to reach HTTP</label><br>
<label for="q212-d"><input type="checkbox" id="q212-d" name="q212" value="D"> <strong>D.</strong> It prevents traffic from reaching on HTTP unless from the IP 192.168.1.1</label><br>
<label for="q212-e"><input type="checkbox" id="q212-e" name="q212" value="E"> <strong>E.</strong> It configures a security group's inbound rules</label><br>
<label for="q212-f"><input type="checkbox" id="q212-f" name="q212" value="F"> <strong>F.</strong> It lets traffic flow from one IP on port 22</label><br>
<label for="q212-g"><input type="checkbox" id="q212-g" name="q212" value="G"> <strong>G.</strong> It configures a security group's outbound rules</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. It allows any IP to pass through on the HTTP port

E. It configures a security group's inbound rules

F. It lets traffic flow from one IP on port 22

</details>

---

## Câu 213

**Chủ đề:** Design High-Performing Architectures

A retail company is using AWS Site-to-Site VPN connections for secure connectivity to its AWS cloud resources from its on-premises data center. Due to a surge in traffic across the VPN connections to the AWS cloud, users are experiencing slower VPN connectivity.

Which of the following options will maximize the VPN throughput?

**Lựa chọn:**

<label for="q213-a"><input type="radio" id="q213-a" name="q213" value="A"> <strong>A.</strong> Use Transfer Acceleration for the VPN connection to maximize the throughput</label><br>
<label for="q213-b"><input type="radio" id="q213-b" name="q213" value="B"> <strong>B.</strong> Use AWS Global Accelerator for the VPN connection to maximize the throughput</label><br>
<label for="q213-c"><input type="radio" id="q213-c" name="q213" value="C"> <strong>C.</strong> Create a virtual private gateway with equal cost multipath routing and multiple channels</label><br>
<label for="q213-d"><input type="radio" id="q213-d" name="q213" value="D"> <strong>D.</strong> Create an AWS Transit Gateway with equal cost multipath routing and add additional VPN tunnels</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Create an AWS Transit Gateway with equal cost multipath routing and add additional VPN tunnels

</details>

---

## Câu 214

**Chủ đề:** Design Resilient Architectures

An e-commerce company wants to migrate its on-premises application to AWS. The application consists of application servers and a Microsoft SQL Server database. The solution should result in the maximum possible availability for the database layer while minimizing operational and management overhead.

As a solutions architect, which of the following would you recommend to meet the given requirements?

**Lựa chọn:**

<label for="q214-a"><input type="radio" id="q214-a" name="q214" value="A"> <strong>A.</strong> Migrate the data to Amazon EC2 instance hosted SQL Server database. Deploy the Amazon EC2 instances in a Multi-AZ configuration</label><br>
<label for="q214-b"><input type="radio" id="q214-b" name="q214" value="B"> <strong>B.</strong> Migrate the data to Amazon RDS for SQL Server database in a cross-region read-replica configuration</label><br>
<label for="q214-c"><input type="radio" id="q214-c" name="q214" value="C"> <strong>C.</strong> Migrate the data to Amazon RDS for SQL Server database in a cross-region Multi-AZ deployment</label><br>
<label for="q214-d"><input type="radio" id="q214-d" name="q214" value="D"> <strong>D.</strong> Migrate the data to Amazon RDS for SQL Server database in a Multi-AZ deployment</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Migrate the data to Amazon RDS for SQL Server database in a Multi-AZ deployment

</details>

---

## Câu 215

**Chủ đề:** Design High-Performing Architectures

A Big Data processing company has created a distributed data processing framework that performs best if the network performance between the processing machines is high. The application has to be deployed on AWS, and the company is only looking at performance as the key measure.

As a Solutions Architect, which deployment do you recommend?

**Lựa chọn:**

<label for="q215-a"><input type="radio" id="q215-a" name="q215" value="A"> <strong>A.</strong> Use Spot Instances</label><br>
<label for="q215-b"><input type="radio" id="q215-b" name="q215" value="B"> <strong>B.</strong> Use a Spread placement group</label><br>
<label for="q215-c"><input type="radio" id="q215-c" name="q215" value="C"> <strong>C.</strong> Optimize the Amazon EC2 kernel using EC2 User Data</label><br>
<label for="q215-d"><input type="radio" id="q215-d" name="q215" value="D"> <strong>D.</strong> Use a Cluster placement group</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use a Cluster placement group

</details>

---

## Câu 216

**Chủ đề:** Design Cost-Optimized Architectures

A streaming media company operates a high-traffic content delivery platform on AWS. The application backend is deployed on Amazon EC2 instances within an Auto Scaling group across multiple Availability Zones in a VPC. The team has observed that workloads follow predictable usage patterns, such as higher viewership on weekends and in the evenings, along with occasional real-time spikes due to viral content. To reduce cost and improve responsiveness, the team wants an automated scaling approach that can forecast future demand using historical usage patterns, scale in advance based on those predictions, and react quickly to unplanned usage surges in real time.

Which scaling strategy should a solutions architect recommend to meet these requirements?

**Lựa chọn:**

<label for="q216-a"><input type="radio" id="q216-a" name="q216" value="A"> <strong>A.</strong> Configure step scaling policies based on EC2 CPU utilization. Use CloudWatch alarms to trigger scaling actions when utilization crosses defined thresholds with incremental adjustments</label><br>
<label for="q216-b"><input type="radio" id="q216-b" name="q216" value="B"> <strong>B.</strong> Use predictive scaling for the Auto Scaling group to analyze daily and weekly patterns, and configure dynamic scaling with target tracking policies to respond to real-time traffic changes</label><br>
<label for="q216-c"><input type="radio" id="q216-c" name="q216" value="C"> <strong>C.</strong> Implement scheduled scaling actions based on pre-defined time windows from historical traffic data. Adjust instance count manually for known high-traffic hours</label><br>
<label for="q216-d"><input type="radio" id="q216-d" name="q216" value="D"> <strong>D.</strong> Set up simple scaling policies with longer cooldown periods to avoid rapid scaling. Trigger scale-out events based on average network throughput</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use predictive scaling for the Auto Scaling group to analyze daily and weekly patterns, and configure dynamic scaling with target tracking policies to respond to real-time traffic changes

</details>

---

## Câu 217

**Chủ đề:** Design High-Performing Architectures

An e-commerce company tracks user clicks on its flagship website and performs analytics to provide near-real-time product recommendations. An Amazon EC2 instance receives data from the website and sends the data to an Amazon Aurora Database instance. Another Amazon EC2 instance continuously checks the changes in the database and executes SQL queries to provide recommendations. Now, the company wants a redesign to decouple and scale the infrastructure. The solution must ensure that data can be analyzed in real-time without any data loss even when the company sees huge traffic spikes.

What would you recommend as an AWS Certified Solutions Architect - Associate?

**Lựa chọn:**

<label for="q217-a"><input type="radio" id="q217-a" name="q217" value="A"> <strong>A.</strong> Leverage Amazon Kinesis Data Streams to capture the data from the website and feed it into Amazon QuickSight which can query the data in real time. Lastly, the analyzed feed is output into Kinesis Data Firehose to persist the data on Amazon S3</label><br>
<label for="q217-b"><input type="radio" id="q217-b" name="q217" value="B"> <strong>B.</strong> Leverage Amazon Kinesis Data Streams to capture the data from the website and feed it into Amazon Kinesis Data Analytics which can query the data in real time. Lastly, the analyzed feed is output into Amazon Kinesis Data Firehose to persist the data on Amazon S3</label><br>
<label for="q217-c"><input type="radio" id="q217-c" name="q217" value="C"> <strong>C.</strong> Leverage Amazon Kinesis Data Streams to capture the data from the website and feed it into Amazon Kinesis Data Firehose to persist the data on Amazon S3. Lastly, use Amazon Athena to analyze the data in real time</label><br>
<label for="q217-d"><input type="radio" id="q217-d" name="q217" value="D"> <strong>D.</strong> Leverage Amazon SQS to capture the data from the website. Configure a fleet of Amazon EC2 instances under an Auto scaling group to process messages from the Amazon SQS queue and trigger the scaling policy based on the number of pending messages in the queue. Perform real-time analytics using a third-party library on the Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Leverage Amazon Kinesis Data Streams to capture the data from the website and feed it into Amazon Kinesis Data Analytics which can query the data in real time. Lastly, the analyzed feed is output into Amazon Kinesis Data Firehose to persist the data on Amazon S3

</details>

---

## Câu 218

**Chủ đề:** Design Secure Architectures

For security purposes, a development team has decided to deploy the Amazon EC2 instances in a private subnet. The team plans to use VPC endpoints so that the instances can access some AWS services securely. The members of the team would like to know about the two AWS services that support Gateway Endpoints.

As a solutions architect, which of the following services would you suggest for this requirement? (Select two)

**Lựa chọn:**

<label for="q218-a"><input type="checkbox" id="q218-a" name="q218" value="A"> <strong>A.</strong> Amazon Simple Queue Service (Amazon SQS)</label><br>
<label for="q218-b"><input type="checkbox" id="q218-b" name="q218" value="B"> <strong>B.</strong> Amazon Simple Notification Service (Amazon SNS)</label><br>
<label for="q218-c"><input type="checkbox" id="q218-c" name="q218" value="C"> <strong>C.</strong> Amazon DynamoDB</label><br>
<label for="q218-d"><input type="checkbox" id="q218-d" name="q218" value="D"> <strong>D.</strong> Amazon S3</label><br>
<label for="q218-e"><input type="checkbox" id="q218-e" name="q218" value="E"> <strong>E.</strong> Amazon Kinesis</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Amazon DynamoDB

D. Amazon S3

</details>

---

## Câu 219

**Chủ đề:** Design High-Performing Architectures

A research organization is running a high-performance computing (HPC) workload using Amazon EC2 instances that are distributed across multiple Availability Zones (AZs) within a single AWS Region. The workload requires access to a shared file system with the lowest possible latency for frequent reads and writes.The team decides to use Amazon Elastic File System (Amazon EFS) for its scalability and simplicity. To ensure optimal performance and reduce network latency, the solution architect must design the architecture so that each EC2 instance can access the file system with the least possible delay.

Which of the following is the most appropriate solution to meet these requirements?

**Lựa chọn:**

<label for="q219-a"><input type="radio" id="q219-a" name="q219" value="A"> <strong>A.</strong> Create EFS mount targets in each AZ and mount the EFS file system to EC2 instances in the same AZ as the mount target</label><br>
<label for="q219-b"><input type="radio" id="q219-b" name="q219" value="B"> <strong>B.</strong> Create mount targets for Amazon EFS on an EC2 instance in each AZ and use them to serve as access points for other instances</label><br>
<label for="q219-c"><input type="radio" id="q219-c" name="q219" value="C"> <strong>C.</strong> Create a single EFS mount target in one AZ and allow all EC2 instances in other AZs to access it using the default mount target</label><br>
<label for="q219-d"><input type="radio" id="q219-d" name="q219" value="D"> <strong>D.</strong> Use Mountpoint for Amazon S3 to mount an S3 bucket on each EC2 instance and use it as a shared storage layer across Availability Zones</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create EFS mount targets in each AZ and mount the EFS file system to EC2 instances in the same AZ as the mount target

</details>

---

## Câu 220

**Chủ đề:** Design High-Performing Architectures

The engineering team at an e-commerce company has been tasked with migrating to a serverless architecture. The team wants to focus on the key points of consideration when using AWS Lambda as a backbone for this architecture.

As a Solutions Architect, which of the following options would you identify as correct for the given requirement? (Select three)

**Lựa chọn:**

<label for="q220-a"><input type="checkbox" id="q220-a" name="q220" value="A"> <strong>A.</strong> By default, AWS Lambda functions always operate from an AWS-owned VPC and hence have access to any public internet address or public AWS APIs. Once an AWS Lambda function is VPC-enabled, it will need a route through a Network Address Translation gateway (NAT gateway) in a public subnet to access public resources</label><br>
<label for="q220-b"><input type="checkbox" id="q220-b" name="q220" value="B"> <strong>B.</strong> AWS Lambda allocates compute power in proportion to the memory you allocate to your function. AWS, thus recommends to over provision your function time out settings for the proper performance of AWS Lambda functions</label><br>
<label for="q220-c"><input type="checkbox" id="q220-c" name="q220" value="C"> <strong>C.</strong> The bigger your deployment package, the slower your AWS Lambda function will cold-start. Hence, AWS suggests packaging dependencies as a separate package from the actual AWS Lambda package</label><br>
<label for="q220-d"><input type="checkbox" id="q220-d" name="q220" value="D"> <strong>D.</strong> Since AWS Lambda functions can scale extremely quickly, it's a good idea to deploy a Amazon CloudWatch Alarm that notifies your team when function metrics such as ConcurrentExecutions or Invocations exceeds the expected threshold</label><br>
<label for="q220-e"><input type="checkbox" id="q220-e" name="q220" value="E"> <strong>E.</strong> If you intend to reuse code in more than one AWS Lambda function, you should consider creating an AWS Lambda Layer for the reusable code</label><br>
<label for="q220-f"><input type="checkbox" id="q220-f" name="q220" value="F"> <strong>F.</strong> Serverless architecture and containers complement each other but you cannot package and deploy AWS Lambda functions as container images</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. By default, AWS Lambda functions always operate from an AWS-owned VPC and hence have access to any public internet address or public AWS APIs. Once an AWS Lambda function is VPC-enabled, it will need a route through a Network Address Translation gateway (NAT gateway) in a public subnet to access public resources

D. Since AWS Lambda functions can scale extremely quickly, it's a good idea to deploy a Amazon CloudWatch Alarm that notifies your team when function metrics such as ConcurrentExecutions or Invocations exceeds the expected threshold

E. If you intend to reuse code in more than one AWS Lambda function, you should consider creating an AWS Lambda Layer for the reusable code

</details>

---

## Câu 221

**Chủ đề:** Design Secure Architectures

An Elastic Load Balancer has marked all the Amazon EC2 instances in the target group as unhealthy. Surprisingly, when a developer enters the IP address of the Amazon EC2 instances in the web browser, he can access the website.

What could be the reason the instances are being marked as unhealthy? (Select two)

**Lựa chọn:**

<label for="q221-a"><input type="checkbox" id="q221-a" name="q221" value="A"> <strong>A.</strong> The security group of the Amazon EC2 instance does not allow for traffic from the security group of the Application Load Balancer</label><br>
<label for="q221-b"><input type="checkbox" id="q221-b" name="q221" value="B"> <strong>B.</strong> The route for the health check is misconfigured</label><br>
<label for="q221-c"><input type="checkbox" id="q221-c" name="q221" value="C"> <strong>C.</strong> The Amazon Elastic Block Store (Amazon EBS) volumes have been improperly mounted</label><br>
<label for="q221-d"><input type="checkbox" id="q221-d" name="q221" value="D"> <strong>D.</strong> Your web-app has a runtime that is not supported by the Application Load Balancer</label><br>
<label for="q221-e"><input type="checkbox" id="q221-e" name="q221" value="E"> <strong>E.</strong> You need to attach elastic IP address (EIP) to the Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The security group of the Amazon EC2 instance does not allow for traffic from the security group of the Application Load Balancer

B. The route for the health check is misconfigured

</details>

---

## Câu 222

**Chủ đề:** Design High-Performing Architectures

A Big Data analytics company writes data and log files in Amazon S3 buckets. The company now wants to stream the existing data files as well as any ongoing file updates from Amazon S3 to Amazon Kinesis Data Streams.

As a Solutions Architect, which of the following would you suggest as the fastest possible way of building a solution for this requirement?

**Lựa chọn:**

<label for="q222-a"><input type="radio" id="q222-a" name="q222" value="A"> <strong>A.</strong> Configure Amazon EventBridge events for the bucket actions on Amazon S3. An AWS Lambda function can then be triggered from the Amazon EventBridge event that will send the necessary data to Amazon Kinesis Data Streams</label><br>
<label for="q222-b"><input type="radio" id="q222-b" name="q222" value="B"> <strong>B.</strong> Leverage Amazon S3 event notification to trigger an AWS Lambda function for the file create event. The AWS Lambda function will then send the necessary data to Amazon Kinesis Data Streams</label><br>
<label for="q222-c"><input type="radio" id="q222-c" name="q222" value="C"> <strong>C.</strong> Amazon S3 bucket actions can be directly configured to write data into Amazon Simple Notification Service (Amazon SNS). Amazon SNS can then be used to send the updates to Amazon Kinesis Data Streams</label><br>
<label for="q222-d"><input type="radio" id="q222-d" name="q222" value="D"> <strong>D.</strong> Leverage AWS Database Migration Service (AWS DMS) as a bridge between Amazon S3 and Amazon Kinesis Data Streams</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Leverage AWS Database Migration Service (AWS DMS) as a bridge between Amazon S3 and Amazon Kinesis Data Streams

</details>

---

## Câu 223

**Chủ đề:** Design High-Performing Architectures

A Pharmaceuticals company is looking for a simple solution to connect its VPCs and on-premises networks through a central hub.

As a Solutions Architect, which of the following would you suggest as the solution that requires the LEAST operational overhead?

**Lựa chọn:**

<label for="q223-a"><input type="radio" id="q223-a" name="q223" value="A"> <strong>A.</strong> Use AWS Transit Gateway to connect the Amazon VPCs to the on-premises networks</label><br>
<label for="q223-b"><input type="radio" id="q223-b" name="q223" value="B"> <strong>B.</strong> Use Transit VPC Solution to connect the Amazon VPCs to the on-premises networks</label><br>
<label for="q223-c"><input type="radio" id="q223-c" name="q223" value="C"> <strong>C.</strong> Partially meshed VPC peering can be used to connect the Amazon VPCs to the on-premises networks</label><br>
<label for="q223-d"><input type="radio" id="q223-d" name="q223" value="D"> <strong>D.</strong> Fully meshed VPC peering can be used to connect the Amazon VPCs to the on-premises networks</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS Transit Gateway to connect the Amazon VPCs to the on-premises networks

</details>

---

## Câu 224

**Chủ đề:** Design Resilient Architectures

An e-commerce company has copied 1 petabyte of data from its on-premises data center to an Amazon S3 bucket in the us-west-1 Region using an AWS Direct Connect link. The company now wants to set up a one-time copy of the data to another Amazon S3 bucket in the us-east-1 Region. The on-premises data center does not allow the use of AWS Snowball.

As a Solutions Architect, which of the following options can be used to accomplish this goal? (Select two)

**Lựa chọn:**

<label for="q224-a"><input type="checkbox" id="q224-a" name="q224" value="A"> <strong>A.</strong> Copy data from the source bucket to the destination bucket using the aws S3 sync command</label><br>
<label for="q224-b"><input type="checkbox" id="q224-b" name="q224" value="B"> <strong>B.</strong> Use AWS Snowball Edge device to copy the data from one Region to another Region</label><br>
<label for="q224-c"><input type="checkbox" id="q224-c" name="q224" value="C"> <strong>C.</strong> Copy data from the source Amazon S3 bucket to a target Amazon S3 bucket using the S3 console</label><br>
<label for="q224-d"><input type="checkbox" id="q224-d" name="q224" value="D"> <strong>D.</strong> Set up Amazon S3 batch replication to copy objects across Amazon S3 buckets in another Region using S3 console and then delete the replication configuration</label><br>
<label for="q224-e"><input type="checkbox" id="q224-e" name="q224" value="E"> <strong>E.</strong> Set up Amazon S3 Transfer Acceleration (Amazon S3TA) to copy objects across Amazon S3 buckets in different Regions using S3 console</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Copy data from the source bucket to the destination bucket using the aws S3 sync command

D. Set up Amazon S3 batch replication to copy objects across Amazon S3 buckets in another Region using S3 console and then delete the replication configuration

</details>

---

## Câu 225

**Chủ đề:** Design Cost-Optimized Architectures

A startup's cloud infrastructure consists of a few Amazon EC2 instances, Amazon RDS instances and Amazon S3 storage. A year into their business operations, the startup is incurring costs that seem too high for their business requirements.

Which of the following options represents a valid cost-optimization solution?

**Lựa chọn:**

<label for="q225-a"><input type="radio" id="q225-a" name="q225" value="A"> <strong>A.</strong> Use Amazon S3 Storage class analysis to get recommendations for transitions of objects to Amazon S3 Glacier storage classes to reduce storage costs. You can also automate moving these objects into lower-cost storage tier using Lifecycle Policies</label><br>
<label for="q225-b"><input type="radio" id="q225-b" name="q225" value="B"> <strong>B.</strong> Use AWS Cost Optimization Hub to get a report of Amazon EC2 instances that are either idle or have low utilization and use AWS Compute Optimizer to look at instance type recommendations</label><br>
<label for="q225-c"><input type="radio" id="q225-c" name="q225" value="C"> <strong>C.</strong> Use AWS Trusted Advisor checks on Amazon EC2 Reserved Instances to automatically renew reserved instances (RI). AWS Trusted advisor also suggests Amazon RDS idle database instances</label><br>
<label for="q225-d"><input type="radio" id="q225-d" name="q225" value="D"> <strong>D.</strong> Use AWS Compute Optimizer recommendations to help you choose the optimal Amazon EC2 purchasing options and help reserve your instance capacities at reduced costs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS Cost Optimization Hub to get a report of Amazon EC2 instances that are either idle or have low utilization and use AWS Compute Optimizer to look at instance type recommendations

</details>

---

## Câu 226

**Chủ đề:** Design Secure Architectures

A retail company uses AWS Cloud to manage its technology infrastructure. The company has deployed its consumer-focused web application on Amazon EC2-based web servers and uses Amazon RDS PostgreSQL database as the data store. The PostgreSQL database is set up in a private subnet that allows inbound traffic from selected Amazon EC2 instances. The database also uses AWS Key Management Service (AWS KMS) for encrypting data at rest.

Which of the following steps would you recommend to facilitate end-to-end security for the data-in-transit while accessing the database?

**Lựa chọn:**

<label for="q226-a"><input type="radio" id="q226-a" name="q226" value="A"> <strong>A.</strong> Use IAM authentication to access the database instead of the database user's access credentials</label><br>
<label for="q226-b"><input type="radio" id="q226-b" name="q226" value="B"> <strong>B.</strong> Configure Amazon RDS to use SSL for data in transit</label><br>
<label for="q226-c"><input type="radio" id="q226-c" name="q226" value="C"> <strong>C.</strong> Create a new security group that blocks SSH from the selected Amazon EC2 instances into the database</label><br>
<label for="q226-d"><input type="radio" id="q226-d" name="q226" value="D"> <strong>D.</strong> Create a new network access control list (network ACL) that blocks SSH from the entire Amazon EC2 subnet into the database</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure Amazon RDS to use SSL for data in transit

</details>

---

## Câu 227

**Chủ đề:** Design Resilient Architectures

A media company uses Amazon ElastiCache Redis to enhance the performance of its Amazon RDS database layer. The company wants a robust disaster recovery strategy for its caching layer that guarantees minimal downtime as well as minimal data loss while ensuring good application performance.

Which of the following solutions will you recommend to address the given use-case?

**Lựa chọn:**

<label for="q227-a"><input type="radio" id="q227-a" name="q227" value="A"> <strong>A.</strong> Opt for Multi-AZ configuration with automatic failover functionality to help mitigate failure</label><br>
<label for="q227-b"><input type="radio" id="q227-b" name="q227" value="B"> <strong>B.</strong> Schedule daily automatic backups at a time when you expect low resource utilization for your cluster</label><br>
<label for="q227-c"><input type="radio" id="q227-c" name="q227" value="C"> <strong>C.</strong> Schedule manual backups using Redis append-only file (AOF)</label><br>
<label for="q227-d"><input type="radio" id="q227-d" name="q227" value="D"> <strong>D.</strong> Add read-replicas across multiple availability zones (AZs) to reduce the risk of potential data loss because of failure</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Opt for Multi-AZ configuration with automatic failover functionality to help mitigate failure

</details>

---

## Câu 228

**Chủ đề:** Design Resilient Architectures

An IT company has a large number of clients opting to build their application programming interface (API) using Docker containers. To facilitate the hosting of these containers, the company is looking at various orchestration services available with AWS.

As a Solutions Architect, which of the following solutions will you suggest? (Select two)

**Lựa chọn:**

<label for="q228-a"><input type="checkbox" id="q228-a" name="q228" value="A"> <strong>A.</strong> Use Amazon Elastic Kubernetes Service (Amazon EKS) with AWS Fargate for serverless orchestration of the containerized services</label><br>
<label for="q228-b"><input type="checkbox" id="q228-b" name="q228" value="B"> <strong>B.</strong> Use Amazon Elastic Container Service (Amazon ECS) with Amazon EC2 for serverless orchestration of the containerized services</label><br>
<label for="q228-c"><input type="checkbox" id="q228-c" name="q228" value="C"> <strong>C.</strong> Use Amazon Elastic Container Service (Amazon ECS) with AWS Fargate for serverless orchestration of the containerized services</label><br>
<label for="q228-d"><input type="checkbox" id="q228-d" name="q228" value="D"> <strong>D.</strong> Use Amazon EMR for serverless orchestration of the containerized services</label><br>
<label for="q228-e"><input type="checkbox" id="q228-e" name="q228" value="E"> <strong>E.</strong> Use Amazon SageMaker for serverless orchestration of the containerized services</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon Elastic Kubernetes Service (Amazon EKS) with AWS Fargate for serverless orchestration of the containerized services

C. Use Amazon Elastic Container Service (Amazon ECS) with AWS Fargate for serverless orchestration of the containerized services

</details>

---

## Câu 229

**Chủ đề:** Design Secure Architectures

A systems administrator is creating IAM policies and attaching them to IAM identities. After creating the necessary identity-based policies, the administrator is now creating resource-based policies.

Which is the only resource-based policy that the IAM service supports?

**Lựa chọn:**

<label for="q229-a"><input type="radio" id="q229-a" name="q229" value="A"> <strong>A.</strong> AWS Organizations Service Control Policies (SCP)</label><br>
<label for="q229-b"><input type="radio" id="q229-b" name="q229" value="B"> <strong>B.</strong> Trust policy</label><br>
<label for="q229-c"><input type="radio" id="q229-c" name="q229" value="C"> <strong>C.</strong> Access control list (ACL)</label><br>
<label for="q229-d"><input type="radio" id="q229-d" name="q229" value="D"> <strong>D.</strong> Permissions boundary</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Trust policy

</details>

---

## Câu 230

**Chủ đề:** Design Resilient Architectures

A CRM company has a software as a service (SaaS) application that feeds updates to other in-house and third-party applications. The SaaS application and the in-house applications are being migrated to use AWS services for this inter-application communication.

As a Solutions Architect, which of the following would you suggest to asynchronously decouple the architecture?

**Lựa chọn:**

<label for="q230-a"><input type="radio" id="q230-a" name="q230" value="A"> <strong>A.</strong> Use Amazon Simple Queue Service (Amazon SQS) to decouple the architecture</label><br>
<label for="q230-b"><input type="radio" id="q230-b" name="q230" value="B"> <strong>B.</strong> Use Amazon EventBridge to decouple the system architecture</label><br>
<label for="q230-c"><input type="radio" id="q230-c" name="q230" value="C"> <strong>C.</strong> Use Amazon Simple Notification Service (Amazon SNS) to communicate between systems and decouple the architecture</label><br>
<label for="q230-d"><input type="radio" id="q230-d" name="q230" value="D"> <strong>D.</strong> Use Elastic Load Balancing (ELB) for effective decoupling of system architecture</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon EventBridge to decouple the system architecture

</details>

---

## Câu 231

**Chủ đề:** Design High-Performing Architectures

An enterprise has decided to move its secondary workloads such as backups and archives to AWS cloud. The CTO wishes to move the data stored on physical tapes to Cloud, without changing their current tape backup workflows. The company holds petabytes of data on tapes and needs a cost-optimized solution to move this data to cloud.

What is an optimal solution that meets these requirements while keeping the costs to a minimum?

**Lựa chọn:**

<label for="q231-a"><input type="radio" id="q231-a" name="q231" value="A"> <strong>A.</strong> Use Tape Gateway, which can be used to move on-premises tape data onto AWS Cloud. Then, Amazon S3 archiving storage classes can be used to store data cost-effectively for years</label><br>
<label for="q231-b"><input type="radio" id="q231-b" name="q231" value="B"> <strong>B.</strong> Use AWS DataSync, which makes it simple and fast to move large amounts of data online between on-premises storage and AWS Cloud. Data moved to Cloud can then be stored cost-effectively in Amazon S3 archiving storage classes</label><br>
<label for="q231-c"><input type="radio" id="q231-c" name="q231" value="C"> <strong>C.</strong> Use AWS Direct Connect, a cloud service solution that makes it easy to establish a dedicated network connection from on-premises to AWS to transfer data. Once this is done, Amazon S3 can be used to store data at lesser costs</label><br>
<label for="q231-d"><input type="radio" id="q231-d" name="q231" value="D"> <strong>D.</strong> Use AWS VPN connection between the on-premises datacenter and your Amazon VPC. Once this is established, you can use Amazon Elastic File System (Amazon EFS) to get a scalable, fully managed elastic NFS file system for use with AWS Cloud services and on-premises resources</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Tape Gateway, which can be used to move on-premises tape data onto AWS Cloud. Then, Amazon S3 archiving storage classes can be used to store data cost-effectively for years

</details>

---

## Câu 232

**Chủ đề:** Design Cost-Optimized Architectures

A healthcare provider is experiencing rapid data growth in its on-premises servers due to increased patient imaging and record retention requirements. The organization wants to extend its storage capacity to AWS in a way that preserves quick access to critical records, including from its local file systems. The company must optimize bandwidth usage during migration and avoid any retrieval fees or delays when accessing the data in the cloud. The provider wants a hybrid cloud solution that requires minimal application reconfiguration, allows frequent local access to key datasets, and ensures that cloud storage costs remain predictable without paying extra for data retrieval.

Which AWS solution best meets these requirements?

**Lựa chọn:**

<label for="q232-a"><input type="radio" id="q232-a" name="q232" value="A"> <strong>A.</strong> Implement Amazon FSx for Windows File Server and configure on-premises servers to mount the file system using a VPN connection. Store all primary data in FSx and use it as the central NAS replacement</label><br>
<label for="q232-b"><input type="radio" id="q232-b" name="q232" value="B"> <strong>B.</strong> Set up Amazon S3 Standard-Infrequent Access (S3 Standard-IA) as the primary storage tier. Configure the on-premises file server to replicate changes to the S3 bucket using AWS DataSync for asynchronous updates</label><br>
<label for="q232-c"><input type="radio" id="q232-c" name="q232" value="C"> <strong>C.</strong> Deploy AWS Storage Gateway using cached volumes. Store frequently accessed data locally, while writing all primary data asynchronously to Amazon S3</label><br>
<label for="q232-d"><input type="radio" id="q232-d" name="q232" value="D"> <strong>D.</strong> Deploy AWS Storage Gateway using stored volumes. Retain the full dataset on-premises and asynchronously back up point-in-time snapshots to Amazon S3. Configure applications to read from the local volume and recover data from the cloud if needed</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Deploy AWS Storage Gateway using cached volumes. Store frequently accessed data locally, while writing all primary data asynchronously to Amazon S3

</details>

---

## Câu 233

**Chủ đề:** Design Secure Architectures

A company has recently created a new department to handle their services workload. An IT team has been asked to create a custom VPC to isolate the resources created in this new department. They have set up the public subnet and internet gateway (IGW). However, they are not able to ping the Amazon EC2 instances with elastic IP address (EIP) launched in the newly created VPC.

As a Solutions Architect, the team has requested your help. How will you troubleshoot this scenario? (Select two)

**Lựa chọn:**

<label for="q233-a"><input type="checkbox" id="q233-a" name="q233" value="A"> <strong>A.</strong> Disable Source / Destination check on the Amazon EC2 instance</label><br>
<label for="q233-b"><input type="checkbox" id="q233-b" name="q233" value="B"> <strong>B.</strong> Check if the security groups allow ping from the source</label><br>
<label for="q233-c"><input type="checkbox" id="q233-c" name="q233" value="C"> <strong>C.</strong> Contact AWS support to map your VPC with subnet</label><br>
<label for="q233-d"><input type="checkbox" id="q233-d" name="q233" value="D"> <strong>D.</strong> Create a secondary internet gateway to attach with public subnet and move the current internet gateway to private and write route tables</label><br>
<label for="q233-e"><input type="checkbox" id="q233-e" name="q233" value="E"> <strong>E.</strong> Check if the route table is configured with internet gateway</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Check if the security groups allow ping from the source

E. Check if the route table is configured with internet gateway

</details>

---

## Câu 234

**Chủ đề:** Design Secure Architectures

A company runs a popular dating website on the AWS Cloud. As a Solutions Architect, you've designed the architecture of the website to follow a serverless pattern on the AWS Cloud using Amazon API Gateway and AWS Lambda. The backend uses an Amazon RDS PostgreSQL database. Currently, the application uses a username and password combination to connect the AWS Lambda function to the Amazon RDS database.

You would like to improve the security at the authentication level by leveraging short-lived credentials. What will you choose? (Select two)

**Lựa chọn:**

<label for="q234-a"><input type="checkbox" id="q234-a" name="q234" value="A"> <strong>A.</strong> Embed a credential rotation logic in the AWS Lambda, retrieving them from SSM</label><br>
<label for="q234-b"><input type="checkbox" id="q234-b" name="q234" value="B"> <strong>B.</strong> Use IAM authentication from AWS Lambda to Amazon RDS PostgreSQL</label><br>
<label for="q234-c"><input type="checkbox" id="q234-c" name="q234" value="C"> <strong>C.</strong> Restrict the Amazon RDS database security group to the AWS Lambda's security group</label><br>
<label for="q234-d"><input type="checkbox" id="q234-d" name="q234" value="D"> <strong>D.</strong> Deploy AWS Lambda in a VPC</label><br>
<label for="q234-e"><input type="checkbox" id="q234-e" name="q234" value="E"> <strong>E.</strong> Attach an AWS Identity and Access Management (IAM) role to AWS Lambda</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use IAM authentication from AWS Lambda to Amazon RDS PostgreSQL

E. Attach an AWS Identity and Access Management (IAM) role to AWS Lambda

</details>

---

## Câu 235

**Chủ đề:** Design Secure Architectures

A CRM web application was written as a monolith in PHP and is facing scaling issues because of performance bottlenecks. The CTO wants to re-engineer towards microservices architecture and expose their application from the same load balancer, linked to different target groups with different URLs: checkout.mycorp.com, www.mycorp.com, yourcorp.com/profile and yourcorp.com/search. The CTO would like to expose all these URLs as HTTPS endpoints for security purposes.

As a solutions architect, which of the following would you recommend as a solution that requires MINIMAL configuration effort?

**Lựa chọn:**

<label for="q235-a"><input type="radio" id="q235-a" name="q235" value="A"> <strong>A.</strong> Use Secure Sockets Layer certificate (SSL certificate) with SNI</label><br>
<label for="q235-b"><input type="radio" id="q235-b" name="q235" value="B"> <strong>B.</strong> Use a wildcard Secure Sockets Layer certificate (SSL certificate)</label><br>
<label for="q235-c"><input type="radio" id="q235-c" name="q235" value="C"> <strong>C.</strong> Use an HTTP to HTTPS redirect</label><br>
<label for="q235-d"><input type="radio" id="q235-d" name="q235" value="D"> <strong>D.</strong> Change the Elastic Load Balancing (ELB) SSL Security Policy</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Secure Sockets Layer certificate (SSL certificate) with SNI

</details>

---

## Câu 236

**Chủ đề:** Design Resilient Architectures

A financial services firm has traditionally operated with an on-premise data center and would like to create a disaster recovery strategy leveraging the AWS Cloud.

As a Solutions Architect, you would like to ensure that a scaled-down version of a fully functional environment is always running in the AWS cloud, and in case of a disaster, the recovery time is kept to a minimum. Which disaster recovery strategy is that?

**Lựa chọn:**

<label for="q236-a"><input type="radio" id="q236-a" name="q236" value="A"> <strong>A.</strong> Warm Standby</label><br>
<label for="q236-b"><input type="radio" id="q236-b" name="q236" value="B"> <strong>B.</strong> Pilot Light</label><br>
<label for="q236-c"><input type="radio" id="q236-c" name="q236" value="C"> <strong>C.</strong> Backup and Restore</label><br>
<label for="q236-d"><input type="radio" id="q236-d" name="q236" value="D"> <strong>D.</strong> Multi Site</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Warm Standby

</details>

---

## Câu 237

**Chủ đề:** Design Resilient Architectures

A fintech startup hosts its real-time transaction metadata in Amazon DynamoDB tables. During a recent system maintenance event, a junior engineer accidentally deleted a production table, resulting in major service downtime and irreversible data loss. Leadership has mandated an immediate solution that prevents future data loss from human error, while requiring minimal ongoing maintenance or manual effort from the engineering team.

Which approach best addresses these requirements with the least operational overhead?

**Lựa chọn:**

<label for="q237-a"><input type="radio" id="q237-a" name="q237" value="A"> <strong>A.</strong> Enable point-in-time recovery (PITR) on each DynamoDB table</label><br>
<label for="q237-b"><input type="radio" id="q237-b" name="q237" value="B"> <strong>B.</strong> Enable deletion protection on DynamoDB tables</label><br>
<label for="q237-c"><input type="radio" id="q237-c" name="q237" value="C"> <strong>C.</strong> Configure AWS CloudTrail to monitor DynamoDB API calls. Set up an Amazon EventBridge rule to detect DeleteTable events and trigger a Lambda function that recreates the deleted table using backup data stored in Amazon S3</label><br>
<label for="q237-d"><input type="radio" id="q237-d" name="q237" value="D"> <strong>D.</strong> Manually export each table as a full backup to Amazon S3 on a weekly basis. Use the DynamoDB export to S3 feature and rely on manual recovery if tables are deleted</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Enable deletion protection on DynamoDB tables

</details>

---

## Câu 238

**Chủ đề:** Design Cost-Optimized Architectures

You have an Amazon S3 bucket that contains files in two different folders - s3://my-bucket/images and s3://my-bucket/thumbnails. When an image is first uploaded and new, it is viewed several times. But after 45 days, analytics prove that image files are on average rarely requested, but the thumbnails still are. After 180 days, you would like to archive the image files and the thumbnails. Overall you would like the solution to remain highly available to prevent disasters happening against a whole Availability Zone (AZ).

How can you implement an efficient cost strategy for your Amazon S3 bucket? (Select two)

**Lựa chọn:**

<label for="q238-a"><input type="checkbox" id="q238-a" name="q238" value="A"> <strong>A.</strong> Create a Lifecycle Policy to transition objects to Amazon S3 One Zone IA using a prefix after 45 days</label><br>
<label for="q238-b"><input type="checkbox" id="q238-b" name="q238" value="B"> <strong>B.</strong> Create a Lifecycle Policy to transition objects to Amazon S3 Standard IA using a prefix after 45 days</label><br>
<label for="q238-c"><input type="checkbox" id="q238-c" name="q238" value="C"> <strong>C.</strong> Create a Lifecycle Policy to transition all objects to Amazon S3 Glacier after 180 days</label><br>
<label for="q238-d"><input type="checkbox" id="q238-d" name="q238" value="D"> <strong>D.</strong> Create a Lifecycle Policy to transition all objects to Amazon S3 Standard IA after 45 days</label><br>
<label for="q238-e"><input type="checkbox" id="q238-e" name="q238" value="E"> <strong>E.</strong> Create a Lifecycle Policy to transition objects to Amazon S3 Glacier using a prefix after 180 days</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create a Lifecycle Policy to transition objects to Amazon S3 Standard IA using a prefix after 45 days

C. Create a Lifecycle Policy to transition all objects to Amazon S3 Glacier after 180 days

</details>

---

## Câu 239

**Chủ đề:** Design Cost-Optimized Architectures

You have developed a new REST API leveraging the Amazon API Gateway, AWS Lambda and Amazon Aurora database services. Most of the workload on the website is read-heavy. The data rarely changes and it is acceptable to serve users outdated data for about 24 hours. Recently, the website has been experiencing high load and the costs incurred on the Aurora database have been very high.

How can you easily reduce the costs while improving performance, with minimal changes?

**Lựa chọn:**

<label for="q239-a"><input type="radio" id="q239-a" name="q239" value="A"> <strong>A.</strong> Add Amazon Aurora Read Replicas</label><br>
<label for="q239-b"><input type="radio" id="q239-b" name="q239" value="B"> <strong>B.</strong> Enable Amazon API Gateway Caching</label><br>
<label for="q239-c"><input type="radio" id="q239-c" name="q239" value="C"> <strong>C.</strong> Enable AWS Lambda In Memory Caching</label><br>
<label for="q239-d"><input type="radio" id="q239-d" name="q239" value="D"> <strong>D.</strong> Switch to using an Application Load Balancer</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Enable Amazon API Gateway Caching

</details>

---

## Câu 240

**Chủ đề:** Design Resilient Architectures

A small rental company had 5 employees, all working under the same AWS cloud account. These employees deployed their applications built for various functions- including billing, operations, finance, etc. Each of these employees has been operating in their own VPC. Now, there is a need to connect these VPCs so that the applications can communicate with each other.

Which of the following is the MOST cost-effective solution for this use-case?

**Lựa chọn:**

<label for="q240-a"><input type="radio" id="q240-a" name="q240" value="A"> <strong>A.</strong> Use an AWS Direct Connect connection</label><br>
<label for="q240-b"><input type="radio" id="q240-b" name="q240" value="B"> <strong>B.</strong> Use a VPC peering connection</label><br>
<label for="q240-c"><input type="radio" id="q240-c" name="q240" value="C"> <strong>C.</strong> Use an Internet Gateway</label><br>
<label for="q240-d"><input type="radio" id="q240-d" name="q240" value="D"> <strong>D.</strong> Use a Network Address Translation gateway (NAT gateway)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use a VPC peering connection

</details>

---

## Câu 241

**Chủ đề:** Design Cost-Optimized Architectures

You are working as a Solutions Architect for a photo processing company that has a proprietary algorithm to compress an image without any loss in quality. Because of the efficiency of the algorithm, your clients are willing to wait for a response that carries their compressed images back. You also want to process these jobs asynchronously and scale quickly, to cater to the high demand. Additionally, you also want the job to be retried in case of failures.

Which combination of choices do you recommend to minimize cost and comply with the requirements? (Select two)

**Lựa chọn:**

<label for="q241-a"><input type="checkbox" id="q241-a" name="q241" value="A"> <strong>A.</strong> Amazon Simple Notification Service (Amazon SNS)</label><br>
<label for="q241-b"><input type="checkbox" id="q241-b" name="q241" value="B"> <strong>B.</strong> Amazon EC2 Spot Instances</label><br>
<label for="q241-c"><input type="checkbox" id="q241-c" name="q241" value="C"> <strong>C.</strong> Amazon Simple Queue Service (Amazon SQS)</label><br>
<label for="q241-d"><input type="checkbox" id="q241-d" name="q241" value="D"> <strong>D.</strong> Amazon EC2 Reserved Instances (RIs)</label><br>
<label for="q241-e"><input type="checkbox" id="q241-e" name="q241" value="E"> <strong>E.</strong> Amazon EC2 On-Demand Instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Amazon EC2 Spot Instances

C. Amazon Simple Queue Service (Amazon SQS)

</details>

---

## Câu 242

**Chủ đề:** Design High-Performing Architectures

You started a new job as a solutions architect at a company that has both AWS experts and people learning AWS. Recently, a developer misconfigured a newly created Amazon RDS database which resulted in a production outage.

How can you ensure that Amazon RDS specific best practices are incorporated into a reusable infrastructure template to be used by all your AWS users?

**Lựa chọn:**

<label for="q242-a"><input type="radio" id="q242-a" name="q242" value="A"> <strong>A.</strong> Store your recommendations in a custom AWS Trusted Advisor rule</label><br>
<label for="q242-b"><input type="radio" id="q242-b" name="q242" value="B"> <strong>B.</strong> Create an AWS Lambda function which sends emails when it finds misconfigured Amazon RDS databases</label><br>
<label for="q242-c"><input type="radio" id="q242-c" name="q242" value="C"> <strong>C.</strong> Use AWS CloudFormation to manage Amazon RDS databases</label><br>
<label for="q242-d"><input type="radio" id="q242-d" name="q242" value="D"> <strong>D.</strong> Attach an IAM policy to interns preventing them from creating an Amazon RDS database</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use AWS CloudFormation to manage Amazon RDS databases

</details>

---

## Câu 243

**Chủ đề:** Design Secure Architectures

A company wants to adopt a hybrid cloud infrastructure where it uses some AWS services such as Amazon S3 alongside its on-premises data center. The company wants a dedicated private connection between the on-premise data center and AWS. In case of failures though, the company needs to guarantee uptime and is willing to use the public internet for an encrypted connection.

What do you recommend? (Select two)

**Lựa chọn:**

<label for="q243-a"><input type="checkbox" id="q243-a" name="q243" value="A"> <strong>A.</strong> Use AWS Direct Connect connection as a primary connection</label><br>
<label for="q243-b"><input type="checkbox" id="q243-b" name="q243" value="B"> <strong>B.</strong> Use AWS Site-to-Site VPN as a primary connection</label><br>
<label for="q243-c"><input type="checkbox" id="q243-c" name="q243" value="C"> <strong>C.</strong> Use Egress Only Internet Gateway as a backup connection</label><br>
<label for="q243-d"><input type="checkbox" id="q243-d" name="q243" value="D"> <strong>D.</strong> Use AWS Site-to-Site VPN as a backup connection</label><br>
<label for="q243-e"><input type="checkbox" id="q243-e" name="q243" value="E"> <strong>E.</strong> Use AWS Direct Connect connection as a backup connection</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS Direct Connect connection as a primary connection

D. Use AWS Site-to-Site VPN as a backup connection

</details>

---

## Câu 244

**Chủ đề:** Design Cost-Optimized Architectures

As an e-sport tournament hosting company, you have servers that need to scale and be highly available. Therefore you have deployed an Elastic Load Balancing (ELB) with an Auto Scaling group (ASG) across 3 Availability Zones (AZs). When e-sport tournaments are running, the servers need to scale quickly. And when tournaments are done, the servers can be idle. As a general rule, you would like to be highly available, have the capacity to scale and optimize your costs.

What do you recommend? (Select two)

**Lựa chọn:**

<label for="q244-a"><input type="checkbox" id="q244-a" name="q244" value="A"> <strong>A.</strong> Set the minimum capacity to 1</label><br>
<label for="q244-b"><input type="checkbox" id="q244-b" name="q244" value="B"> <strong>B.</strong> Set the minimum capacity to 3</label><br>
<label for="q244-c"><input type="checkbox" id="q244-c" name="q244" value="C"> <strong>C.</strong> Set the minimum capacity to 2</label><br>
<label for="q244-d"><input type="checkbox" id="q244-d" name="q244" value="D"> <strong>D.</strong> Use Dedicated hosts for the minimum capacity</label><br>
<label for="q244-e"><input type="checkbox" id="q244-e" name="q244" value="E"> <strong>E.</strong> Use Reserved Instances (RIs) for the minimum capacity</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set the minimum capacity to 2

E. Use Reserved Instances (RIs) for the minimum capacity

</details>

---

## Câu 245

**Chủ đề:** Design High-Performing Architectures

A ride-hailing startup has launched a mobile app that matches passengers with nearby drivers based on real-time GPS coordinates. The application backend uses an Amazon RDS for PostgreSQL instance with read replicas to store the latitude and longitude of drivers and passengers. As the service scales, the backend experiences performance bottlenecks during peak hours, especially when thousands of updates and reads occur per second to keep location data current. The company expects its user base to double in the next few months and needs a high-performance, scalable solution that can handle frequent write and read operations with minimal latency.

What do you recommend?

**Lựa chọn:**

<label for="q245-a"><input type="radio" id="q245-a" name="q245" value="A"> <strong>A.</strong> Create a read-replica Auto Scaling policy for the PostgreSQL database to dynamically add replicas during peak load. Distribute traffic evenly using an RDS proxy with failover configuration</label><br>
<label for="q245-b"><input type="radio" id="q245-b" name="q245" value="B"> <strong>B.</strong> Migrate the location data to Amazon OpenSearch Service and use its geospatial indexing features to retrieve and store coordinates in near real-time. Visualize tracking data using OpenSearch Dashboards</label><br>
<label for="q245-c"><input type="radio" id="q245-c" name="q245" value="C"> <strong>C.</strong> Place an Amazon ElastiCache for Redis cluster in front of the PostgreSQL database. Modify the application to cache recent location reads and updates in Redis, using a TTL-based eviction strategy</label><br>
<label for="q245-d"><input type="radio" id="q245-d" name="q245" value="D"> <strong>D.</strong> Enable Multi-AZ deployment for the primary RDS instance to improve write resilience and fault tolerance. Use Multi-AZ standby failover to distribute reads during peak hours</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Place an Amazon ElastiCache for Redis cluster in front of the PostgreSQL database. Modify the application to cache recent location reads and updates in Redis, using a TTL-based eviction strategy

</details>

---

## Câu 246

**Chủ đề:** Design High-Performing Architectures

A company's business logic is built on several microservices that are running in the on-premises data center. They currently communicate using a message broker that supports the MQTT protocol. The company is looking at migrating these applications and the message broker to AWS Cloud without changing the application logic.

Which technology allows you to get a managed message broker that supports the MQTT protocol?

**Lựa chọn:**

<label for="q246-a"><input type="radio" id="q246-a" name="q246" value="A"> <strong>A.</strong> Amazon MQ</label><br>
<label for="q246-b"><input type="radio" id="q246-b" name="q246" value="B"> <strong>B.</strong> Amazon Simple Queue Service (Amazon SQS)</label><br>
<label for="q246-c"><input type="radio" id="q246-c" name="q246" value="C"> <strong>C.</strong> Amazon Simple Notification Service (Amazon SNS)</label><br>
<label for="q246-d"><input type="radio" id="q246-d" name="q246" value="D"> <strong>D.</strong> Amazon Kinesis Data Streams</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon MQ

</details>

---

## Câu 247

**Chủ đề:** Design Secure Architectures

A developer in your company has set up a classic 2 tier architecture consisting of an Application Load Balancer and an Auto Scaling group (ASG) managing a fleet of Amazon EC2 instances. The Application Load Balancer is deployed in a subnet of size 10.0.1.0/24 and the Auto Scaling group is deployed in a subnet of size 10.0.4.0/22.

As a solutions architect, you would like to adhere to the security pillar of the well-architected framework. How do you configure the security group of the Amazon EC2 instances to only allow traffic coming from the Application Load Balancer?

**Lựa chọn:**

<label for="q247-a"><input type="radio" id="q247-a" name="q247" value="A"> <strong>A.</strong> Add a rule to authorize the security group of the Application Load Balancer</label><br>
<label for="q247-b"><input type="radio" id="q247-b" name="q247" value="B"> <strong>B.</strong> Add a rule to authorize the CIDR 10.0.4.0/22</label><br>
<label for="q247-c"><input type="radio" id="q247-c" name="q247" value="C"> <strong>C.</strong> Add a rule to authorize the security group of the Auto Scaling group</label><br>
<label for="q247-d"><input type="radio" id="q247-d" name="q247" value="D"> <strong>D.</strong> Add a rule to authorize the CIDR 10.0.1.0/24</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Add a rule to authorize the security group of the Application Load Balancer

</details>

---

## Câu 248

**Chủ đề:** Design High-Performing Architectures

The engineering team at a leading e-commerce company is anticipating a surge in the traffic because of a flash sale planned for the weekend. You have estimated the web traffic to be 10x. The content of your website is highly dynamic and changes very often.

As a Solutions Architect, which of the following options would you recommend to make sure your infrastructure scales for that day?

**Lựa chọn:**

<label for="q248-a"><input type="radio" id="q248-a" name="q248" value="A"> <strong>A.</strong> Use an Amazon Route 53 Multi Value record</label><br>
<label for="q248-b"><input type="radio" id="q248-b" name="q248" value="B"> <strong>B.</strong> Use an Amazon CloudFront distribution in front of your website</label><br>
<label for="q248-c"><input type="radio" id="q248-c" name="q248" value="C"> <strong>C.</strong> Use an Auto Scaling Group</label><br>
<label for="q248-d"><input type="radio" id="q248-d" name="q248" value="D"> <strong>D.</strong> Deploy the website on Amazon S3</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use an Auto Scaling Group

</details>

---

## Câu 249

**Chủ đề:** Design High-Performing Architectures

A niche social media application allows users to connect with sports athletes. As a solutions architect, you've designed the architecture of the application to be fully serverless using Amazon API Gateway and AWS Lambda. The backend uses an Amazon DynamoDB table. Some of the star athletes using the application are highly popular, and therefore Amazon DynamoDB has increased the read capacity units (RCUs). Still, the application is experiencing a hot partition problem.

What can you do to improve the performance of Amazon DynamoDB and eliminate the hot partition problem without a lot of application refactoring?

**Lựa chọn:**

<label for="q249-a"><input type="radio" id="q249-a" name="q249" value="A"> <strong>A.</strong> Use Amazon ElastiCache</label><br>
<label for="q249-b"><input type="radio" id="q249-b" name="q249" value="B"> <strong>B.</strong> Use Amazon DynamoDB Streams</label><br>
<label for="q249-c"><input type="radio" id="q249-c" name="q249" value="C"> <strong>C.</strong> Use Amazon DynamoDB DAX</label><br>
<label for="q249-d"><input type="radio" id="q249-d" name="q249" value="D"> <strong>D.</strong> Use Amazon DynamoDB Global Tables</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Amazon DynamoDB DAX

</details>

---

## Câu 250

**Chủ đề:** Design Cost-Optimized Architectures

A genomics research firm is processing sporadic bursts of data-intensive workloads using Amazon EC2 instances. The shared storage must support unpredictable spikes in file operations, but the average daily throughput demand remains relatively low. The team has selected Amazon Elastic File System (EFS) for its scalability and wants to ensure optimal cost and performance during bursts without provisioning throughput manually.

Which approach should the team take to best meet these requirements?

**Lựa chọn:**

<label for="q250-a"><input type="radio" id="q250-a" name="q250" value="A"> <strong>A.</strong> Switch the EFS storage class to EFS One Zone to reduce cost, which will automatically enable burst throughput mode</label><br>
<label for="q250-b"><input type="radio" id="q250-b" name="q250" value="B"> <strong>B.</strong> Change the throughput mode to provisioned and configure the desired throughput value to support burst workloads</label><br>
<label for="q250-c"><input type="radio" id="q250-c" name="q250" value="C"> <strong>C.</strong> Enable EFS Infrequent Access (IA) storage class to reduce storage cost while continuing to benefit from burst throughput mode</label><br>
<label for="q250-d"><input type="radio" id="q250-d" name="q250" value="D"> <strong>D.</strong> Enable EFS burst throughput mode on the file system using the General Purpose performance mode and EFS Standard storage class</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Enable EFS burst throughput mode on the file system using the General Purpose performance mode and EFS Standard storage class

</details>

---

## Câu 251

**Chủ đề:** Design Resilient Architectures

A media company operates a video rendering pipeline on Amazon EKS, where containerized jobs are scheduled using Kubernetes deployments. The application experiences bursty traffic patterns, particularly during peak streaming hours. The platform uses the Kubernetes Horizontal Pod Autoscaler (HPA) to scale pods based on CPU utilization. A solutions architect observes that the total number of EC2 worker nodes remains constant during traffic spikes, even when all nodes are at maximum resource utilization. The company needs a solution that enables automatic scaling of the underlying compute infrastructure when pod demand exceeds cluster capacity.

Which solution should the architect implement to resolve this issue with the least operational overhead?

**Lựa chọn:**

<label for="q251-a"><input type="radio" id="q251-a" name="q251" value="A"> <strong>A.</strong> Enable Amazon EC2 Auto Scaling with custom CloudWatch alarms based on cluster-wide CPU and memory usage to dynamically adjust node count in the EKS worker node group</label><br>
<label for="q251-b"><input type="radio" id="q251-b" name="q251" value="B"> <strong>B.</strong> Implement an AWS Lambda function that runs every 10 minutes and checks EKS pod scheduling status. Trigger node scaling manually using the eksctl CLI or AWS SDK if unschedulable pods are detected</label><br>
<label for="q251-c"><input type="radio" id="q251-c" name="q251" value="C"> <strong>C.</strong> Use AWS Fargate to replace the EKS worker nodes with serverless compute profiles, allowing Fargate to scale pods automatically without managing EC2 infrastructure</label><br>
<label for="q251-d"><input type="radio" id="q251-d" name="q251" value="D"> <strong>D.</strong> Deploy the Kubernetes Cluster Autoscaler to the EKS cluster. Configure it to integrate with the existing EC2 Auto Scaling group to automatically launch or terminate nodes based on pending pod demands</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Deploy the Kubernetes Cluster Autoscaler to the EKS cluster. Configure it to integrate with the existing EC2 Auto Scaling group to automatically launch or terminate nodes based on pending pod demands

</details>

---

## Câu 252

**Chủ đề:** Design Resilient Architectures

A development team has configured Elastic Load Balancing for host-based routing. The idea is to support multiple subdomains and different top-level domains.

The rule *.example.com matches which of the following?

**Lựa chọn:**

<label for="q252-a"><input type="radio" id="q252-a" name="q252" value="A"> <strong>A.</strong> example.com</label><br>
<label for="q252-b"><input type="radio" id="q252-b" name="q252" value="B"> <strong>B.</strong> example.test.com</label><br>
<label for="q252-c"><input type="radio" id="q252-c" name="q252" value="C"> <strong>C.</strong> EXAMPLE.COM</label><br>
<label for="q252-d"><input type="radio" id="q252-d" name="q252" value="D"> <strong>D.</strong> test.example.com</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. test.example.com

</details>

---

## Câu 253

**Chủ đề:** Design High-Performing Architectures

A company uses Application Load Balancers in multiple AWS Regions. The Application Load Balancers receive inconsistent traffic that varies throughout the year. The engineering team at the company needs to allow the IP addresses of the Application Load Balancers in the on-premises firewall to enable connectivity.

Which of the following represents the MOST scalable solution with minimal configuration changes?

**Lựa chọn:**

<label for="q253-a"><input type="radio" id="q253-a" name="q253" value="A"> <strong>A.</strong> Migrate all Application Load Balancers in different Regions to the Network Load Balancers. Configure the on-premises firewall's rule to allow the Elastic IP addresses of all the Network Load Balancers</label><br>
<label for="q253-b"><input type="radio" id="q253-b" name="q253" value="B"> <strong>B.</strong> Set up a Network Load Balancer in one Region. Register the private IP addresses of the Application Load Balancers in different Regions with the Network Load Balancer. Configure the on-premises firewall's rule to allow the Elastic IP address attached to the Network Load Balancer</label><br>
<label for="q253-c"><input type="radio" id="q253-c" name="q253" value="C"> <strong>C.</strong> Develop an AWS Lambda script to get the IP addresses of the Application Load Balancers in different Regions. Configure the on-premises firewall's rule to allow the IP addresses of the Application Load Balancers</label><br>
<label for="q253-d"><input type="radio" id="q253-d" name="q253" value="D"> <strong>D.</strong> Set up AWS Global Accelerator. Register the Application Load Balancers in different Regions to the AWS Global Accelerator. Configure the on-premises firewall's rule to allow static IP addresses associated with the AWS Global Accelerator</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up AWS Global Accelerator. Register the Application Load Balancers in different Regions to the AWS Global Accelerator. Configure the on-premises firewall's rule to allow static IP addresses associated with the AWS Global Accelerator

</details>

---

## Câu 254

**Chủ đề:** Design High-Performing Architectures

Amazon Route 53 is configured to route traffic to two Network Load Balancer nodes belonging to two Availability Zones (AZs): AZ-A and AZ-B. Cross-zone load balancing is disabled. AZ-A has four targets and AZ-B has six targets.

Which of the below statements is true about traffic distribution to the target instances from Amazon Route 53?

**Lựa chọn:**

<label for="q254-a"><input type="radio" id="q254-a" name="q254" value="A"> <strong>A.</strong> Each of the six targets in AZ-B receives 10% of the traffic</label><br>
<label for="q254-b"><input type="radio" id="q254-b" name="q254" value="B"> <strong>B.</strong> Each of the four targets in AZ-A receives 8% of the traffic</label><br>
<label for="q254-c"><input type="radio" id="q254-c" name="q254" value="C"> <strong>C.</strong> Each of the four targets in AZ-A receives 12.5% of the traffic</label><br>
<label for="q254-d"><input type="radio" id="q254-d" name="q254" value="D"> <strong>D.</strong> Each of the four targets in AZ-A receives 10% of the traffic</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Each of the four targets in AZ-A receives 12.5% of the traffic

</details>

---

## Câu 255

**Chủ đề:** Design High-Performing Architectures

An IT company runs a high-performance computing (HPC) workload on AWS. The workload requires high network throughput and low-latency network performance along with tightly coupled node-to-node communications. The Amazon EC2 instances are properly sized for compute and storage capacity and are launched using default options.

Which of the following solutions can be used to improve the performance of the workload?

**Lựa chọn:**

<label for="q255-a"><input type="radio" id="q255-a" name="q255" value="A"> <strong>A.</strong> Select the appropriate capacity reservation while launching Amazon EC2 instances</label><br>
<label for="q255-b"><input type="radio" id="q255-b" name="q255" value="B"> <strong>B.</strong> Select a cluster placement group while launching Amazon EC2 instances</label><br>
<label for="q255-c"><input type="radio" id="q255-c" name="q255" value="C"> <strong>C.</strong> Select dedicated instance tenancy while launching Amazon EC2 instances</label><br>
<label for="q255-d"><input type="radio" id="q255-d" name="q255" value="D"> <strong>D.</strong> Select an Elastic Inference accelerator while launching Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Select a cluster placement group while launching Amazon EC2 instances

</details>

---

## Câu 256

**Chủ đề:** Design High-Performing Architectures

A social media company wants the capability to dynamically alter the size of a geographic area from which traffic is routed to a specific server resource.

Which feature of Amazon Route 53 can help achieve this functionality?

**Lựa chọn:**

<label for="q256-a"><input type="radio" id="q256-a" name="q256" value="A"> <strong>A.</strong> Geolocation routing</label><br>
<label for="q256-b"><input type="radio" id="q256-b" name="q256" value="B"> <strong>B.</strong> Latency-based routing</label><br>
<label for="q256-c"><input type="radio" id="q256-c" name="q256" value="C"> <strong>C.</strong> Geoproximity routing</label><br>
<label for="q256-d"><input type="radio" id="q256-d" name="q256" value="D"> <strong>D.</strong> Weighted routing</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Geoproximity routing

</details>

---

## Câu 257

**Chủ đề:** Design High-Performing Architectures

A ride-sharing company wants to use an Amazon DynamoDB table for data storage. The table will not be used during the night hours whereas the read and write traffic will often be unpredictable during day hours. When traffic spikes occur they will happen very quickly.

Which of the following will you recommend as the best-fit solution?

**Lựa chọn:**

<label for="q257-a"><input type="radio" id="q257-a" name="q257" value="A"> <strong>A.</strong> Set up Amazon DynamoDB table in the provisioned capacity mode with auto-scaling enabled</label><br>
<label for="q257-b"><input type="radio" id="q257-b" name="q257" value="B"> <strong>B.</strong> Set up Amazon DynamoDB table in the on-demand capacity mode</label><br>
<label for="q257-c"><input type="radio" id="q257-c" name="q257" value="C"> <strong>C.</strong> Set up Amazon DynamoDB table with a global secondary index</label><br>
<label for="q257-d"><input type="radio" id="q257-d" name="q257" value="D"> <strong>D.</strong> Set up Amazon DynamoDB global table in the provisioned capacity mode</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up Amazon DynamoDB table in the on-demand capacity mode

</details>

---

## Câu 258

**Chủ đề:** Design Resilient Architectures

The engineering team at a social media company has recently migrated to AWS Cloud from its on-premises data center. The team is evaluating Amazon CloudFront to be used as a CDN for its flagship application. The team has hired you as an AWS Certified Solutions Architect – Associate to advise on Amazon CloudFront capabilities on routing, security, and high availability.

Which of the following would you identify as correct regarding Amazon CloudFront? (Select three)

**Lựa chọn:**

<label for="q258-a"><input type="checkbox" id="q258-a" name="q258" value="A"> <strong>A.</strong> Use AWS Key Management Service (AWS KMS) encryption in Amazon CloudFront to protect sensitive data for specific content</label><br>
<label for="q258-b"><input type="checkbox" id="q258-b" name="q258" value="B"> <strong>B.</strong> Use geo restriction to configure Amazon CloudFront for high-availability and failover</label><br>
<label for="q258-c"><input type="checkbox" id="q258-c" name="q258" value="C"> <strong>C.</strong> Amazon CloudFront can route to multiple origins based on the price class</label><br>
<label for="q258-d"><input type="checkbox" id="q258-d" name="q258" value="D"> <strong>D.</strong> Amazon CloudFront can route to multiple origins based on the content type</label><br>
<label for="q258-e"><input type="checkbox" id="q258-e" name="q258" value="E"> <strong>E.</strong> Use an origin group with primary and secondary origins to configure Amazon CloudFront for high-availability and failover</label><br>
<label for="q258-f"><input type="checkbox" id="q258-f" name="q258" value="F"> <strong>F.</strong> Use field level encryption in Amazon CloudFront to protect sensitive data for specific content</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Amazon CloudFront can route to multiple origins based on the content type

E. Use an origin group with primary and secondary origins to configure Amazon CloudFront for high-availability and failover

F. Use field level encryption in Amazon CloudFront to protect sensitive data for specific content

</details>

---

## Câu 259

**Chủ đề:** Design Secure Architectures

A financial services company is implementing two separate data retention policies to comply with regulatory standards:

Policy A: Critical transaction records must be immediately available for audit and must not be deleted or overwritten for 7 years.

Policy B: Archived compliance data must be stored in a low-cost, long-term storage solution and locked from deletion or modification for at least 10 years.

As a solutions architect, which combination of AWS features should you recommend to enforce these policies effectively?

**Lựa chọn:**

<label for="q259-a"><input type="radio" id="q259-a" name="q259" value="A"> <strong>A.</strong> Use Amazon S3 Standard storage class with S3 Lifecycle policies for Policy A, and S3 Glacier Flexible Retrieval for Policy B</label><br>
<label for="q259-b"><input type="radio" id="q259-b" name="q259" value="B"> <strong>B.</strong> Use Amazon S3 Object Lock in Compliance mode for Policy A, and S3 Glacier Vault Lock for Policy B</label><br>
<label for="q259-c"><input type="radio" id="q259-c" name="q259" value="C"> <strong>C.</strong> Use Amazon S3 Glacier Vault Lock for both policies to reduce storage costs while enforcing retention</label><br>
<label for="q259-d"><input type="radio" id="q259-d" name="q259" value="D"> <strong>D.</strong> Use Amazon S3 Object Lock in Governance mode for both policies to ensure data cannot be deleted prematurely</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon S3 Object Lock in Compliance mode for Policy A, and S3 Glacier Vault Lock for Policy B

</details>

---

## Câu 260

**Chủ đề:** Design Secure Architectures

A company wants to grant access to an Amazon S3 bucket to users in its own AWS account as well as to users in another AWS account. Which of the following options can be used to meet this requirement?

**Lựa chọn:**

<label for="q260-a"><input type="radio" id="q260-a" name="q260" value="A"> <strong>A.</strong> Use either a bucket policy or a user policy to grant permission to users in its account as well as to users in another account</label><br>
<label for="q260-b"><input type="radio" id="q260-b" name="q260" value="B"> <strong>B.</strong> Use a bucket policy to grant permission to users in its account as well as to users in another account</label><br>
<label for="q260-c"><input type="radio" id="q260-c" name="q260" value="C"> <strong>C.</strong> Use a user policy to grant permission to users in its account as well as to users in another account</label><br>
<label for="q260-d"><input type="radio" id="q260-d" name="q260" value="D"> <strong>D.</strong> Use permissions boundary to grant permission to users in its account as well as to users in another account</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use a bucket policy to grant permission to users in its account as well as to users in another account

</details>

---

## Câu 261

**Chủ đề:** Design Resilient Architectures

A streaming solutions company is building a video streaming product by using an Application Load Balancer (ALB) that routes the requests to the underlying Amazon EC2 instances. The engineering team has noticed a peculiar pattern. The Application Load Balancer removes an instance from its pool of healthy instances whenever it is detected as unhealthy but the Auto Scaling group fails to kick-in and provision the replacement instance.

What could explain this anomaly?

**Lựa chọn:**

<label for="q261-a"><input type="radio" id="q261-a" name="q261" value="A"> <strong>A.</strong> The Auto Scaling group is using Amazon EC2 based health check and the Application Load Balancer is using ALB based health check</label><br>
<label for="q261-b"><input type="radio" id="q261-b" name="q261" value="B"> <strong>B.</strong> The Auto Scaling group is using ALB based health check and the Application Load Balancer is using Amazon EC2 based health check</label><br>
<label for="q261-c"><input type="radio" id="q261-c" name="q261" value="C"> <strong>C.</strong> Both the Auto Scaling group and Application Load Balancer are using ALB based health check</label><br>
<label for="q261-d"><input type="radio" id="q261-d" name="q261" value="D"> <strong>D.</strong> Both the Auto Scaling group and Application Load Balancer are using Amazon EC2 based health check</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The Auto Scaling group is using Amazon EC2 based health check and the Application Load Balancer is using ALB based health check

</details>

---

## Câu 262

**Chủ đề:** Design Cost-Optimized Architectures

A retail company maintains an AWS Direct Connect connection to AWS and has recently migrated its data warehouse to AWS. The data analysts at the company query the data warehouse using a visualization tool. The average size of a query returned by the data warehouse is 60 megabytes and the query responses returned by the data warehouse are not cached in the visualization tool. Each webpage returned by the visualization tool is approximately 600 kilobytes.

Which of the following options offers the LOWEST data transfer egress cost for the company?

**Lựa chọn:**

<label for="q262-a"><input type="radio" id="q262-a" name="q262" value="A"> <strong>A.</strong> Deploy the visualization tool in the same AWS region as the data warehouse. Access the visualization tool over the internet at a location in the same region</label><br>
<label for="q262-b"><input type="radio" id="q262-b" name="q262" value="B"> <strong>B.</strong> Deploy the visualization tool on-premises. Query the data warehouse directly over an AWS Direct Connect connection at a location in the same AWS region</label><br>
<label for="q262-c"><input type="radio" id="q262-c" name="q262" value="C"> <strong>C.</strong> Deploy the visualization tool in the same AWS region as the data warehouse. Access the visualization tool over a Direct Connect connection at a location in the same region</label><br>
<label for="q262-d"><input type="radio" id="q262-d" name="q262" value="D"> <strong>D.</strong> Deploy the visualization tool on-premises. Query the data warehouse over the internet at a location in the same AWS region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Deploy the visualization tool in the same AWS region as the data warehouse. Access the visualization tool over a Direct Connect connection at a location in the same region

</details>

---

## Câu 263

**Chủ đề:** Design Resilient Architectures

The engineering team at an e-commerce company uses an AWS Lambda function to write the order data into a single DB instance Amazon Aurora cluster. The team has noticed that many order- writes to its Aurora cluster are getting missed during peak load times. The diagnostics data has revealed that the database is experiencing high CPU and memory consumption during traffic spikes. The team also wants to enhance the availability of the Aurora DB.

Which of the following steps would you combine to address the given scenario? (Select two)

**Lựa chọn:**

<label for="q263-a"><input type="checkbox" id="q263-a" name="q263" value="A"> <strong>A.</strong> Increase the concurrency of the AWS Lambda function so that the order-writes do not get missed during traffic spikes</label><br>
<label for="q263-b"><input type="checkbox" id="q263-b" name="q263" value="B"> <strong>B.</strong> Handle all read operations for your application by connecting to the reader endpoint of the Amazon Aurora cluster so that Aurora can spread the load for read-only connections across the Aurora replica</label><br>
<label for="q263-c"><input type="checkbox" id="q263-c" name="q263" value="C"> <strong>C.</strong> Create a standby Aurora instance in another Availability Zone to improve the availability as the standby can serve as a failover target</label><br>
<label for="q263-d"><input type="checkbox" id="q263-d" name="q263" value="D"> <strong>D.</strong> Create a replica Aurora instance in another Availability Zone to improve the availability as the replica can serve as a failover target</label><br>
<label for="q263-e"><input type="checkbox" id="q263-e" name="q263" value="E"> <strong>E.</strong> Use Amazon EC2 instances behind an Application Load Balancer to write the order data into Amazon Aurora cluster</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Handle all read operations for your application by connecting to the reader endpoint of the Amazon Aurora cluster so that Aurora can spread the load for read-only connections across the Aurora replica

D. Create a replica Aurora instance in another Availability Zone to improve the availability as the replica can serve as a failover target

</details>

---

## Câu 264

**Chủ đề:** Design High-Performing Architectures

A global enterprise is modernizing its hybrid IT infrastructure to improve both availability and network performance. The company operates a TCP-based application hosted on Amazon EC2 instances that are deployed across multiple AWS Regions, while a secondary UDP-based component of the application is hosted in its on-premises data centers. These application components must be accessed by customers around the world with minimal latency and consistent uptime.

Which combination of options should a solutions architect implement for the given use case? (Select two)

**Lựa chọn:**

<label for="q264-a"><input type="checkbox" id="q264-a" name="q264" value="A"> <strong>A.</strong> Configure an AWS Global Accelerator standard accelerator, and register the TCP-based EC2 workloads behind the load balancers</label><br>
<label for="q264-b"><input type="checkbox" id="q264-b" name="q264" value="B"> <strong>B.</strong> Set up AWS Direct Connect connections to route all TCP and UDP traffic through a single Region, using static routes and BGP failover</label><br>
<label for="q264-c"><input type="checkbox" id="q264-c" name="q264" value="C"> <strong>C.</strong> Deploy AWS PrivateLink to connect each on-premises UDP workload to the AWS Regions through interface endpoints exposed by the Network Load Balancers</label><br>
<label for="q264-d"><input type="checkbox" id="q264-d" name="q264" value="D"> <strong>D.</strong> Create a Network Load Balancer (NLB) in each Region to handle the EC2-based TCP traffic. For the UDP-based on-premises workload, configure NLBs in each Region to route to the on-premises endpoints via IP-based target groups</label><br>
<label for="q264-e"><input type="checkbox" id="q264-e" name="q264" value="E"> <strong>E.</strong> Create a Network Load Balancer (NLB) in each Region to handle the EC2-based TCP traffic. For the UDP-based on-premises workload, configure Application Load Balancers in each Region to route to the on-premises endpoints via IP-based target groups</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Configure an AWS Global Accelerator standard accelerator, and register the TCP-based EC2 workloads behind the load balancers

D. Create a Network Load Balancer (NLB) in each Region to handle the EC2-based TCP traffic. For the UDP-based on-premises workload, configure NLBs in each Region to route to the on-premises endpoints via IP-based target groups

</details>

---

## Câu 265

**Chủ đề:** Design Cost-Optimized Architectures

A media company wants to get out of the business of owning and maintaining its own IT infrastructure. As part of this digital transformation, the media company wants to archive about 5 petabytes of data in its on-premises data center to durable long term storage.

As a solutions architect, what is your recommendation to migrate this data in the MOST cost-optimal way?

**Lựa chọn:**

<label for="q265-a"><input type="radio" id="q265-a" name="q265" value="A"> <strong>A.</strong> Transfer the on-premises data into multiple AWS Snowball Edge Storage Optimized devices. Copy the AWS Snowball Edge data into Amazon S3 Glacier</label><br>
<label for="q265-b"><input type="radio" id="q265-b" name="q265" value="B"> <strong>B.</strong> Setup AWS direct connect between the on-premises data center and AWS Cloud. Use this connection to transfer the data into Amazon S3 Glacier</label><br>
<label for="q265-c"><input type="radio" id="q265-c" name="q265" value="C"> <strong>C.</strong> Setup AWS Site-to-Site VPN connection between the on-premises data center and AWS Cloud. Use this connection to transfer the data into Amazon S3 Glacier</label><br>
<label for="q265-d"><input type="radio" id="q265-d" name="q265" value="D"> <strong>D.</strong> Transfer the on-premises data into multiple AWS Snowball Edge Storage Optimized devices. Copy the AWS Snowball Edge data into Amazon S3 and create a lifecycle policy to transition the data into Amazon S3 Glacier</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Transfer the on-premises data into multiple AWS Snowball Edge Storage Optimized devices. Copy the AWS Snowball Edge data into Amazon S3 and create a lifecycle policy to transition the data into Amazon S3 Glacier

</details>

---

## Câu 266

**Chủ đề:** Design Resilient Architectures

A fintech company currently operates a real-time search and analytics platform on-premises. This platform ingests streaming data from multiple data-producing systems and provides immediate search capabilities and interactive visualizations for end users. As part of its cloud migration strategy, the company wants to rearchitect the solution using AWS-native services.

Which of the following represents the most efficient solution?

**Lựa chọn:**

<label for="q266-a"><input type="radio" id="q266-a" name="q266" value="A"> <strong>A.</strong> Deploy Amazon EC2 instances to handle the ingestion and processing of streaming data, storing the results in Amazon S3. Utilize Amazon Athena to search the stored data, and use Amazon Managed Grafana to generate dashboards and visual insights</label><br>
<label for="q266-b"><input type="radio" id="q266-b" name="q266" value="B"> <strong>B.</strong> Ingest and process the streaming data using Amazon Kinesis Data Streams, then index the data with Amazon OpenSearch Service for real-time search capabilities. Use Amazon QuickSight to build interactive dashboards and visualizations based on the indexed data</label><br>
<label for="q266-c"><input type="radio" id="q266-c" name="q266" value="C"> <strong>C.</strong> Use AWS Glue streaming ETL to process data streams and load the data into Amazon Redshift. Use Amazon Redshift’s full-text search capabilities for querying. Use Amazon QuickSight for data visualizations</label><br>
<label for="q266-d"><input type="radio" id="q266-d" name="q266" value="D"> <strong>D.</strong> Use Amazon Elastic Container Service (Amazon ECS) with AWS Fargate to ingest the data into Amazon DynamoDB to facilitate full text search. Use Amazon CloudWatch to create dashboards and query the data</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Ingest and process the streaming data using Amazon Kinesis Data Streams, then index the data with Amazon OpenSearch Service for real-time search capabilities. Use Amazon QuickSight to build interactive dashboards and visualizations based on the indexed data

</details>

---

## Câu 267

**Chủ đề:** Design Resilient Architectures

An enterprise SaaS provider is currently operating a legacy web application hosted on a single Amazon EC2 instance within a public subnet. The same instance also hosts a MySQL database. DNS records for the application are configured through Amazon Route 53. As part of a modernization initiative, the company wants to rearchitect this application for high availability and scalability. In addition, the company wants to improve read performance on the database layer to handle increasing user traffic.

Which combination of solutions will meet these requirements? (Select two)

**Lựa chọn:**

<label for="q267-a"><input type="checkbox" id="q267-a" name="q267" value="A"> <strong>A.</strong> Deploy an additional EC2 instance in a different AWS Region, and configure Amazon Route 53 with a failover routing policy to direct traffic to the secondary instance during primary Region outages</label><br>
<label for="q267-b"><input type="checkbox" id="q267-b" name="q267" value="B"> <strong>B.</strong> Use an Auto Scaling group to deploy EC2 instances across multiple Availability Zones within a single Region. Register the instances in a target group behind an Application Load Balancer to distribute web traffic evenly</label><br>
<label for="q267-c"><input type="checkbox" id="q267-c" name="q267" value="C"> <strong>C.</strong> Migrate the existing MySQL database to an Amazon Aurora MySQL cluster. Deploy the primary DB instance and one or more read replicas in different Availability Zones</label><br>
<label for="q267-d"><input type="checkbox" id="q267-d" name="q267" value="D"> <strong>D.</strong> Use an Auto Scaling group to deploy EC2 instances across multiple Availability Zones in two AWS Regions. Register the instances in a target group behind an Application Load Balancer to distribute web traffic evenly</label><br>
<label for="q267-e"><input type="checkbox" id="q267-e" name="q267" value="E"> <strong>E.</strong> Use Amazon CloudFront with Lambda@Edge to serve dynamic content from EC2 instances located in different Regions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use an Auto Scaling group to deploy EC2 instances across multiple Availability Zones within a single Region. Register the instances in a target group behind an Application Load Balancer to distribute web traffic evenly

C. Migrate the existing MySQL database to an Amazon Aurora MySQL cluster. Deploy the primary DB instance and one or more read replicas in different Availability Zones

</details>

---

## Câu 268

**Chủ đề:** Design High-Performing Architectures

An enterprise runs a critical Oracle database workload in its on-premises environment. The company now plans to replicate both existing records and continuous transactional changes to a managed Oracle environment in AWS. The target database will run on Amazon RDS for Oracle. Data transfer volume is expected to fluctuate throughout the day, and the team wants the solution to provision compute resources automatically based on actual workload requirements.

Which solution will meet these requirements?

**Lựa chọn:**

<label for="q268-a"><input type="radio" id="q268-a" name="q268" value="A"> <strong>A.</strong> Use AWS Glue to extract data from the on-premises Oracle database and write the output to Amazon RDS for Oracle. Configure Glue to run on demand when changes are detected</label><br>
<label for="q268-b"><input type="radio" id="q268-b" name="q268" value="B"> <strong>B.</strong> Deploy the AWS DMS replication instance on Amazon EC2. Configure the instance with custom scripts that monitor CPU usage and resize the instance using EC2 Auto Scaling policies.</label><br>
<label for="q268-c"><input type="radio" id="q268-c" name="q268" value="C"> <strong>C.</strong> Configure an AWS DMS Serverless replication task to synchronize historical and ongoing changes between the on-premises Oracle database and Amazon RDS for Oracle</label><br>
<label for="q268-d"><input type="radio" id="q268-d" name="q268" value="D"> <strong>D.</strong> Use AWS Lambda to capture change data from the on-premises Oracle database. Trigger Lambda functions to write the updates to Amazon RDS for Oracle in real time.</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Configure an AWS DMS Serverless replication task to synchronize historical and ongoing changes between the on-premises Oracle database and Amazon RDS for Oracle

</details>

---

## Câu 269

**Chủ đề:** Design Secure Architectures

A tech company runs a web application that includes multiple internal services deployed across Amazon EC2 instances within a VPC. These services require communication with a third-party SaaS provider's API for analytics and billing, which is also hosted on the AWS infrastructure. The company is concerned about minimizing public internet exposure while maintaining secure and reliable connectivity. The solution must ensure private access without allowing unsolicited incoming traffic from the SaaS provider.

Which solution will best meet these requirements?

**Lựa chọn:**

<label for="q269-a"><input type="radio" id="q269-a" name="q269" value="A"> <strong>A.</strong> Establish a VPN connection using AWS Site-to-Site VPN to create a secure tunnel between the internal services and the third-party SaaS provider</label><br>
<label for="q269-b"><input type="radio" id="q269-b" name="q269" value="B"> <strong>B.</strong> Use AWS PrivateLink to create a private endpoint within the application’s VPC that connects securely to the SaaS provider’s VPC</label><br>
<label for="q269-c"><input type="radio" id="q269-c" name="q269" value="C"> <strong>C.</strong> Set up VPC peering between the application VPC and the SaaS provider’s VPC to allow direct communication</label><br>
<label for="q269-d"><input type="radio" id="q269-d" name="q269" value="D"> <strong>D.</strong> Use AWS CloudFront to route requests from the application’s internal services to the SaaS provider through edge locations</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS PrivateLink to create a private endpoint within the application’s VPC that connects securely to the SaaS provider’s VPC

</details>

---

## Câu 270

**Chủ đề:** Design Secure Architectures

A retail enterprise is expanding its hybrid IT infrastructure and plans to securely connect its on-premises corporate network to its AWS environment. The company wants to ensure that all data exchanged between on-premises systems and AWS is encrypted at both the network and session layers. Additionally, the solution must incorporate granular security controls that restrict unnecessary or unauthorized access between the cloud and on-premises environments. A solutions architect must recommend a scalable and secure approach that supports these goals.

Which solution best meets these requirements?

**Lựa chọn:**

<label for="q270-a"><input type="radio" id="q270-a" name="q270" value="A"> <strong>A.</strong> Establish a dedicated AWS Direct Connect connection between the corporate network and AWS. Configure VPC route tables to control traffic flow and use security groups and network ACLs to restrict access as needed</label><br>
<label for="q270-b"><input type="radio" id="q270-b" name="q270" value="B"> <strong>B.</strong> Use AWS Client VPN to allow corporate users to connect to the VPC individually. Manage access controls with security groups and IAM policies</label><br>
<label for="q270-c"><input type="radio" id="q270-c" name="q270" value="C"> <strong>C.</strong> Set up AWS Site-to-Site VPN to connect the on-premises network to the AWS VPC. Use route tables to manage traffic flow and configure security groups and network ACLs to allow only authorized communication between systems</label><br>
<label for="q270-d"><input type="radio" id="q270-d" name="q270" value="D"> <strong>D.</strong> Set up a bastion host in a public subnet of the VPC to provide SSH-based access to AWS resources from the corporate network. Use security groups to control access</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set up AWS Site-to-Site VPN to connect the on-premises network to the AWS VPC. Use route tables to manage traffic flow and configure security groups and network ACLs to allow only authorized communication between systems

</details>

---

## Câu 271

**Chủ đề:** Design Resilient Architectures

A data analytics team at a global media firm is building a new analytics platform to process large volumes of both historical and real-time data. This data is stored in Amazon S3. The team wants to implement a serverless solution that allows them to query the data directly using SQL. Additionally, the solution must ensure that all data is encrypted at rest and automatically replicated to another AWS Region to support business continuity.

Which solution will meet these requirements with the LEAST operational overhead?

**Lựa chọn:**

<label for="q271-a"><input type="radio" id="q271-a" name="q271" value="A"> <strong>A.</strong> Create an Amazon S3 bucket configured with server-side encryption using AWS KMS multi-Region keys (SSE-KMS). Enable cross-Region replication (CRR) on the source bucket. Use Amazon Athena to run SQL queries on the data</label><br>
<label for="q271-b"><input type="radio" id="q271-b" name="q271" value="B"> <strong>B.</strong> Enable Cross-Region Replication (CRR) on the existing Amazon S3 bucket. Apply server-side encryption using Amazon S3 managed keys (SSE-S3). Use Amazon Athena to run SQL queries on the replicated data</label><br>
<label for="q271-c"><input type="radio" id="q271-c" name="q271" value="C"> <strong>C.</strong> Create an Amazon S3 bucket configured with server-side encryption using Amazon S3 managed keys (SSE-S3). Enable cross-Region replication (CRR) on the source bucket. Use Amazon Redshift Spectrum to query the S3 data using SQL</label><br>
<label for="q271-d"><input type="radio" id="q271-d" name="q271" value="D"> <strong>D.</strong> Enable Cross-Region Replication (CRR) on the existing Amazon S3 bucket. Apply server-side encryption using AWS KMS multi-Region keys (SSE-KMS). Use Amazon Athena to run SQL queries on the replicated data</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an Amazon S3 bucket configured with server-side encryption using AWS KMS multi-Region keys (SSE-KMS). Enable cross-Region replication (CRR) on the source bucket. Use Amazon Athena to run SQL queries on the data

</details>

---

## Câu 272

**Chủ đề:** Design Cost-Optimized Architectures

The data engineering team at an e-commerce company has set up a workflow to ingest the clickstream data into the raw zone of the Amazon S3 data lake. The team wants to run some SQL based data sanity checks on the raw zone of the data lake.

What AWS services would you recommend for this use-case such that the solution is cost-effective and easy to maintain?

**Lựa chọn:**

<label for="q272-a"><input type="radio" id="q272-a" name="q272" value="A"> <strong>A.</strong> Load the incremental raw zone data into Amazon Redshift on an hourly basis and run the SQL based sanity checks</label><br>
<label for="q272-b"><input type="radio" id="q272-b" name="q272" value="B"> <strong>B.</strong> Load the incremental raw zone data into Amazon RDS on an hourly basis and run the SQL based sanity checks</label><br>
<label for="q272-c"><input type="radio" id="q272-c" name="q272" value="C"> <strong>C.</strong> Load the incremental raw zone data into an Amazon EMR based Spark Cluster on an hourly basis and use SparkSQL to run the SQL based sanity checks</label><br>
<label for="q272-d"><input type="radio" id="q272-d" name="q272" value="D"> <strong>D.</strong> Use Amazon Athena to run SQL based analytics against Amazon S3 data</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon Athena to run SQL based analytics against Amazon S3 data

</details>

---

## Câu 273

**Chủ đề:** Design Secure Architectures

A global media company uses a fleet of Amazon EC2 instances (behind an Application Load Balancer) to power its video streaming application. To improve the performance of the application, the engineering team has also created an Amazon CloudFront distribution with the Application Load Balancer as the custom origin. The security team at the company has noticed a spike in the number and types of SQL injection and cross-site scripting attack vectors on the application.

As a solutions architect, which of the following solutions would you recommend as the MOST effective in countering these malicious attacks?

**Lựa chọn:**

<label for="q273-a"><input type="radio" id="q273-a" name="q273" value="A"> <strong>A.</strong> Use Amazon Route 53 with Amazon CloudFront distribution</label><br>
<label for="q273-b"><input type="radio" id="q273-b" name="q273" value="B"> <strong>B.</strong> Use AWS Firewall Manager with CloudFront distribution</label><br>
<label for="q273-c"><input type="radio" id="q273-c" name="q273" value="C"> <strong>C.</strong> Use AWS Security Hub with Amazon CloudFront distribution</label><br>
<label for="q273-d"><input type="radio" id="q273-d" name="q273" value="D"> <strong>D.</strong> Use AWS Web Application Firewall (AWS WAF) with Amazon CloudFront distribution</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Web Application Firewall (AWS WAF) with Amazon CloudFront distribution

</details>

---

## Câu 274

**Chủ đề:** Design Secure Architectures

The infrastructure team at a company maintains 5 different VPCs (let's call these VPCs A, B, C, D, E) for resource isolation. Due to the changed organizational structure, the team wants to interconnect all VPCs together. To facilitate this, the team has set up VPC peering connection between VPC A and all other VPCs in a hub and spoke model with VPC A at the center. However, the team has still failed to establish connectivity between all VPCs.

As a solutions architect, which of the following would you recommend as the MOST resource-efficient and scalable solution?

**Lựa chọn:**

<label for="q274-a"><input type="radio" id="q274-a" name="q274" value="A"> <strong>A.</strong> Establish VPC peering connections between all VPCs</label><br>
<label for="q274-b"><input type="radio" id="q274-b" name="q274" value="B"> <strong>B.</strong> Use AWS transit gateway to interconnect the VPCs</label><br>
<label for="q274-c"><input type="radio" id="q274-c" name="q274" value="C"> <strong>C.</strong> Use an internet gateway to interconnect the VPCs</label><br>
<label for="q274-d"><input type="radio" id="q274-d" name="q274" value="D"> <strong>D.</strong> Use a VPC endpoint to interconnect the VPCs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS transit gateway to interconnect the VPCs

</details>

---

## Câu 275

**Chủ đề:** Design Secure Architectures

A media company operates a web application that enables users to upload photos. These uploads are stored in an Amazon S3 bucket located in the eu-west-2 Region. To enhance performance and provide secure access under a custom domain name, the company wants to integrate Amazon CloudFront for uploads to the S3 bucket. The architecture must support secure HTTPS connections using a custom domain, and the upload process must ensure optimal speed and security.

Which combination of actions will fulfill these requirements? (Select two)

**Lựa chọn:**

<label for="q275-a"><input type="checkbox" id="q275-a" name="q275" value="A"> <strong>A.</strong> Create a CloudFront distribution with an S3 static website endpoint as the origin and enable upload operations</label><br>
<label for="q275-b"><input type="checkbox" id="q275-b" name="q275" value="B"> <strong>B.</strong> Set up a custom origin request policy in CloudFront that includes all viewer headers and query strings. Enable S3 Object Ownership to allow CloudFront to assume control of uploaded files via a signed URL</label><br>
<label for="q275-c"><input type="checkbox" id="q275-c" name="q275" value="C"> <strong>C.</strong> Request a public certificate from AWS Certificate Manager (ACM) in the us-east-1 Region and associate it with the CloudFront distribution</label><br>
<label for="q275-d"><input type="checkbox" id="q275-d" name="q275" value="D"> <strong>D.</strong> Request a public certificate from AWS Certificate Manager (ACM) in the eu-west-2 Region and associate it with the CloudFront distribution</label><br>
<label for="q275-e"><input type="checkbox" id="q275-e" name="q275" value="E"> <strong>E.</strong> Set up Amazon S3 to accept uploads from CloudFront by enabling origin access control (OAC)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Request a public certificate from AWS Certificate Manager (ACM) in the us-east-1 Region and associate it with the CloudFront distribution

E. Set up Amazon S3 to accept uploads from CloudFront by enabling origin access control (OAC)

</details>

---

## Câu 276

**Chủ đề:** Design Resilient Architectures

A company hosts a Microsoft SQL Server database on Amazon EC2 instances with attached Amazon EBS volumes. The operations team takes daily snapshots of these EBS volumes as backups. However, a recent incident occurred in which an automated script designed to clean up expired snapshots accidentally deleted all available snapshots, leading to potential data loss. The company wants to improve the backup strategy to avoid permanent data loss while still ensuring that old snapshots are eventually removed to optimize cost. A solutions architect needs to implement a mechanism that prevents immediate and irreversible deletion of snapshots.

Which solution will best meet these requirements with the least development effort?

**Lựa chọn:**

<label for="q276-a"><input type="radio" id="q276-a" name="q276" value="A"> <strong>A.</strong> Enable AWS Backup Vault Lock on the backup vault and store EBS snapshots in that vault to enforce deletion protection</label><br>
<label for="q276-b"><input type="radio" id="q276-b" name="q276" value="B"> <strong>B.</strong> Set up a 7-day EBS snapshot retention rule in Recycle Bin and apply the rule for all snapshots</label><br>
<label for="q276-c"><input type="radio" id="q276-c" name="q276" value="C"> <strong>C.</strong> Implement a Lambda-based backup automation workflow that archives snapshot metadata in DynamoDB and stores backups in Amazon S3 Glacier Deep Archive for long-term recovery</label><br>
<label for="q276-d"><input type="radio" id="q276-d" name="q276" value="D"> <strong>D.</strong> Set up the IAM policy of the user to deny EBS snapshot deletion</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up a 7-day EBS snapshot retention rule in Recycle Bin and apply the rule for all snapshots

</details>

---

## Câu 277

**Chủ đề:** Design Secure Architectures

A fintech company recently conducted a security audit and discovered that some IAM roles and Amazon S3 buckets might be unintentionally shared with external accounts or publicly accessible. The security team wants to identify these overly permissive resources and ensure that only intended principals (within their AWS Organization or specific AWS accounts) have access. They need a solution that can analyze IAM policies and resource policies to detect unintended access paths to AWS resources such as S3 buckets, IAM roles, KMS keys, and SNS topics.

Which solution should the team use to meet this requirement?

**Lựa chọn:**

<label for="q277-a"><input type="radio" id="q277-a" name="q277" value="A"> <strong>A.</strong> Use IAM Access Advisor to get detailed access analysis of S3 bucket policies and determine which principals outside the organization have access</label><br>
<label for="q277-b"><input type="radio" id="q277-b" name="q277" value="B"> <strong>B.</strong> Use AWS Config to track configuration changes and infer resource-sharing behavior by analyzing compliance rules</label><br>
<label for="q277-c"><input type="radio" id="q277-c" name="q277" value="C"> <strong>C.</strong> Use Amazon Inspector to detect over-permissive IAM policies and access paths across the environment</label><br>
<label for="q277-d"><input type="radio" id="q277-d" name="q277" value="D"> <strong>D.</strong> Use AWS Identity and Access Management (IAM) Access Analyzer to evaluate resource-based and identity-based policies and identify resources shared outside the account or organization</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Identity and Access Management (IAM) Access Analyzer to evaluate resource-based and identity-based policies and identify resources shared outside the account or organization

</details>

---

## Câu 278

**Chủ đề:** Design Secure Architectures

An enterprise is developing an internal compliance framework for its cloud infrastructure hosted on AWS. The enterprise uses AWS Organizations to group accounts under various organizational units (OUs) based on departmental function. As part of its governance controls, the security team mandates that all Amazon EC2 instances must be tagged to indicate the level of data classification — either 'confidential' or 'public'. Additionally, the organization must ensure that IAM users cannot launch EC2 instances without assigning a classification tag, nor should they be able to remove the tag from running instances. A solutions architect must design a solution to meet these compliance controls while minimizing operational overhead.

Which combination of steps will meet these requirements? (Select two)

**Lựa chọn:**

<label for="q278-a"><input type="checkbox" id="q278-a" name="q278" value="A"> <strong>A.</strong> Create a tag enforcement Lambda function that runs on a schedule to identify EC2 instances without the required tag. The function sends a notification to administrators and optionally shuts down noncompliant resources</label><br>
<label for="q278-b"><input type="checkbox" id="q278-b" name="q278" value="B"> <strong>B.</strong> Use AWS Identity and Access Management (IAM) permission boundaries to restrict EC2-related actions unless the dataClassification tag is present. Apply these boundaries to all IAM roles used for EC2 provisioning</label><br>
<label for="q278-c"><input type="checkbox" id="q278-c" name="q278" value="C"> <strong>C.</strong> Define a tag policy in AWS Organizations that enforces the dataClassification key and restricts values to 'confidential' and 'public'. Attach this tag policy to the applicable organizational unit (OU) to enforce uniform tagging behavior across accounts</label><br>
<label for="q278-d"><input type="checkbox" id="q278-d" name="q278" value="D"> <strong>D.</strong> Enable AWS Config rules to detect noncompliant EC2 instances. Trigger an AWS Systems Manager Automation runbook to reapply missing tags automatically when noncompliance is detected</label><br>
<label for="q278-e"><input type="checkbox" id="q278-e" name="q278" value="E"> <strong>E.</strong> Create a service control policy (SCP) that denies the ec2:RunInstances API action unless the required tag key is present in the request. Create a second SCP that denies the ec2:DeleteTags action for EC2 resources. Attach both SCPs to the relevant OU in AWS Organizations</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Define a tag policy in AWS Organizations that enforces the dataClassification key and restricts values to 'confidential' and 'public'. Attach this tag policy to the applicable organizational unit (OU) to enforce uniform tagging behavior across accounts

E. Create a service control policy (SCP) that denies the ec2:RunInstances API action unless the required tag key is present in the request. Create a second SCP that denies the ec2:DeleteTags action for EC2 resources. Attach both SCPs to the relevant OU in AWS Organizations

</details>

---

## Câu 279

**Chủ đề:** Design Cost-Optimized Architectures

A medium-sized business has a taxi dispatch application deployed on an Amazon EC2 instance. Because of an unknown bug, the application causes the instance to freeze regularly. Then, the instance has to be manually restarted via the AWS management console.

Which of the following is the MOST cost-optimal and resource-efficient way to implement an automated solution until a permanent fix is delivered by the development team?

**Lựa chọn:**

<label for="q279-a"><input type="radio" id="q279-a" name="q279" value="A"> <strong>A.</strong> Setup an Amazon CloudWatch alarm to monitor the health status of the instance. In case of an Instance Health Check failure, Amazon CloudWatch Alarm can publish to an Amazon Simple Notification Service (Amazon SNS) event which can then trigger an AWS lambda function. The AWS lambda function can use Amazon EC2 API to reboot the instance</label><br>
<label for="q279-b"><input type="radio" id="q279-b" name="q279" value="B"> <strong>B.</strong> Use Amazon EventBridge events to trigger an AWS Lambda function to check the instance status every 5 minutes. In the case of Instance Health Check failure, the AWS lambda function can use Amazon EC2 API to reboot the instance</label><br>
<label for="q279-c"><input type="radio" id="q279-c" name="q279" value="C"> <strong>C.</strong> Setup an Amazon CloudWatch alarm to monitor the health status of the instance. In case of an Instance Health Check failure, an EC2 Reboot CloudWatch Alarm Action can be used to reboot the instance</label><br>
<label for="q279-d"><input type="radio" id="q279-d" name="q279" value="D"> <strong>D.</strong> Use Amazon EventBridge events to trigger an AWS Lambda function to reboot the instance status every 5 minutes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Setup an Amazon CloudWatch alarm to monitor the health status of the instance. In case of an Instance Health Check failure, an EC2 Reboot CloudWatch Alarm Action can be used to reboot the instance

</details>

---

## Câu 280

**Chủ đề:** Design Resilient Architectures

A media streaming company expects a major increase in user activity during the launch of a highly anticipated live event. The streaming platform is deployed on AWS and uses Amazon EC2 instances for the application layer and Amazon RDS for persistent storage. The operations team needs to proactively monitor system performance to ensure a smooth user experience during the event. Their monitoring setup must provide data visibility with intervals of no more than 2 minutes, and the team prefers a solution that is quick to implement and low-maintenance.

Which solution should the team implement?

**Lựa chọn:**

<label for="q280-a"><input type="radio" id="q280-a" name="q280" value="A"> <strong>A.</strong> Use Amazon EventBridge to collect EC2 state changes and publish them to Amazon SNS. Subscribe a monitoring dashboard to the SNS topic to visualize metrics</label><br>
<label for="q280-b"><input type="radio" id="q280-b" name="q280" value="B"> <strong>B.</strong> Enable detailed monitoring on all EC2 instances and use Amazon CloudWatch metrics to track performance</label><br>
<label for="q280-c"><input type="radio" id="q280-c" name="q280" value="C"> <strong>C.</strong> Stream EC2 system logs to an Amazon OpenSearch Service domain for real-time indexing and visualization. Use OpenSearch Dashboards to monitor CPU and memory metrics</label><br>
<label for="q280-d"><input type="radio" id="q280-d" name="q280" value="D"> <strong>D.</strong> Install the CloudWatch agent on all EC2 instances. Configure the agent to collect high-resolution custom metrics and stream them to CloudWatch Logs for analysis via Amazon Athena</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Enable detailed monitoring on all EC2 instances and use Amazon CloudWatch metrics to track performance

</details>

---

## Câu 281

**Chủ đề:** Design High-Performing Architectures

Reporters at a news agency upload/download video files (about 500 megabytes each) to/from an Amazon S3 bucket as part of their daily work. As the agency has started offices in remote locations, it has resulted in poor latency for uploading and accessing data to/from the given Amazon S3 bucket. The agency wants to continue using a serverless storage solution such as Amazon S3 but wants to improve the performance.

As a solutions architect, which of the following solutions do you propose to address this issue? (Select two)

**Lựa chọn:**

<label for="q281-a"><input type="checkbox" id="q281-a" name="q281" value="A"> <strong>A.</strong> Create new Amazon S3 buckets in every region where the agency has a remote office, so that each office can maintain its storage for the media assets</label><br>
<label for="q281-b"><input type="checkbox" id="q281-b" name="q281" value="B"> <strong>B.</strong> Move Amazon S3 data into Amazon Elastic File System (Amazon EFS) created in a US region, connect to Amazon EFS file system from Amazon EC2 instances in other AWS regions using an inter-region VPC peering connection</label><br>
<label for="q281-c"><input type="checkbox" id="q281-c" name="q281" value="C"> <strong>C.</strong> Use Amazon CloudFront distribution with origin as the Amazon S3 bucket. This would speed up uploads as well as downloads for the video files</label><br>
<label for="q281-d"><input type="checkbox" id="q281-d" name="q281" value="D"> <strong>D.</strong> Enable Amazon S3 Transfer Acceleration (Amazon S3TA) for the Amazon S3 bucket. This would speed up uploads as well as downloads for the video files</label><br>
<label for="q281-e"><input type="checkbox" id="q281-e" name="q281" value="E"> <strong>E.</strong> Spin up Amazon EC2 instances in each region where the agency has a remote office. Create a daily job to transfer Amazon S3 data into Amazon EBS volumes attached to the Amazon EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Amazon CloudFront distribution with origin as the Amazon S3 bucket. This would speed up uploads as well as downloads for the video files

D. Enable Amazon S3 Transfer Acceleration (Amazon S3TA) for the Amazon S3 bucket. This would speed up uploads as well as downloads for the video files

</details>

---

## Câu 282

**Chủ đề:** Design High-Performing Architectures

A company needs a massive PostgreSQL database and the engineering team would like to retain control over managing the patches, version upgrades for the database, and consistent performance with high IOPS. The team wants to install the database on an Amazon EC2 instance with the optimal storage type on the attached Amazon EBS volume.

As a solutions architect, which of the following configurations would you suggest to the engineering team?

**Lựa chọn:**

<label for="q282-a"><input type="radio" id="q282-a" name="q282" value="A"> <strong>A.</strong> Amazon EC2 with Amazon EBS volume of General Purpose SSD (gp2) type</label><br>
<label for="q282-b"><input type="radio" id="q282-b" name="q282" value="B"> <strong>B.</strong> Amazon EC2 with Amazon EBS volume of Provisioned IOPS SSD (io1) type</label><br>
<label for="q282-c"><input type="radio" id="q282-c" name="q282" value="C"> <strong>C.</strong> Amazon EC2 with Amazon EBS volume of Throughput Optimized HDD (st1) type</label><br>
<label for="q282-d"><input type="radio" id="q282-d" name="q282" value="D"> <strong>D.</strong> Amazon EC2 with Amazon EBS volume of cold HDD (sc1) type</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Amazon EC2 with Amazon EBS volume of Provisioned IOPS SSD (io1) type

</details>

---

## Câu 283

**Chủ đề:** Design High-Performing Architectures

A digital media startup allows users to submit images through its web portal. These images are uploaded directly into an Amazon S3 bucket. On average, around 200 images are uploaded daily. The company wants to automatically generate a smaller preview version (thumbnail) of each new image and store the resulting thumbnails in a separate Amazon S3 bucket. The team prefers a design that is low-cost, requires minimal infrastructure management, and automatically reacts to new uploads.

Which solution will meet these requirements MOST cost-effectively?

**Lựa chọn:**

<label for="q283-a"><input type="radio" id="q283-a" name="q283" value="A"> <strong>A.</strong> Set up a step-based processing workflow using AWS Glue jobs triggered on a regular interval. Use the jobs to scan the primary S3 bucket for new files and generate thumbnails for any that lack them. Write the thumbnails to a second S3 bucket</label><br>
<label for="q283-b"><input type="radio" id="q283-b" name="q283" value="B"> <strong>B.</strong> Deploy a containerized application on AWS Fargate that polls the S3 bucket every minute to detect new uploads. Configure the container to generate thumbnails and save them in the second bucket</label><br>
<label for="q283-c"><input type="radio" id="q283-c" name="q283" value="C"> <strong>C.</strong> Enable Amazon S3 Access Analyzer and configure it to call an AWS Lambda function whenever a new image is added. Use the Lambda function to generate and store the thumbnail</label><br>
<label for="q283-d"><input type="radio" id="q283-d" name="q283" value="D"> <strong>D.</strong> Configure the S3 bucket to send an event notification to an AWS Lambda function each time a new image is uploaded. Use the Lambda function to process the image, create a thumbnail, and store the thumbnail in the second S3 bucket</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Configure the S3 bucket to send an event notification to an AWS Lambda function each time a new image is uploaded. Use the Lambda function to process the image, create a thumbnail, and store the thumbnail in the second S3 bucket

</details>

---

## Câu 284

**Chủ đề:** Design Secure Architectures

An organization operates a legacy reporting tool hosted on an Amazon EC2 instance located within a public subnet of a VPC. This tool aggregates scanned PDF reports from field devices and temporarily stores them on an attached Amazon EBS volume. At the end of each day, the tool transfers the accumulated files to an Amazon S3 bucket for archival. A solutions architect identifies that the files are being uploaded over the internet using S3's public endpoint. To improve security and avoid exposing data traffic to the public internet, the architect needs to reconfigure the setup so that uploads to Amazon S3 occur privately without using the public S3 endpoint.

Which solution will fulfill these requirements?

**Lựa chọn:**

<label for="q284-a"><input type="radio" id="q284-a" name="q284" value="A"> <strong>A.</strong> Create a gateway VPC endpoint for Amazon S3 in the VPC. Ensure that the EC2 instance’s subnet route table is updated to route S3 traffic through the endpoint. Confirm that appropriate IAM policies are in place to permit access via the VPC endpoint</label><br>
<label for="q284-b"><input type="radio" id="q284-b" name="q284" value="B"> <strong>B.</strong> Create an S3 access point within the same Region and attach a policy that grants the EC2 instance access. Update the application to use the access point alias to upload data</label><br>
<label for="q284-c"><input type="radio" id="q284-c" name="q284" value="C"> <strong>C.</strong> Set up a NAT gateway in the public subnet and modify the route table of the EC2 instance's subnet to direct Amazon S3 traffic through the NAT gateway</label><br>
<label for="q284-d"><input type="radio" id="q284-d" name="q284" value="D"> <strong>D.</strong> Provision a dedicated AWS Direct Connect link to route traffic from the VPC to Amazon S3 privately</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a gateway VPC endpoint for Amazon S3 in the VPC. Ensure that the EC2 instance’s subnet route table is updated to route S3 traffic through the endpoint. Confirm that appropriate IAM policies are in place to permit access via the VPC endpoint

</details>

---

## Câu 285

**Chủ đề:** Design Resilient Architectures

A company wants to ensure high availability for its Amazon RDS database. The development team wants to opt for Multi-AZ deployment and they would like to understand what happens when the primary instance of the Multi-AZ configuration goes down.

As a Solutions Architect, which of the following will you identify as the outcome of the scenario?

**Lựa chọn:**

<label for="q285-a"><input type="radio" id="q285-a" name="q285" value="A"> <strong>A.</strong> An email will be sent to the System Administrator asking for manual intervention</label><br>
<label for="q285-b"><input type="radio" id="q285-b" name="q285" value="B"> <strong>B.</strong> The CNAME record will be updated to point to the standby database</label><br>
<label for="q285-c"><input type="radio" id="q285-c" name="q285" value="C"> <strong>C.</strong> The URL to access the database will change to the standby database</label><br>
<label for="q285-d"><input type="radio" id="q285-d" name="q285" value="D"> <strong>D.</strong> The application will be down until the primary database has recovered itself</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. The CNAME record will be updated to point to the standby database

</details>

---

## Câu 286

**Chủ đề:** Design Resilient Architectures

A logistics company runs a two-step job handling process on AWS. The first step quickly receives job submissions from clients, while the second step requires longer processing time to complete each job. Currently, both steps run on separate Amazon EC2 Auto Scaling groups. However, during high-demand hours, the job processing stage falls behind, and there is concern that jobs may be lost due to instance termination during scaling events. A solutions architect needs to design a more scalable and reliable architecture that preserves job data and accommodates fluctuating demand in both stages.

Which solution will meet these requirements?

**Lựa chọn:**

<label for="q286-a"><input type="radio" id="q286-a" name="q286" value="A"> <strong>A.</strong> Set up a single Amazon SQS queue for both the job intake and job processing stages. Assign the SQS queue to collect incoming jobs as well as processing jobs. Configure all EC2 instances to poll this queue. Scale the Auto Scaling groups based on number of messages in the queue</label><br>
<label for="q286-b"><input type="radio" id="q286-b" name="q286" value="B"> <strong>B.</strong> Configure each Auto Scaling group to maintain its maximum expected size during peak hours by setting a fixed minimum capacity. Monitor CPUUtilization through Amazon CloudWatch to ensure consistent scaling behavior</label><br>
<label for="q286-c"><input type="radio" id="q286-c" name="q286" value="C"> <strong>C.</strong> Set up two Amazon SQS queues to decouple the job intake and job processing stages respectively. Assign one SQS queue to collect incoming jobs, and another to queue them for processing. Configure the EC2 instances to poll the relevant queue. Scale the Auto Scaling groups based on notifications from each queue</label><br>
<label for="q286-d"><input type="radio" id="q286-d" name="q286" value="D"> <strong>D.</strong> Set up two Amazon SQS queues to decouple the job intake and job processing stages respectively. Assign one SQS queue to collect incoming jobs, and another to queue them for processing. Configure the EC2 instances to poll the relevant queue. Scale the Auto Scaling groups based on number of messages in each queue</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up two Amazon SQS queues to decouple the job intake and job processing stages respectively. Assign one SQS queue to collect incoming jobs, and another to queue them for processing. Configure the EC2 instances to poll the relevant queue. Scale the Auto Scaling groups based on number of messages in each queue

</details>

---

## Câu 287

**Chủ đề:** Design High-Performing Architectures

A mobile-based e-learning platform is migrating its backend storage layer to Amazon DynamoDB to support a rapidly increasing number of student users and learning transactions. The platform must ensure seamless availability and minimal disruption for a global user base. The DynamoDB design must provide low-latency performance, high availability, and automatic fault tolerance across geographies with the lowest possible operational overhead and cost.

Which solution will fulfill these needs in the most cost-efficient manner?

**Lựa chọn:**

<label for="q287-a"><input type="radio" id="q287-a" name="q287" value="A"> <strong>A.</strong> Use DynamoDB global tables for automatic multi-Region replication. Enable provisioned capacity mode with auto scaling to optimize cost and ensure consistent availability</label><br>
<label for="q287-b"><input type="radio" id="q287-b" name="q287" value="B"> <strong>B.</strong> Enable DynamoDB Accelerator (DAX) to reduce response time for read operations. Deploy DAX in one Region, and use scheduled Lambda functions to replicate data to other Regions</label><br>
<label for="q287-c"><input type="radio" id="q287-c" name="q287" value="C"> <strong>C.</strong> Deploy separate DynamoDB tables in each required AWS Region using on-demand capacity mode. Implement a custom cross-Region replication mechanism by streaming data changes with DynamoDB Streams and processing them through AWS Lambda functions</label><br>
<label for="q287-d"><input type="radio" id="q287-d" name="q287" value="D"> <strong>D.</strong> Create separate DynamoDB tables in multiple Regions. Use AWS Data Pipeline to synchronize data periodically between Regions to maintain availability</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use DynamoDB global tables for automatic multi-Region replication. Enable provisioned capacity mode with auto scaling to optimize cost and ensure consistent availability

</details>

---

## Câu 288

**Chủ đề:** Design Cost-Optimized Architectures

A digital content production company has transitioned all of its media assets to Amazon S3 in an effort to reduce storage costs. However, the rendering engine used in production continues to run in an on-premises data center and requires frequent and low-latency access to large media files. The company wants to implement a storage solution that maintains application performance while keeping costs low.

Which approach should the company choose to meet these requirements in the most cost-effective way?

**Lựa chọn:**

<label for="q288-a"><input type="radio" id="q288-a" name="q288" value="A"> <strong>A.</strong> Use Mountpoint for Amazon S3 on the on-premises rendering servers to facilitate low-latency access to the S3 bucket</label><br>
<label for="q288-b"><input type="radio" id="q288-b" name="q288" value="B"> <strong>B.</strong> Set up an Amazon S3 File Gateway to provide storage for the on-premises application</label><br>
<label for="q288-c"><input type="radio" id="q288-c" name="q288" value="C"> <strong>C.</strong> Set up a dedicated on-premises storage array that periodically fetches data from Amazon S3 using a custom-built application. Mount this storage volume on the rendering servers as their primary working directory</label><br>
<label for="q288-d"><input type="radio" id="q288-d" name="q288" value="D"> <strong>D.</strong> Deploy an Amazon FSx for Lustre file system and sync media data from Amazon S3 into it using DataSync. Mount the FSx file system on the on-premises render servers using a VPN tunnel</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up an Amazon S3 File Gateway to provide storage for the on-premises application

</details>

---

## Câu 289

**Chủ đề:** Design Secure Architectures

An e-commerce company uses a two-tier architecture with application servers in the public subnet and an Amazon RDS MySQL DB in a private subnet. The development team can use a bastion host in the public subnet to access the MySQL database and run queries from the bastion host. However, end-users are reporting application errors. Upon inspecting application logs, the team notices several "could not connect to server: connection timed out" error messages.

Which of the following options represent the root cause for this issue?

**Lựa chọn:**

<label for="q289-a"><input type="radio" id="q289-a" name="q289" value="A"> <strong>A.</strong> The security group configuration for the database instance does not have the correct rules to allow inbound connections from the application servers</label><br>
<label for="q289-b"><input type="radio" id="q289-b" name="q289" value="B"> <strong>B.</strong> The database user credentials (username and password) configured for the application are incorrect</label><br>
<label for="q289-c"><input type="radio" id="q289-c" name="q289" value="C"> <strong>C.</strong> The security group configuration for the application servers does not have the correct rules to allow inbound connections from the database instance</label><br>
<label for="q289-d"><input type="radio" id="q289-d" name="q289" value="D"> <strong>D.</strong> The database user credentials (username and password) configured for the application do not have the required privilege for the given database</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The security group configuration for the database instance does not have the correct rules to allow inbound connections from the application servers

</details>

---

## Câu 290

**Chủ đề:** Design Cost-Optimized Architectures

A multinational logistics company operates its shipment tracking platform from Amazon EC2 instances deployed in the AWS us-west-2 Region. The platform exposes a set of APIs over HTTPS, which are used by logistics partners and customers around the world to retrieve real-time tracking data. The company has observed that users from Europe and Asia experience latency issues and inconsistent API response times when accessing the service. As a cloud architect, you have been tasked to propose the most cost-effective solution to improve performance for these international users without migrating the application.

Which solution should you recommend?

**Lựa chọn:**

<label for="q290-a"><input type="radio" id="q290-a" name="q290" value="A"> <strong>A.</strong> Deploy an Amazon CloudFront distribution in front of the API endpoint and apply the CachingOptimized managed policy to enhance caching behavior and improve content delivery efficiency</label><br>
<label for="q290-b"><input type="radio" id="q290-b" name="q290" value="B"> <strong>B.</strong> Configure AWS Global Accelerator in front of the existing HTTPS API, create one endpoint group in us-west-2 for the current application endpoint, and use the accelerator’s global edge network to improve performance for users connecting from Europe and Asia</label><br>
<label for="q290-c"><input type="radio" id="q290-c" name="q290" value="C"> <strong>C.</strong> Deploy Amazon API Gateway in multiple AWS Regions and synchronize the API definitions. Use AWS Lambda as a proxy to forward requests to the EC2-hosted API in us-west-2</label><br>
<label for="q290-d"><input type="radio" id="q290-d" name="q290" value="D"> <strong>D.</strong> Use Amazon Route 53 latency-based routing to direct user requests to a copy of the EC2 API deployed in each major geographic Region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Configure AWS Global Accelerator in front of the existing HTTPS API, create one endpoint group in us-west-2 for the current application endpoint, and use the accelerator’s global edge network to improve performance for users connecting from Europe and Asia

</details>

---

## Câu 291

**Chủ đề:** Design High-Performing Architectures

A DevOps team is tasked with enabling secure and temporary SSH access to Amazon EC2 instances for developers during deployments. The team wants to avoid distributing long-term SSH key pairs and instead prefers ephemeral access that can be audited and revoked immediately after the session ends. The team wants direct access via the AWS Management Console.

What do you recommend?

**Lựa chọn:**

<label for="q291-a"><input type="radio" id="q291-a" name="q291" value="A"> <strong>A.</strong> Use EC2 Instance Connect to inject a temporary public key and establish SSH access using the instance’s public IP address</label><br>
<label for="q291-b"><input type="radio" id="q291-b" name="q291" value="B"> <strong>B.</strong> Use EC2 Instance Connect to inject a static SSH key and connect via the instance's private IP address directly from the internet</label><br>
<label for="q291-c"><input type="radio" id="q291-c" name="q291" value="C"> <strong>C.</strong> Use EC2 Instance Connect with Systems Manager Agent disabled, and connect via private IP using an internal proxy endpoint</label><br>
<label for="q291-d"><input type="radio" id="q291-d" name="q291" value="D"> <strong>D.</strong> Use an EC2 Instance Connect Endpoint to reach the instances even though they already have public IP addresses, because Instance Connect requires an endpoint for all SSH sessions</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use EC2 Instance Connect to inject a temporary public key and establish SSH access using the instance’s public IP address

</details>

---

## Câu 292

**Chủ đề:** Design High-Performing Architectures

A streaming service provider collects user experience feedback through embedded feedback forms in their mobile and web apps. Feedback submissions frequently spike to thousands per hour during content launches or service outages. Currently, the feedback is sent via email to the operations team for manual review. The company now wants to automate feedback collection and sentiment analysis so that insights can be generated quickly and stored for a full year for trend analysis.

Which solution provides the most scalable and automated approach to meet these requirements?

**Lựa chọn:**

<label for="q292-a"><input type="radio" id="q292-a" name="q292" value="A"> <strong>A.</strong> Design a RESTful API with Amazon API Gateway that forwards incoming feedback data to an Amazon SQS queue. Set up an AWS Lambda function to process the queue messages, analyze sentiment using Amazon Comprehend, and store results in a DynamoDB table with a 365-day TTL configured on each item</label><br>
<label for="q292-b"><input type="radio" id="q292-b" name="q292" value="B"> <strong>B.</strong> Build a web service on Amazon EC2 that receives feedback data and stores each record in a DynamoDB table. Use the EC2 application to invoke Amazon Comprehend for sentiment detection and write results to a second table. Apply a TTL of 365 days to each table</label><br>
<label for="q292-c"><input type="radio" id="q292-c" name="q292" value="C"> <strong>C.</strong> Use Amazon EventBridge to capture feedback events and forward them to an AWS Step Functions workflow. The workflow invokes Lambda functions for validation, calls Amazon Transcribe to convert the text to audio for archival, and stores the results in an Amazon RDS database. Configure a lifecycle policy to remove records after 12 months</label><br>
<label for="q292-d"><input type="radio" id="q292-d" name="q292" value="D"> <strong>D.</strong> Route all feedback submissions through Amazon Kinesis Data Streams. Use an AWS Lambda consumer to batch process incoming records, invoke Amazon Translate to detect language and convert input to English, and save the processed content in an Amazon OpenSearch Service index. Configure OpenSearch Index State Management (ISM) policies to delete documents after 12 months</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Design a RESTful API with Amazon API Gateway that forwards incoming feedback data to an Amazon SQS queue. Set up an AWS Lambda function to process the queue messages, analyze sentiment using Amazon Comprehend, and store results in a DynamoDB table with a 365-day TTL configured on each item

</details>

---

## Câu 293

**Chủ đề:** Design High-Performing Architectures

You have built an application that is deployed with Elastic Load Balancing and an Auto Scaling Group. As a Solutions Architect, you have configured aggressive Amazon CloudWatch alarms, making your Auto Scaling Group (ASG) scale in and out very quickly, renewing your fleet of Amazon EC2 instances on a daily basis. A production bug appeared two days ago, but the team is unable to SSH into the instance to debug the issue, because the instance has already been terminated by the Auto Scaling Group. The log files are saved on the Amazon EC2 instance.

How will you resolve the issue and make sure it doesn't happen again?

**Lựa chọn:**

<label for="q293-a"><input type="radio" id="q293-a" name="q293" value="A"> <strong>A.</strong> Install an Amazon CloudWatch Logs agents on the Amazon EC2 instances to send logs to Amazon CloudWatch</label><br>
<label for="q293-b"><input type="radio" id="q293-b" name="q293" value="B"> <strong>B.</strong> Disable the Termination from the Auto Scaling Group any time a user reports an issue</label><br>
<label for="q293-c"><input type="radio" id="q293-c" name="q293" value="C"> <strong>C.</strong> Make a snapshot of the Amazon EC2 instance just before it gets terminated</label><br>
<label for="q293-d"><input type="radio" id="q293-d" name="q293" value="D"> <strong>D.</strong> Use AWS Lambda to regularly SSH into the Amazon EC2 instances and copy the log files to Amazon S3</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Install an Amazon CloudWatch Logs agents on the Amazon EC2 instances to send logs to Amazon CloudWatch

</details>

---

## Câu 294

**Chủ đề:** Design Resilient Architectures

A digital media company runs its content rendering service on Amazon EC2 instances that are registered with an Application Load Balancer (ALB) using IP-based target groups. The company relies on AWS Systems Manager to manage and patch these instances regularly. According to new compliance requirements, EC2 instances must be safely removed from production traffic during patching to prevent user disruption and maintain application integrity. However, during the most recent patch cycle, the operations team noticed application failures and API timeouts, even though patching succeeded on the instances. You are asked to suggest a reliable and scalable way to ensure safe patching while preserving service availability.

Which solution will best meet the new compliance and operational requirements? (Select two)

**Lựa chọn:**

<label for="q294-a"><input type="checkbox" id="q294-a" name="q294" value="A"> <strong>A.</strong> Configure a custom Lambda function triggered by an Amazon EventBridge rule that disables the EC2 instance's network interface during the patching window and re-enables it after patching completes</label><br>
<label for="q294-b"><input type="checkbox" id="q294-b" name="q294" value="B"> <strong>B.</strong> Modify the load balancer configuration to attach EC2 instances using instance ID-based target groups instead of IP-based targets, allowing Systems Manager to directly communicate with instance metadata</label><br>
<label for="q294-c"><input type="checkbox" id="q294-c" name="q294" value="C"> <strong>C.</strong> Use AWS Systems Manager Automation with the AWSEC2-PatchLoadBalancerInstance document to manage patching</label><br>
<label for="q294-d"><input type="checkbox" id="q294-d" name="q294" value="D"> <strong>D.</strong> Use Amazon CloudWatch Logs Insights to monitor patching success and then manually adjust ALB target group registrations before and after each patch window</label><br>
<label for="q294-e"><input type="checkbox" id="q294-e" name="q294" value="E"> <strong>E.</strong> Configure Systems Manager Maintenance Windows to coordinate patching and instance removal from the ALB during the defined window</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use AWS Systems Manager Automation with the AWSEC2-PatchLoadBalancerInstance document to manage patching

E. Configure Systems Manager Maintenance Windows to coordinate patching and instance removal from the ALB during the defined window

</details>

---

## Câu 295

**Chủ đề:** Design High-Performing Architectures

A financial services company runs its flagship web application on AWS. The application serves thousands of users during peak hours. The company needs a scalable near-real-time solution to share hundreds of thousands of financial transactions with multiple internal applications. The solution should also remove sensitive details from the transactions before storing the cleansed transactions in a document database for low-latency retrieval.

As an AWS Certified Solutions Architect Associate, which of the following would you recommend?

**Lựa chọn:**

<label for="q295-a"><input type="radio" id="q295-a" name="q295" value="A"> <strong>A.</strong> Batch process the raw transactions data into Amazon S3 flat files. Use S3 events to trigger an AWS Lambda function to remove sensitive data from the raw transactions in the flat file and then store the cleansed transactions in Amazon DynamoDB. Leverage DynamoDB Streams to share the transactions data with the internal applications</label><br>
<label for="q295-b"><input type="radio" id="q295-b" name="q295" value="B"> <strong>B.</strong> Feed the streaming transactions into Amazon Kinesis Data Streams. Leverage AWS Lambda integration to remove sensitive data from every transaction and then store the cleansed transactions in Amazon DynamoDB. The internal applications can consume the raw transactions off the Amazon Kinesis Data Stream</label><br>
<label for="q295-c"><input type="radio" id="q295-c" name="q295" value="C"> <strong>C.</strong> Feed the streaming transactions into Amazon Kinesis Data Firehose. Leverage AWS Lambda integration to remove sensitive data from every transaction and then store the cleansed transactions in Amazon DynamoDB. The internal applications can consume the raw transactions off the Amazon Kinesis Data Firehose</label><br>
<label for="q295-d"><input type="radio" id="q295-d" name="q295" value="D"> <strong>D.</strong> Persist the raw transactions into Amazon DynamoDB. Configure a rule in Amazon DynamoDB to update the transaction by removing sensitive data whenever any new raw transaction is written. Leverage Amazon DynamoDB Streams to share the transactions data with the internal applications</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Feed the streaming transactions into Amazon Kinesis Data Streams. Leverage AWS Lambda integration to remove sensitive data from every transaction and then store the cleansed transactions in Amazon DynamoDB. The internal applications can consume the raw transactions off the Amazon Kinesis Data Stream

</details>

---

## Câu 296

**Chủ đề:** Design Resilient Architectures

A healthcare startup runs a lightweight reporting application on a single Amazon EC2 On-Demand instance. The application is designed to be stateless, fault-tolerant, and optimized for fast rendering of analytics dashboards. During major health events or news cycles, the team observes latency issues and occasional 5xx errors due to traffic spikes. To meet growing demand without over-provisioning resources during off-peak hours, the company wants to implement a cost-effective, scalable solution that ensures consistent performance even under unpredictable load.

Which approach best meets the requirements while minimizing costs?

**Lựa chọn:**

<label for="q296-a"><input type="radio" id="q296-a" name="q296" value="A"> <strong>A.</strong> Clone the EC2 instance using an AMI and launch a second On-Demand instance. Register both instances with an Application Load Balancer to distribute incoming traffic evenly</label><br>
<label for="q296-b"><input type="radio" id="q296-b" name="q296" value="B"> <strong>B.</strong> Configure an Amazon EventBridge rule to monitor system-level metrics from the EC2 instance. Trigger a Lambda function to re-deploy the application in a different Availability Zone when CPU utilization exceeds 70%</label><br>
<label for="q296-c"><input type="radio" id="q296-c" name="q296" value="C"> <strong>C.</strong> Build an Amazon Machine Image (AMI) from the existing EC2 instance and configure a launch template. Create an Auto Scaling group using the launch template with Spot Instance pricing enabled. Attach an Application Load Balancer to distribute traffic across dynamically launched instances</label><br>
<label for="q296-d"><input type="radio" id="q296-d" name="q296" value="D"> <strong>D.</strong> Containerize the application using Amazon ECS with Fargate launch type. Deploy the container to a single Fargate task and set a CloudWatch alarm to increase memory and CPU allocation dynamically based on load</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Build an Amazon Machine Image (AMI) from the existing EC2 instance and configure a launch template. Create an Auto Scaling group using the launch template with Spot Instance pricing enabled. Attach an Application Load Balancer to distribute traffic across dynamically launched instances

</details>

---

## Câu 297

**Chủ đề:** Design High-Performing Architectures

A Customer relationship management (CRM) application is facing user experience issues with users reporting frequent sign-in requests from the application. The application is currently hosted on multiple Amazon EC2 instances behind an Application Load Balancer. The engineering team has identified the root cause as unhealthy servers causing session data to be lost. The team would like to implement a distributed in-memory cache-based session management solution.

As a solutions architect, which of the following solutions would you recommend?

**Lựa chọn:**

<label for="q297-a"><input type="radio" id="q297-a" name="q297" value="A"> <strong>A.</strong> Use Amazon RDS for distributed in-memory cache based session management</label><br>
<label for="q297-b"><input type="radio" id="q297-b" name="q297" value="B"> <strong>B.</strong> Use Amazon Elasticache for distributed in-memory cache based session management</label><br>
<label for="q297-c"><input type="radio" id="q297-c" name="q297" value="C"> <strong>C.</strong> Use Application Load Balancer sticky sessions</label><br>
<label for="q297-d"><input type="radio" id="q297-d" name="q297" value="D"> <strong>D.</strong> Use Amazon DynamoDB for distributed in-memory cache based session management</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon Elasticache for distributed in-memory cache based session management

</details>

---

## Câu 298

**Chủ đề:** Design High-Performing Architectures

A big data analytics company is using Amazon Kinesis Data Streams (KDS) to process IoT data from the field devices of an agricultural sciences company. Multiple consumer applications are using the incoming data streams and the engineers have noticed a performance lag for the data delivery speed between producers and consumers of the data streams.

As a solutions architect, which of the following would you recommend for improving the performance for the given use-case?

**Lựa chọn:**

<label for="q298-a"><input type="radio" id="q298-a" name="q298" value="A"> <strong>A.</strong> Swap out Amazon Kinesis Data Streams with Amazon SQS Standard queues</label><br>
<label for="q298-b"><input type="radio" id="q298-b" name="q298" value="B"> <strong>B.</strong> Swap out Amazon Kinesis Data Streams with Amazon SQS FIFO queues</label><br>
<label for="q298-c"><input type="radio" id="q298-c" name="q298" value="C"> <strong>C.</strong> Use Enhanced Fanout feature of Amazon Kinesis Data Streams</label><br>
<label for="q298-d"><input type="radio" id="q298-d" name="q298" value="D"> <strong>D.</strong> Swap out Amazon Kinesis Data Streams with Amazon Kinesis Data Firehose</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Enhanced Fanout feature of Amazon Kinesis Data Streams

</details>

---

## Câu 299

**Chủ đề:** Design Secure Architectures

A silicon valley based healthcare startup uses AWS Cloud for its IT infrastructure. The startup stores patient health records on Amazon Simple Storage Service (Amazon S3). The engineering team needs to implement an archival solution based on Amazon S3 Glacier to enforce regulatory and compliance controls on data access.

As a solutions architect, which of the following solutions would you recommend?

**Lựa chọn:**

<label for="q299-a"><input type="radio" id="q299-a" name="q299" value="A"> <strong>A.</strong> Use Amazon S3 Glacier vault to store the sensitive archived data and then use a vault lock policy to enforce compliance controls</label><br>
<label for="q299-b"><input type="radio" id="q299-b" name="q299" value="B"> <strong>B.</strong> Use Amazon S3 Glacier to store the sensitive archived data and then use an Amazon S3 lifecycle policy to enforce compliance controls</label><br>
<label for="q299-c"><input type="radio" id="q299-c" name="q299" value="C"> <strong>C.</strong> Use Amazon S3 Glacier vault to store the sensitive archived data and then use an Amazon S3 Access Control List to enforce compliance controls</label><br>
<label for="q299-d"><input type="radio" id="q299-d" name="q299" value="D"> <strong>D.</strong> Use Amazon S3 Glacier to store the sensitive archived data and then use an Amazon S3 Access Control List to enforce compliance controls</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon S3 Glacier vault to store the sensitive archived data and then use a vault lock policy to enforce compliance controls

</details>

---

## Câu 300

**Chủ đề:** Design Secure Architectures

A pharmaceutical company is considering moving to AWS Cloud to accelerate the research and development process. Most of the daily workflows would be centered around running batch jobs on Amazon EC2 instances with storage on Amazon Elastic Block Store (Amazon EBS) volumes. The CTO is concerned about meeting HIPAA compliance norms for sensitive data stored on Amazon EBS.

Which of the following options outline the correct capabilities of an encrypted Amazon EBS volume? (Select three)

**Lựa chọn:**

<label for="q300-a"><input type="checkbox" id="q300-a" name="q300" value="A"> <strong>A.</strong> Data at rest inside the volume is encrypted</label><br>
<label for="q300-b"><input type="checkbox" id="q300-b" name="q300" value="B"> <strong>B.</strong> Data moving between the volume and the instance is NOT encrypted</label><br>
<label for="q300-c"><input type="checkbox" id="q300-c" name="q300" value="C"> <strong>C.</strong> Any snapshot created from the volume is encrypted</label><br>
<label for="q300-d"><input type="checkbox" id="q300-d" name="q300" value="D"> <strong>D.</strong> Any snapshot created from the volume is NOT encrypted</label><br>
<label for="q300-e"><input type="checkbox" id="q300-e" name="q300" value="E"> <strong>E.</strong> Data moving between the volume and the instance is encrypted</label><br>
<label for="q300-f"><input type="checkbox" id="q300-f" name="q300" value="F"> <strong>F.</strong> Data at rest inside the volume is NOT encrypted</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Data at rest inside the volume is encrypted

C. Any snapshot created from the volume is encrypted

E. Data moving between the volume and the instance is encrypted

</details>

---

## Câu 301

**Chủ đề:** Design Secure Architectures

A retail company wants to establish encrypted network connectivity between its on-premises data center and AWS Cloud. The company wants to get the solution up and running in the fastest possible time and it should also support encryption in transit.

As a solutions architect, which of the following solutions would you suggest to the company?

**Lựa chọn:**

<label for="q301-a"><input type="radio" id="q301-a" name="q301" value="A"> <strong>A.</strong> Use AWS Direct Connect to establish encrypted network connectivity between the on-premises data center and AWS Cloud</label><br>
<label for="q301-b"><input type="radio" id="q301-b" name="q301" value="B"> <strong>B.</strong> Use AWS Data Sync to establish encrypted network connectivity between the on-premises data center and AWS Cloud</label><br>
<label for="q301-c"><input type="radio" id="q301-c" name="q301" value="C"> <strong>C.</strong> Use AWS Secrets Manager to establish encrypted network connectivity between the on-premises data center and AWS Cloud</label><br>
<label for="q301-d"><input type="radio" id="q301-d" name="q301" value="D"> <strong>D.</strong> Use AWS Site-to-Site VPN to establish encrypted network connectivity between the on-premises data center and AWS Cloud</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS Site-to-Site VPN to establish encrypted network connectivity between the on-premises data center and AWS Cloud

</details>

---

## Câu 302

**Chủ đề:** Design Resilient Architectures

The engineering team at a retail company manages 3 Amazon EC2 instances that make read-heavy database requests to the Amazon RDS for the PostgreSQL database instance. As an AWS Certified Solutions Architect - Associate, you have been tasked to make the database instance resilient from a disaster recovery perspective.

Which of the following features will help you in disaster recovery of the database? (Select two)

**Lựa chọn:**

<label for="q302-a"><input type="checkbox" id="q302-a" name="q302" value="A"> <strong>A.</strong> Use cross-Region Read Replicas</label><br>
<label for="q302-b"><input type="checkbox" id="q302-b" name="q302" value="B"> <strong>B.</strong> Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups across multiple Regions</label><br>
<label for="q302-c"><input type="checkbox" id="q302-c" name="q302" value="C"> <strong>C.</strong> Use Amazon RDS Provisioned IOPS (SSD) Storage in place of General Purpose (SSD) Storage</label><br>
<label for="q302-d"><input type="checkbox" id="q302-d" name="q302" value="D"> <strong>D.</strong> Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups in a single AWS Region</label><br>
<label for="q302-e"><input type="checkbox" id="q302-e" name="q302" value="E"> <strong>E.</strong> Use the database cloning feature of the Amazon RDS Database cluster</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use cross-Region Read Replicas

B. Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups across multiple Regions

</details>

---

## Câu 303

**Chủ đề:** Design Cost-Optimized Architectures

Computer vision researchers at a university are trying to optimize the I/O bound processes for a proprietary algorithm running on Amazon EC2 instances. The ideal storage would facilitate high-performance IOPS when doing file processing in a temporary storage space before uploading the results back into Amazon S3.

As a solutions architect, which of the following AWS storage options would you recommend as the MOST performant as well as cost-optimal?

**Lựa chọn:**

<label for="q303-a"><input type="radio" id="q303-a" name="q303" value="A"> <strong>A.</strong> Use Amazon EC2 instances with Instance Store as the storage option</label><br>
<label for="q303-b"><input type="radio" id="q303-b" name="q303" value="B"> <strong>B.</strong> Use Amazon EC2 instances with Amazon EBS General Purpose SSD (gp2) as the storage option</label><br>
<label for="q303-c"><input type="radio" id="q303-c" name="q303" value="C"> <strong>C.</strong> Use Amazon EC2 instances with Amazon EBS Provisioned IOPS SSD (io1) as the storage option</label><br>
<label for="q303-d"><input type="radio" id="q303-d" name="q303" value="D"> <strong>D.</strong> Use Amazon EC2 instances with Amazon EBS Throughput Optimized HDD (st1) as the storage option</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon EC2 instances with Instance Store as the storage option

</details>

---

## Câu 304

**Chủ đề:** Design Resilient Architectures

An e-commerce company uses Amazon Simple Queue Service (Amazon SQS) queues to decouple their application architecture. The engineering team has observed message processing failures for some customer orders.

As a solutions architect, which of the following solutions would you recommend for handling such message failures?

**Lựa chọn:**

<label for="q304-a"><input type="radio" id="q304-a" name="q304" value="A"> <strong>A.</strong> Use a temporary queue to handle message processing failures</label><br>
<label for="q304-b"><input type="radio" id="q304-b" name="q304" value="B"> <strong>B.</strong> Use a dead-letter queue to handle message processing failures</label><br>
<label for="q304-c"><input type="radio" id="q304-c" name="q304" value="C"> <strong>C.</strong> Use short polling to handle message processing failures</label><br>
<label for="q304-d"><input type="radio" id="q304-d" name="q304" value="D"> <strong>D.</strong> Use long polling to handle message processing failures</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use a dead-letter queue to handle message processing failures

</details>

---

## Câu 305

**Chủ đề:** Design Secure Architectures

An online gaming company wants to block access to its application from specific countries; however, the company wants to allow its remote development team (from one of the blocked countries) to have access to the application. The application is deployed on Amazon EC2 instances running under an Application Load Balancer with AWS Web Application Firewall (AWS WAF).

As a solutions architect, which of the following solutions can be combined to address the given use-case? (Select two)

**Lựa chọn:**

<label for="q305-a"><input type="checkbox" id="q305-a" name="q305" value="A"> <strong>A.</strong> Create a deny rule for the blocked countries in the network access control list (network ACL) associated with each of the Amazon EC2 instances</label><br>
<label for="q305-b"><input type="checkbox" id="q305-b" name="q305" value="B"> <strong>B.</strong> Use Application Load Balancer geo match statement listing the countries that you want to block</label><br>
<label for="q305-c"><input type="checkbox" id="q305-c" name="q305" value="C"> <strong>C.</strong> Use Application Load Balancer IP set statement that specifies the IP addresses that you want to allow through</label><br>
<label for="q305-d"><input type="checkbox" id="q305-d" name="q305" value="D"> <strong>D.</strong> Use AWS WAF geo match statement listing the countries that you want to block</label><br>
<label for="q305-e"><input type="checkbox" id="q305-e" name="q305" value="E"> <strong>E.</strong> Use AWS WAF IP set statement that specifies the IP addresses that you want to allow through</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS WAF geo match statement listing the countries that you want to block

E. Use AWS WAF IP set statement that specifies the IP addresses that you want to allow through

</details>

---

## Câu 306

**Chủ đề:** Design Secure Architectures

A digital publishing platform stores large volumes of media assets (such as images and documents) in an Amazon S3 bucket. These assets are accessed frequently during business hours by internal editors and content delivery tools. The company has strict encryption policies and currently uses AWS KMS to handle server-side encryption. The cloud operations team notices that AWS KMS request costs are increasing significantly due to the high frequency of object uploads and accesses. The team is now looking for a way to maintain the same encryption method but reduce the cost of KMS usage, especially for frequent access patterns.

Which solution meets the company's encryption and cost optimization goals?

**Lựa chọn:**

<label for="q306-a"><input type="radio" id="q306-a" name="q306" value="A"> <strong>A.</strong> Configure a VPC endpoint for S3 and restrict access to the bucket to traffic originating from the endpoint to avoid additional KMS charges</label><br>
<label for="q306-b"><input type="radio" id="q306-b" name="q306" value="B"> <strong>B.</strong> Use client-side encryption by generating a local symmetric key and uploading it to Amazon S3 along with each object’s metadata for decryption</label><br>
<label for="q306-c"><input type="radio" id="q306-c" name="q306" value="C"> <strong>C.</strong> Switch to server-side encryption using Amazon S3 managed keys (SSE-S3) to eliminate all AWS KMS-related encryption charges while maintaining the same level of encryption control</label><br>
<label for="q306-d"><input type="radio" id="q306-d" name="q306" value="D"> <strong>D.</strong> Enable S3 Bucket Keys for server-side encryption with AWS KMS (SSE-KMS) so that new objects use a bucket-level key rather than requesting individual KMS data keys for every object</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Enable S3 Bucket Keys for server-side encryption with AWS KMS (SSE-KMS) so that new objects use a bucket-level key rather than requesting individual KMS data keys for every object

</details>

---

## Câu 307

**Chủ đề:** Design Resilient Architectures

A SaaS analytics company is deploying a microservices-based application on Amazon ECS using the Fargate launch type. The application requires access to a shared, POSIX-compliant file system that is available across multiple Availability Zones for redundancy and availability. To meet compliance requirements, the system must support regional backups and cross-Region data recovery with a recovery point objective (RPO) of no more than 8 hours. A backup strategy will be implemented using AWS Backup to automate replication across Regions. As the lead cloud architect, you are evaluating file storage solutions that align with these requirements.

Which option best meets the application’s availability, durability, and RPO objectives?

**Lựa chọn:**

<label for="q307-a"><input type="radio" id="q307-a" name="q307" value="A"> <strong>A.</strong> Deploy Amazon FSx for Lustre and configure a backup plan using AWS Backup for cross-Region replication of the file system metadata</label><br>
<label for="q307-b"><input type="radio" id="q307-b" name="q307" value="B"> <strong>B.</strong> Use Amazon Elastic File System (Amazon EFS) with the Standard storage class and configure AWS Backup to create cross-Region backups on a scheduled basis</label><br>
<label for="q307-c"><input type="radio" id="q307-c" name="q307" value="C"> <strong>C.</strong> Configure Amazon S3 with the S3 Standard storage class and mount it in containers using Mountpoint for Amazon S3. Use AWS Backup to replicate objects to another Region</label><br>
<label for="q307-d"><input type="radio" id="q307-d" name="q307" value="D"> <strong>D.</strong> Use Amazon FSx for NetApp ONTAP with a Multi-AZ deployment and rely on its native high availability and AWS Backup integration to replicate the file system to another Region automatically</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon Elastic File System (Amazon EFS) with the Standard storage class and configure AWS Backup to create cross-Region backups on a scheduled basis

</details>

---

## Câu 308

**Chủ đề:** Design High-Performing Architectures

A leading media company wants to do an accelerated online migration of hundreds of terabytes of files from their on-premises data center to Amazon S3 and then establish a mechanism to access the migrated data for ongoing updates from the on-premises applications.

As a solutions architect, which of the following would you select as the MOST performant solution for the given use-case?

**Lựa chọn:**

<label for="q308-a"><input type="radio" id="q308-a" name="q308" value="A"> <strong>A.</strong> Use AWS DataSync to migrate existing data to Amazon  S3 as well as access the Amazon S3 data for ongoing updates</label><br>
<label for="q308-b"><input type="radio" id="q308-b" name="q308" value="B"> <strong>B.</strong> Use File Gateway configuration of AWS Storage Gateway to migrate data to Amazon S3 and then use Amazon S3 Transfer Acceleration (Amazon S3TA) for ongoing updates from the on-premises applications</label><br>
<label for="q308-c"><input type="radio" id="q308-c" name="q308" value="C"> <strong>C.</strong> Use Amazon S3 Transfer Acceleration (Amazon S3TA) to migrate existing data to Amazon S3 and then use AWS DataSync for ongoing updates from the on-premises applications</label><br>
<label for="q308-d"><input type="radio" id="q308-d" name="q308" value="D"> <strong>D.</strong> Use AWS DataSync to migrate existing data to Amazon S3 and then use File Gateway to retain access to the migrated data for ongoing updates from the on-premises applications</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use AWS DataSync to migrate existing data to Amazon S3 and then use File Gateway to retain access to the migrated data for ongoing updates from the on-premises applications

</details>

---

## Câu 309

**Chủ đề:** Design Cost-Optimized Architectures

A medical devices company uses Amazon S3 buckets to store critical data. Hundreds of buckets are used to keep the data segregated and well organized. Recently, the development team noticed that the lifecycle policies on the Amazon S3 buckets have not been applied optimally, resulting in higher costs.

As a Solutions Architect, can you recommend a solution to reduce storage costs on Amazon S3 while keeping the IT team's involvement to a minimum?

**Lựa chọn:**

<label for="q309-a"><input type="radio" id="q309-a" name="q309" value="A"> <strong>A.</strong> Configure Amazon EFS to provide a fast, cost-effective and sharable storage service</label><br>
<label for="q309-b"><input type="radio" id="q309-b" name="q309" value="B"> <strong>B.</strong> Use Amazon S3 Intelligent-Tiering storage class to optimize the Amazon S3 storage costs</label><br>
<label for="q309-c"><input type="radio" id="q309-c" name="q309" value="C"> <strong>C.</strong> Use Amazon S3 One Zone-Infrequent Access, to reduce the costs on Amazon S3 storage</label><br>
<label for="q309-d"><input type="radio" id="q309-d" name="q309" value="D"> <strong>D.</strong> Use Amazon S3 Outposts storage class to reduce the costs on Amazon S3 storage by storing the data on-premises</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon S3 Intelligent-Tiering storage class to optimize the Amazon S3 storage costs

</details>

---

## Câu 310

**Chủ đề:** Design Secure Architectures

A financial auditing firm uses Amazon S3 to store sensitive client records that are subject to write-once-read-many (WORM) regulations to prevent alteration or deletion of records for a specific retention period. The firm wants to enforce immutable storage, such that even administrators cannot overwrite or delete the records during the lock duration. They also need audit-friendly enforcement to prevent accidental or malicious deletion.

Which configuration of S3 Object Lock will ensure that the retention policy is strictly enforced, and no user (including root or administrators) can override or delete protected objects during the lock period?

**Lựa chọn:**

<label for="q310-a"><input type="radio" id="q310-a" name="q310" value="A"> <strong>A.</strong> Use S3 Object Lock in Governance Mode, which allows only IAM users with elevated permissions to override or remove retention settings</label><br>
<label for="q310-b"><input type="radio" id="q310-b" name="q310" value="B"> <strong>B.</strong> Enable S3 Versioning and set a bucket policy that denies s3:DeleteObject to all users during the retention period</label><br>
<label for="q310-c"><input type="radio" id="q310-c" name="q310" value="C"> <strong>C.</strong> Use S3 Lifecycle Policies to transition data to Glacier Deep Archive and treat it as immutable during the archival period</label><br>
<label for="q310-d"><input type="radio" id="q310-d" name="q310" value="D"> <strong>D.</strong> Use S3 Object Lock in Compliance Mode, which enforces retention policies strictly and prevents all users from modifying or deleting data during the retention period</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use S3 Object Lock in Compliance Mode, which enforces retention policies strictly and prevents all users from modifying or deleting data during the retention period

</details>

---

## Câu 311

**Chủ đề:** Design Cost-Optimized Architectures

The content division at a digital media agency has an application that generates a large number of files on Amazon S3, each approximately 10 megabytes in size. The agency mandates that the files be stored for 5 years before they can be deleted. The files are frequently accessed in the first 30 days of the object creation but are rarely accessed after the first 30 days. The files contain critical business data that is not easy to reproduce, therefore, immediate accessibility is always required.

Which solution is the MOST cost-effective for the given use case?

**Lựa chọn:**

<label for="q311-a"><input type="radio" id="q311-a" name="q311" value="A"> <strong>A.</strong> Set up an Amazon S3 bucket lifecycle policy to move files from Amazon S3 Standard to Amazon S3 Glacier Flexible Retrieval 30 days after object creation. Delete the files 5 years after object creation</label><br>
<label for="q311-b"><input type="radio" id="q311-b" name="q311" value="B"> <strong>B.</strong> Set up an Amazon S3 bucket lifecycle policy to move files from Amazon S3 Standard to Amazon S3 Standard-IA 30 days after object creation. Archive the files to Amazon S3 Glacier Deep Archive 5 years after object creation</label><br>
<label for="q311-c"><input type="radio" id="q311-c" name="q311" value="C"> <strong>C.</strong> Set up an Amazon S3 bucket lifecycle policy to move files from Amazon S3 Standard to Amazon S3 One Zone-IA 30 days after object creation. Delete the files 5 years after object creation</label><br>
<label for="q311-d"><input type="radio" id="q311-d" name="q311" value="D"> <strong>D.</strong> Set up an Amazon S3 bucket lifecycle policy to move files from Amazon S3 Standard to Amazon S3 Standard-IA 30 days after object creation. Delete the files 5 years after object creation</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up an Amazon S3 bucket lifecycle policy to move files from Amazon S3 Standard to Amazon S3 Standard-IA 30 days after object creation. Delete the files 5 years after object creation

</details>

---

## Câu 312

**Chủ đề:** Design High-Performing Architectures

A media company is evaluating the possibility of moving its IT infrastructure to the AWS Cloud. The company needs at least 10 terabytes of storage with the maximum possible I/O performance for processing certain files which are mostly large videos. The company also needs close to 450 terabytes of very durable storage for storing media content and almost double of it, i.e. 900 terabytes for archival of legacy data.

As a Solutions Architect, which set of services will you recommend to meet these requirements?

**Lựa chọn:**

<label for="q312-a"><input type="radio" id="q312-a" name="q312" value="A"> <strong>A.</strong> Amazon S3 standard storage for maximum performance, Amazon S3 Intelligent-Tiering for intelligent, durable storage, and Amazon S3 Glacier Deep Archive for archival storage</label><br>
<label for="q312-b"><input type="radio" id="q312-b" name="q312" value="B"> <strong>B.</strong> Amazon EC2 instance store for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage</label><br>
<label for="q312-c"><input type="radio" id="q312-c" name="q312" value="C"> <strong>C.</strong> Amazon EBS for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage</label><br>
<label for="q312-d"><input type="radio" id="q312-d" name="q312" value="D"> <strong>D.</strong> Amazon EC2 instance store for maximum performance, AWS Storage Gateway for on-premises durable data access and Amazon S3 Glacier Deep Archive for archival storage</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Amazon EC2 instance store for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage

</details>

---

## Câu 313

**Chủ đề:** Design High-Performing Architectures

You are a cloud architect at an IT company. The company has multiple enterprise customers that manage their own mobile applications that capture and send data to Amazon Kinesis Data Streams. They have been getting a ProvisionedThroughputExceededException exception. You have been contacted to help and upon analysis, you notice that messages are being sent one by one at a high rate.

Which of the following options will help with the exception while keeping costs at a minimum?

**Lựa chọn:**

<label for="q313-a"><input type="radio" id="q313-a" name="q313" value="A"> <strong>A.</strong> Use batch messages</label><br>
<label for="q313-b"><input type="radio" id="q313-b" name="q313" value="B"> <strong>B.</strong> Decrease the Stream retention duration</label><br>
<label for="q313-c"><input type="radio" id="q313-c" name="q313" value="C"> <strong>C.</strong> Increase the number of shards</label><br>
<label for="q313-d"><input type="radio" id="q313-d" name="q313" value="D"> <strong>D.</strong> Use Exponential Backoff</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use batch messages

</details>

---

## Câu 314

**Chủ đề:** Design Cost-Optimized Architectures

A digital design company has migrated its project archiving platform to AWS. The application runs on Amazon EC2 Linux instances in an Auto Scaling group that spans multiple Availability Zones. Designers upload and retrieve high-resolution image files from a shared file system, which is currently configured to use Amazon EFS Standard-IA. Metadata for these files is stored and indexed in an Amazon RDS for PostgreSQL database. The company's cloud engineering team has been asked to optimize storage costs for the image archive without compromising reliability. They are open to refactoring the application to use managed AWS services when necessary.

Which solution offers the most cost-effective architecture?

**Lựa chọn:**

<label for="q314-a"><input type="radio" id="q314-a" name="q314" value="A"> <strong>A.</strong> Replace the EFS file system with Amazon FSx for Lustre. Mount the file system to EC2 instances and store project files there to reduce access latency and cost</label><br>
<label for="q314-b"><input type="radio" id="q314-b" name="q314" value="B"> <strong>B.</strong> Create an Amazon S3 bucket with Intelligent-Tiering enabled. Update the application to store and retrieve project files using the Amazon S3 API</label><br>
<label for="q314-c"><input type="radio" id="q314-c" name="q314" value="C"> <strong>C.</strong> Use AWS Backup to export all EFS files daily to an Amazon S3 bucket. Retain the EFS file system in Standard-IA class for occasional real-time access and route all archival queries to the S3 export</label><br>
<label for="q314-d"><input type="radio" id="q314-d" name="q314" value="D"> <strong>D.</strong> Replace the EFS file system with Amazon FSx for NetApp ONTAP. Use volume tiering to move cold data to lower-cost capacity pool storage. Update the application to use the ONTAP mount path</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create an Amazon S3 bucket with Intelligent-Tiering enabled. Update the application to store and retrieve project files using the Amazon S3 API

</details>

---

## Câu 315

**Chủ đề:** Design High-Performing Architectures

An application with global users across AWS Regions had suffered an issue when the Elastic Load Balancing (ELB) in a Region malfunctioned thereby taking down the traffic with it. The manual intervention cost the company significant time and resulted in major revenue loss.

What should a solutions architect recommend to reduce internet latency and add automatic failover across AWS Regions?

**Lựa chọn:**

<label for="q315-a"><input type="radio" id="q315-a" name="q315" value="A"> <strong>A.</strong> Set up AWS Direct Connect as the backbone for each of the AWS Regions where the application is deployed</label><br>
<label for="q315-b"><input type="radio" id="q315-b" name="q315" value="B"> <strong>B.</strong> Create Amazon S3 buckets in different AWS Regions and configure Amazon CloudFront to pick the nearest edge location to the user</label><br>
<label for="q315-c"><input type="radio" id="q315-c" name="q315" value="C"> <strong>C.</strong> Set up an Amazon Route 53 geoproximity routing policy to route traffic</label><br>
<label for="q315-d"><input type="radio" id="q315-d" name="q315" value="D"> <strong>D.</strong> Set up AWS Global Accelerator and add endpoints to cater to users in different geographic locations</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up AWS Global Accelerator and add endpoints to cater to users in different geographic locations

</details>

---

## Câu 316

**Chủ đề:** Design Resilient Architectures

A company's cloud architect has set up a solution that uses Amazon Route 53 to configure the DNS records for the primary website with the domain pointing to the Application Load Balancer (ALB). The company wants a solution where users will be directed to a static error page, configured as a backup, in case of unavailability of the primary website.

Which configuration will meet the company's requirements, while keeping the changes to a bare minimum?

**Lựa chọn:**

<label for="q316-a"><input type="radio" id="q316-a" name="q316" value="A"> <strong>A.</strong> Set up Amazon Route 53 active-passive type of failover routing policy. If Amazon Route 53 health check determines the Application Load Balancer endpoint as unhealthy, the traffic will be diverted to a static error page, hosted on Amazon S3 bucket</label><br>
<label for="q316-b"><input type="radio" id="q316-b" name="q316" value="B"> <strong>B.</strong> Set up Amazon Route 53 active-active type of failover routing policy. If Amazon Route 53 health check determines the Application Load Balancer endpoint as unhealthy, the traffic will be diverted to a static error page, hosted on Amazon S3 bucket</label><br>
<label for="q316-c"><input type="radio" id="q316-c" name="q316" value="C"> <strong>C.</strong> Use Amazon Route 53 Latency-based routing. Create a latency record to point to the Amazon S3 bucket that holds the error page to be displayed</label><br>
<label for="q316-d"><input type="radio" id="q316-d" name="q316" value="D"> <strong>D.</strong> Use Amazon Route 53 Weighted routing to give minimum weight to Amazon S3 bucket that holds the error page to be displayed. In case of primary failure, the requests get routed to the error page</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Set up Amazon Route 53 active-passive type of failover routing policy. If Amazon Route 53 health check determines the Application Load Balancer endpoint as unhealthy, the traffic will be diverted to a static error page, hosted on Amazon S3 bucket

</details>

---

## Câu 317

**Chủ đề:** Design Secure Architectures

An application hosted on Amazon EC2 contains sensitive personal information about all its customers and needs to be protected from all types of cyber-attacks. The company is considering using the AWS Web Application Firewall (AWS WAF) to handle this requirement.

Can you identify the correct solution leveraging the capabilities of AWS WAF?

**Lựa chọn:**

<label for="q317-a"><input type="radio" id="q317-a" name="q317" value="A"> <strong>A.</strong> Create Amazon CloudFront distribution for the application on Amazon EC2 instances. Deploy AWS WAF on Amazon CloudFront to provide the necessary safety measures</label><br>
<label for="q317-b"><input type="radio" id="q317-b" name="q317" value="B"> <strong>B.</strong> Configure an Application Load Balancer (ALB) to balance the workload for all the Amazon EC2 instances. Configure Amazon CloudFront to distribute from an Application Load Balancer since AWS WAF cannot be directly configured on ALB. This configuration not only provides necessary safety but is scalable too</label><br>
<label for="q317-c"><input type="radio" id="q317-c" name="q317" value="C"> <strong>C.</strong> AWS WAF can be directly configured on Amazon EC2 instances for ensuring the security of the underlying application data</label><br>
<label for="q317-d"><input type="radio" id="q317-d" name="q317" value="D"> <strong>D.</strong> AWS WAF can be directly configured only on an Application Load Balancer or an Amazon API Gateway. One of these two services can then be configured with Amazon EC2 to build the needed secure architecture</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create Amazon CloudFront distribution for the application on Amazon EC2 instances. Deploy AWS WAF on Amazon CloudFront to provide the necessary safety measures

</details>

---

## Câu 318

**Chủ đề:** Design High-Performing Architectures

A company hires experienced specialists to analyze the customer service calls attended by its call center representatives. Now, the company wants to move to AWS Cloud and is looking at an automated solution to analyze customer service calls for sentiment analysis via ad-hoc SQL queries.

As a Solutions Architect, which of the following solutions would you recommend?

**Lựa chọn:**

<label for="q318-a"><input type="radio" id="q318-a" name="q318" value="A"> <strong>A.</strong> Use Amazon Kinesis Data Streams to read the audio files and machine learning (ML) algorithms to convert the audio files into text and run customer sentiment analysis</label><br>
<label for="q318-b"><input type="radio" id="q318-b" name="q318" value="B"> <strong>B.</strong> Use Amazon Kinesis Data Streams to read the audio files and Amazon Alexa to convert them into text. Amazon Kinesis Data Analytics can be used to analyze these files and Amazon Quicksight can be used to visualize and display the output</label><br>
<label for="q318-c"><input type="radio" id="q318-c" name="q318" value="C"> <strong>C.</strong> Use Amazon Transcribe to convert audio files to text and Amazon Athena to perform SQL based analysis to understand the underlying customer sentiments</label><br>
<label for="q318-d"><input type="radio" id="q318-d" name="q318" value="D"> <strong>D.</strong> Use Amazon Transcribe to convert audio files to text and Amazon Quicksight to perform SQL based analysis on these text files to understand the underlying patterns. Visualize and display them onto user Dashboards for reporting purposes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Amazon Transcribe to convert audio files to text and Amazon Athena to perform SQL based analysis to understand the underlying customer sentiments

</details>

---

## Câu 319

**Chủ đề:** Design High-Performing Architectures

A global e-commerce platform currently operates its order processing system in a single on-premises data center located in Europe. As the company grows its customer base across Asia and North America, it plans to deploy the application across multiple AWS Regions to improve availability and reduce latency. The company requires that updates to the central order database be completed in under one second with global consistency. The application layer will be deployed separately in each Region, but the order management data must remain centrally managed and globally synchronized.

Which solution should a solutions architect recommend to meet these requirements?

**Lựa chọn:**

<label for="q319-a"><input type="radio" id="q319-a" name="q319" value="A"> <strong>A.</strong> Migrate the order data to Amazon DynamoDB and create a global table. Deploy the application in each Region and connect to the local DynamoDB replica for low-latency access</label><br>
<label for="q319-b"><input type="radio" id="q319-b" name="q319" value="B"> <strong>B.</strong> Use Amazon RDS for MySQL with a cross-Region read replica. Route all writes to the primary Region and use read replicas for local access in other Regions</label><br>
<label for="q319-c"><input type="radio" id="q319-c" name="q319" value="C"> <strong>C.</strong> Use Amazon Neptune to store tracking updates as graph data. Deploy clusters in each Region and replicate changes using custom-built Lambda functions and Amazon SQS.</label><br>
<label for="q319-d"><input type="radio" id="q319-d" name="q319" value="D"> <strong>D.</strong> Use Amazon Aurora database with MySQL engine, and configure read-only nodes in other Regions to handle local traffic while routing all write operations to the central Region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Migrate the order data to Amazon DynamoDB and create a global table. Deploy the application in each Region and connect to the local DynamoDB replica for low-latency access

</details>

---

## Câu 320

**Chủ đề:** Design High-Performing Architectures

A financial data processing company runs a workload on Amazon EC2 instances that fetch and process real-time transaction batches from an Amazon SQS queue. The application needs to scale based on unpredictable message volume, which fluctuates significantly throughout the day. The system must process messages with minimal delay and no downtime, even during peak spikes. The company is seeking a solution that balances cost-efficiency with availability and elasticity.

Which EC2 purchasing strategy best meets these requirements in the most cost-effective manner?

**Lựa chọn:**

<label for="q320-a"><input type="radio" id="q320-a" name="q320" value="A"> <strong>A.</strong> Purchase EC2 Reserved Instances to match peak capacity and assign all message processing tasks to these instances regardless of load variations</label><br>
<label for="q320-b"><input type="radio" id="q320-b" name="q320" value="B"> <strong>B.</strong> Use EC2 Spot Instances exclusively with Auto Scaling enabled to match message volume fluctuations and save on compute costs</label><br>
<label for="q320-c"><input type="radio" id="q320-c" name="q320" value="C"> <strong>C.</strong> Use Reserved Instances for the baseline level of traffic and configure EC2 Auto Scaling with Spot Instances to handle spikes in message volume</label><br>
<label for="q320-d"><input type="radio" id="q320-d" name="q320" value="D"> <strong>D.</strong> Use EC2 Reserved Instances for the baseline workload and configure EC2 Auto Scaling to launch On-Demand Instances for all traffic spikes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use Reserved Instances for the baseline level of traffic and configure EC2 Auto Scaling with Spot Instances to handle spikes in message volume

</details>

---

## Câu 321

**Chủ đề:** Design Resilient Architectures

A health-care company manages its web application on Amazon EC2 instances running behind Auto Scaling group (ASG). The company provides ambulances for critical patients and needs the application to be reliable. The workload of the company can be managed on 2 Amazon EC2 instances and can peak up to 6 instances when traffic increases.

As a Solutions Architect, which of the following configurations would you select as the best fit for these requirements?

**Lựa chọn:**

<label for="q321-a"><input type="radio" id="q321-a" name="q321" value="A"> <strong>A.</strong> The Auto Scaling group should be configured with the minimum capacity set to 4, with 2 instances each in two different Availability Zones. The maximum capacity of the Auto Scaling group should be set to 6</label><br>
<label for="q321-b"><input type="radio" id="q321-b" name="q321" value="B"> <strong>B.</strong> The Auto Scaling group should be configured with the minimum capacity set to 2, with 1 instance each in two different Availability Zones. The maximum capacity of the Auto Scaling group should be set to 6</label><br>
<label for="q321-c"><input type="radio" id="q321-c" name="q321" value="C"> <strong>C.</strong> The Auto Scaling group should be configured with the minimum capacity set to 2 and the maximum capacity set to 6 in a single Availability Zone</label><br>
<label for="q321-d"><input type="radio" id="q321-d" name="q321" value="D"> <strong>D.</strong> The Auto Scaling group should be configured with the minimum capacity set to 4, with 2 instances each in two different AWS Regions. The maximum capacity of the Auto Scaling group should be set to 6</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. The Auto Scaling group should be configured with the minimum capacity set to 4, with 2 instances each in two different Availability Zones. The maximum capacity of the Auto Scaling group should be set to 6

</details>

---

## Câu 322

**Chủ đề:** Design Secure Architectures

A biomedical research firm operates a file exchange system for external research partners to upload and download experimental data. Currently, the system runs on two Amazon EC2 Linux instances, each configured with Elastic IP addresses to allow access from trusted IPs. File transfers use the SFTP protocol, and Linux user accounts are manually provisioned to enforce file-level access control. Data is stored on a shared file system mounted to both EC2 instances. The firm wants to modernize the solution to a fully managed, serverless model with high IOPS, fine-grained user permission control, and strict IP-based access restrictions. They also want to reduce operational overhead without sacrificing performance or security.

Which solution best meets these requirements?

**Lựa chọn:**

<label for="q322-a"><input type="radio" id="q322-a" name="q322" value="A"> <strong>A.</strong> Use Amazon EFS with encryption enabled. Create an AWS Transfer Family SFTP endpoint in a VPC with Elastic IP addresses. Restrict access using a security group that allows traffic only from known IPs. Manage user access using POSIX identity mappings and IAM policies</label><br>
<label for="q322-b"><input type="radio" id="q322-b" name="q322" value="B"> <strong>B.</strong> Use Amazon FSx for Lustre as the backend storage. Create an AWS Transfer Family SFTP service with a public endpoint. Configure IAM policies to manage user access and attach a security group that restricts access to trusted IP addresses</label><br>
<label for="q322-c"><input type="radio" id="q322-c" name="q322" value="C"> <strong>C.</strong> Use AWS Storage Gateway in file gateway mode to expose an NFS file share. Deploy AWS Transfer Family with a public endpoint and map user identities using IAM roles. Configure IP allow lists using AWS WAF</label><br>
<label for="q322-d"><input type="radio" id="q322-d" name="q322" value="D"> <strong>D.</strong> Use Amazon S3 with server-side encryption enabled. Create an AWS Transfer Family SFTP endpoint with a VPC endpoint in a private subnet. Restrict access to known IPs using security group rules. Manage user-level permissions using IAM role-based access mappings</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon EFS with encryption enabled. Create an AWS Transfer Family SFTP endpoint in a VPC with Elastic IP addresses. Restrict access using a security group that allows traffic only from known IPs. Manage user access using POSIX identity mappings and IAM policies

</details>

---

## Câu 323

**Chủ đề:** Design Secure Architectures

While troubleshooting, a cloud architect realized that the Amazon EC2 instance is unable to connect to the internet using the Internet Gateway.

Which conditions should be met for internet connectivity to be established? (Select two)

**Lựa chọn:**

<label for="q323-a"><input type="checkbox" id="q323-a" name="q323" value="A"> <strong>A.</strong> The instance's subnet is not associated with any route table</label><br>
<label for="q323-b"><input type="checkbox" id="q323-b" name="q323" value="B"> <strong>B.</strong> The network access control list (network ACL) associated with the subnet must have rules to allow inbound and outbound traffic</label><br>
<label for="q323-c"><input type="checkbox" id="q323-c" name="q323" value="C"> <strong>C.</strong> The instance's subnet is associated with multiple route tables with conflicting configurations</label><br>
<label for="q323-d"><input type="checkbox" id="q323-d" name="q323" value="D"> <strong>D.</strong> The route table in the instance’s subnet should have a route to an Internet Gateway</label><br>
<label for="q323-e"><input type="checkbox" id="q323-e" name="q323" value="E"> <strong>E.</strong> The subnet has been configured to be public and has no access to the internet</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. The network access control list (network ACL) associated with the subnet must have rules to allow inbound and outbound traffic

D. The route table in the instance’s subnet should have a route to an Internet Gateway

</details>

---

## Câu 324

**Chủ đề:** Design High-Performing Architectures

A financial analytics firm runs performance-intensive modeling software on Amazon EC2 instances backed by Amazon EBS volumes. The production data resides on EBS volumes attached to EC2 instances in the same AWS Region where the testing environment is hosted. To maintain data integrity, any changes made during testing must not affect production data. The development team needs to frequently create clones of this production data for simulations. The modeling software requires high and consistent I/O performance, and the firm wants to minimize the time required to provision test data.

Which solution should a solutions architect recommend to meet these requirements?

**Lựa chọn:**

<label for="q324-a"><input type="radio" id="q324-a" name="q324" value="A"> <strong>A.</strong> Create Amazon EBS-backed Amazon Machine Images (AMIs) from the production EC2 instances. Launch new EC2 instances in the test environment from the AMIs. Use Amazon EC2 instance store volumes for temporary simulation data</label><br>
<label for="q324-b"><input type="radio" id="q324-b" name="q324" value="B"> <strong>B.</strong> Create new EBS volumes in the test environment and use AWS Backup to perform a backup job of the production volumes. Restore the backup directly to the test EBS volumes to begin simulations</label><br>
<label for="q324-c"><input type="radio" id="q324-c" name="q324" value="C"> <strong>C.</strong> Take snapshots of the production EBS volumes. Enable EBS fast snapshot restore on the snapshots. Create new EBS volumes from the snapshots and attach them to EC2 instances in the test environment</label><br>
<label for="q324-d"><input type="radio" id="q324-d" name="q324" value="D"> <strong>D.</strong> Use Amazon EBS io2 volumes with Multi-Attach enabled. Attach the same production EBS volumes to both the production and test EC2 instances simultaneously to avoid cloning delays and ensure high IOPS performance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Take snapshots of the production EBS volumes. Enable EBS fast snapshot restore on the snapshots. Create new EBS volumes from the snapshots and attach them to EC2 instances in the test environment

</details>

---

## Câu 325

**Chủ đề:** Design High-Performing Architectures

The engineering team at a weather tracking company wants to enhance the performance of its relational database and is looking for a caching solution that supports geospatial data.

As a solutions architect, which of the following solutions will you suggest?

**Lựa chọn:**

<label for="q325-a"><input type="radio" id="q325-a" name="q325" value="A"> <strong>A.</strong> Use Amazon ElastiCache for Memcached</label><br>
<label for="q325-b"><input type="radio" id="q325-b" name="q325" value="B"> <strong>B.</strong> Use Amazon ElastiCache for Redis</label><br>
<label for="q325-c"><input type="radio" id="q325-c" name="q325" value="C"> <strong>C.</strong> Use Amazon DynamoDB Accelerator (DAX)</label><br>
<label for="q325-d"><input type="radio" id="q325-d" name="q325" value="D"> <strong>D.</strong> Use AWS Global Accelerator</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use Amazon ElastiCache for Redis

</details>

---

## Câu 326

**Chủ đề:** Design Cost-Optimized Architectures

A tech enterprise operates several workloads using Amazon EC2, AWS Fargate, and AWS Lambda across various teams. To optimize compute costs, the company has purchased Compute Savings Plans. The cloud operations team needs to implement a solution that not only monitors utilization but also sends automated alerts when coverage levels of the Compute Savings Plans fall below a defined threshold.

What is the MOST operationally efficient way to achieve this?

**Lựa chọn:**

<label for="q326-a"><input type="radio" id="q326-a" name="q326" value="A"> <strong>A.</strong> Use AWS Budgets to create a daily coverage budget specifically for Compute Savings Plans. Define a coverage threshold and configure notifications to alert relevant stakeholders</label><br>
<label for="q326-b"><input type="radio" id="q326-b" name="q326" value="B"> <strong>B.</strong> Configure a custom script that queries the Savings Plans utilization API and pushes results to an Amazon S3 bucket. Use Amazon QuickSight to visualize coverage and email reports weekly</label><br>
<label for="q326-c"><input type="radio" id="q326-c" name="q326" value="C"> <strong>C.</strong> Enable Compute Optimizer recommendations for EC2 and Fargate. Configure automatic notifications for cost optimization opportunities and Savings Plans coverage drops</label><br>
<label for="q326-d"><input type="radio" id="q326-d" name="q326" value="D"> <strong>D.</strong> Create a standalone dashboard in Amazon CloudWatch to track EC2 and Fargate usage. Use metric math to estimate coverage and trigger alarms</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS Budgets to create a daily coverage budget specifically for Compute Savings Plans. Define a coverage threshold and configure notifications to alert relevant stakeholders

</details>

---

## Câu 327

**Chủ đề:** Design Cost-Optimized Architectures

A software engineering intern at a company is documenting the features offered by Amazon EC2 Spot instances and Spot fleets.

Can you help the intern by selecting the correct options that identify the key characteristics of these two types of Spot entities? (Select two)

**Lựa chọn:**

<label for="q327-a"><input type="checkbox" id="q327-a" name="q327" value="A"> <strong>A.</strong> Spot instances are spare Amazon EC2 capacity that can save you up 90% off of On-Demand prices. Spot instances can be interrupted by Amazon EC2 for capacity requirements with a 2-minute notification</label><br>
<label for="q327-b"><input type="checkbox" id="q327-b" name="q327" value="B"> <strong>B.</strong> Spot fleets allow you to request Amazon EC2 Spot instances for 1 to 6 hours at a time to avoid being interrupted</label><br>
<label for="q327-c"><input type="checkbox" id="q327-c" name="q327" value="C"> <strong>C.</strong> A Spot fleet can consist of a set of Spot Instances and optionally On-Demand Instances that are launched to meet your target capacity</label><br>
<label for="q327-d"><input type="checkbox" id="q327-d" name="q327" value="D"> <strong>D.</strong> A Spot fleet can only consist of a set of Spot Instances that are launched to meet your target capacity</label><br>
<label for="q327-e"><input type="checkbox" id="q327-e" name="q327" value="E"> <strong>E.</strong> Spot fleets are spare EC2 capacity that can save you up 90% off of On-Demand prices. Spot fleets are usually interrupted by Amazon EC2 for capacity requirements with a 2-minute notification</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Spot instances are spare Amazon EC2 capacity that can save you up 90% off of On-Demand prices. Spot instances can be interrupted by Amazon EC2 for capacity requirements with a 2-minute notification

C. A Spot fleet can consist of a set of Spot Instances and optionally On-Demand Instances that are launched to meet your target capacity

</details>

---

## Câu 328

**Chủ đề:** Design Cost-Optimized Architectures

The data engineering team at a company wants to analyze Amazon S3 storage access patterns to decide when to transition the right data to the right storage class.

Which of the following represents a correct option regarding the capabilities of Amazon S3 Analytics storage class analysis?

**Lựa chọn:**

<label for="q328-a"><input type="radio" id="q328-a" name="q328" value="A"> <strong>A.</strong> Storage class analysis only provides recommendations for Standard to Standard One-Zone IA classes</label><br>
<label for="q328-b"><input type="radio" id="q328-b" name="q328" value="B"> <strong>B.</strong> Storage class analysis only provides recommendations for Standard to Glacier Deep Archive classes</label><br>
<label for="q328-c"><input type="radio" id="q328-c" name="q328" value="C"> <strong>C.</strong> Storage class analysis only provides recommendations for Standard to Glacier Flexible Retrieval classes</label><br>
<label for="q328-d"><input type="radio" id="q328-d" name="q328" value="D"> <strong>D.</strong> Storage class analysis only provides recommendations for Standard to Standard IA classes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Storage class analysis only provides recommendations for Standard to Standard IA classes

</details>

---

## Câu 329

**Chủ đề:** Design Secure Architectures

The engineering team at a multi-national company uses AWS Firewall Manager to centrally configure and manage firewall rules across its accounts and applications using AWS Organizations.

Which of the following AWS resources can the AWS Firewall Manager configure rules on? (Select three)

**Lựa chọn:**

<label for="q329-a"><input type="checkbox" id="q329-a" name="q329" value="A"> <strong>A.</strong> AWS Web Application Firewall (AWS WAF)</label><br>
<label for="q329-b"><input type="checkbox" id="q329-b" name="q329" value="B"> <strong>B.</strong> Amazon GuardDuty</label><br>
<label for="q329-c"><input type="checkbox" id="q329-c" name="q329" value="C"> <strong>C.</strong> Amazon Inspector</label><br>
<label for="q329-d"><input type="checkbox" id="q329-d" name="q329" value="D"> <strong>D.</strong> AWS Shield Advanced</label><br>
<label for="q329-e"><input type="checkbox" id="q329-e" name="q329" value="E"> <strong>E.</strong> VPC Route Table</label><br>
<label for="q329-f"><input type="checkbox" id="q329-f" name="q329" value="F"> <strong>F.</strong> VPC Security Group</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. AWS Web Application Firewall (AWS WAF)

D. AWS Shield Advanced

F. VPC Security Group

</details>

---

## Câu 330

**Chủ đề:** Design Resilient Architectures

A company manages a multi-tier social media application that runs on Amazon Elastic Compute Cloud (Amazon EC2) instances behind an Application Load Balancer. The instances run in an Amazon EC2 Auto Scaling group across multiple Availability Zones (AZs) and use an Amazon Aurora database. As an AWS Certified Solutions Architect – Associate, you have been tasked to make the application more resilient to periodic spikes in read request rates.

Which of the following solutions would you recommend for the given use-case? (Select two)

**Lựa chọn:**

<label for="q330-a"><input type="checkbox" id="q330-a" name="q330" value="A"> <strong>A.</strong> Use Amazon Aurora Replica</label><br>
<label for="q330-b"><input type="checkbox" id="q330-b" name="q330" value="B"> <strong>B.</strong> Use AWS Shield</label><br>
<label for="q330-c"><input type="checkbox" id="q330-c" name="q330" value="C"> <strong>C.</strong> Use AWS Global Accelerator</label><br>
<label for="q330-d"><input type="checkbox" id="q330-d" name="q330" value="D"> <strong>D.</strong> Use AWS Direct Connect</label><br>
<label for="q330-e"><input type="checkbox" id="q330-e" name="q330" value="E"> <strong>E.</strong> Use Amazon CloudFront distribution in front of the Application Load Balancer</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon Aurora Replica

E. Use Amazon CloudFront distribution in front of the Application Load Balancer

</details>

---

## Câu 331

**Chủ đề:** Design High-Performing Architectures

A company uses Amazon DynamoDB as a data store for various kinds of customer data, such as user profiles, user events, clicks, and visited links. Some of these use-cases require a high request rate (millions of requests per second), low predictable latency, and reliability. The company now wants to add a caching layer to support high read volumes.

As a solutions architect, which of the following AWS services would you recommend as a caching layer for this use-case? (Select two)

**Lựa chọn:**

<label for="q331-a"><input type="checkbox" id="q331-a" name="q331" value="A"> <strong>A.</strong> Amazon DynamoDB Accelerator (DAX)</label><br>
<label for="q331-b"><input type="checkbox" id="q331-b" name="q331" value="B"> <strong>B.</strong> Amazon ElastiCache</label><br>
<label for="q331-c"><input type="checkbox" id="q331-c" name="q331" value="C"> <strong>C.</strong> Amazon Relational Database Service (Amazon RDS)</label><br>
<label for="q331-d"><input type="checkbox" id="q331-d" name="q331" value="D"> <strong>D.</strong> Amazon OpenSearch Service</label><br>
<label for="q331-e"><input type="checkbox" id="q331-e" name="q331" value="E"> <strong>E.</strong> Amazon Redshift</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon DynamoDB Accelerator (DAX)

B. Amazon ElastiCache

</details>

---

## Câu 332

**Chủ đề:** Design Resilient Architectures

A startup uses a fleet of Amazon EC2 servers to manage its CRM application. These Amazon EC2 servers are behind Elastic Load Balancing (ELB). Which of the following configurations are NOT allowed for Elastic Load Balancing?

**Lựa chọn:**

<label for="q332-a"><input type="radio" id="q332-a" name="q332" value="A"> <strong>A.</strong> Use the Elastic Load Balancing to distribute traffic for four Amazon EC2 instances. All the four instances are deployed across two Availability Zones of us-east-1 region</label><br>
<label for="q332-b"><input type="radio" id="q332-b" name="q332" value="B"> <strong>B.</strong> Use the Elastic Load Balancing to distribute traffic for four Amazon EC2 instances. Two of these instances are deployed in Availability Zone A of us-east-1 region and the other two instances are deployed in Availability Zone B of us-west-1 region</label><br>
<label for="q332-c"><input type="radio" id="q332-c" name="q332" value="C"> <strong>C.</strong> Use the Elastic Load Balancing to distribute traffic for four Amazon EC2 instances. All the four instances are deployed in Availability Zone A of us-east-1 region</label><br>
<label for="q332-d"><input type="radio" id="q332-d" name="q332" value="D"> <strong>D.</strong> Use the Elastic Load Balancing to distribute traffic for four Amazon EC2 instances. All the four instances are deployed in Availability Zone B of us-west-1 region</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use the Elastic Load Balancing to distribute traffic for four Amazon EC2 instances. Two of these instances are deployed in Availability Zone A of us-east-1 region and the other two instances are deployed in Availability Zone B of us-west-1 region

</details>

---

## Câu 333

**Chủ đề:** Design Secure Architectures

A developer has configured inbound traffic for the relevant ports in both the Security Group of the Amazon EC2 instance as well as the network access control list (network ACL) of the subnet for the Amazon EC2 instance. The developer is, however, unable to connect to the service running on the Amazon EC2 instance.

As a solutions architect, how will you fix this issue?

**Lựa chọn:**

<label for="q333-a"><input type="radio" id="q333-a" name="q333" value="A"> <strong>A.</strong> Network access control list (network ACL) are stateful, so allowing inbound traffic to the necessary ports enables the connection. Security Groups are stateless, so you must allow both inbound and outbound traffic</label><br>
<label for="q333-b"><input type="radio" id="q333-b" name="q333" value="B"> <strong>B.</strong> IAM Role defined in the Security Group is different from the IAM Role that is given access in the network access control list (network ACL)</label><br>
<label for="q333-c"><input type="radio" id="q333-c" name="q333" value="C"> <strong>C.</strong> Security Groups are stateful, so allowing inbound traffic to the necessary ports enables the connection. Network access control list (network ACL) are stateless, so you must allow both inbound and outbound traffic</label><br>
<label for="q333-d"><input type="radio" id="q333-d" name="q333" value="D"> <strong>D.</strong> Rules associated with network access control list (network ACL) should never be modified from command line. An attempt to modify rules from command line blocks the rule and results in an erratic behavior</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Security Groups are stateful, so allowing inbound traffic to the necessary ports enables the connection. Network access control list (network ACL) are stateless, so you must allow both inbound and outbound traffic

</details>

---

## Câu 334

**Chủ đề:** Design Cost-Optimized Architectures

The engineering team at a social media company has noticed that while some of the images stored in Amazon S3 are frequently accessed, others sit idle for a considerable span of time.

As a solutions architect, what is your recommendation to build the MOST cost-effective solution?

**Lựa chọn:**

<label for="q334-a"><input type="radio" id="q334-a" name="q334" value="A"> <strong>A.</strong> Store the images using the Amazon S3 Intelligent-Tiering storage class</label><br>
<label for="q334-b"><input type="radio" id="q334-b" name="q334" value="B"> <strong>B.</strong> Store the images using the Amazon S3 Standard-IA storage class</label><br>
<label for="q334-c"><input type="radio" id="q334-c" name="q334" value="C"> <strong>C.</strong> Create a data monitoring application on an Amazon EC2 instance in the same region as the bucket storing the images. The application is triggered daily via Amazon CloudWatch and it changes the storage class of infrequently accessed objects to Amazon S3 One Zone-IA and the frequently accessed objects are migrated to Amazon S3 Standard class</label><br>
<label for="q334-d"><input type="radio" id="q334-d" name="q334" value="D"> <strong>D.</strong> Create a data monitoring application on an Amazon EC2 instance in the same region as the bucket storing the images. The application is triggered daily via Amazon CloudWatch and it changes the storage class of infrequently accessed objects to Amazon S3 Standard-IA and the frequently accessed objects are migrated to Amazon S3 Standard class</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Store the images using the Amazon S3 Intelligent-Tiering storage class

</details>

---

## Câu 335

**Chủ đề:** Design High-Performing Architectures

A healthcare startup is deploying an AWS-based analytics platform that processes sensitive patient records. The application backend uses Amazon RDS for structured data and Amazon S3 for storing medical files. S3 Event Notifications trigger AWS Lambda for real-time data classification and alerting. The startup uses AWS IAM Identity Center to manage federated access from their enterprise directory. Development, operations, and compliance teams require granular and secure access to RDS and S3 resources, based strictly on their job roles. The company must follow the principle of least privilege while minimizing manual administrative work.

Which solution should the company implement to meet these requirements with the least operational overhead?

**Lựa chọn:**

<label for="q335-a"><input type="radio" id="q335-a" name="q335" value="A"> <strong>A.</strong> Create individual IAM users for each team member. Attach role-based IAM policies granting permissions to RDS and S3 based on team roles. Use AWS IAM Access Analyzer to monitor for unused permissions and rotate access keys periodically</label><br>
<label for="q335-b"><input type="radio" id="q335-b" name="q335" value="B"> <strong>B.</strong> Create an IAM identity provider that integrates with the company's IdP (e.g., Azure AD or Okta). Use SAML federation to grant access to IAM roles that are manually assigned to each user. Create and maintain inline IAM policies for each role to access RDS and S3</label><br>
<label for="q335-c"><input type="radio" id="q335-c" name="q335" value="C"> <strong>C.</strong> Use AWS IAM Identity Center integrated with the organization’s directory. Define permission sets with least-privilege policies for Amazon RDS and Amazon S3. Assign users to groups based on their team roles and map those groups to the appropriate permission sets</label><br>
<label for="q335-d"><input type="radio" id="q335-d" name="q335" value="D"> <strong>D.</strong> Use AWS Organizations to group team accounts under a single organizational unit (OU). Attach Service Control Policies (SCPs) to the OU that define access boundaries for Amazon RDS and Amazon S3 based on each team’s responsibilities. Assign users to accounts and let SCPs enforce the required access</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use AWS IAM Identity Center integrated with the organization’s directory. Define permission sets with least-privilege policies for Amazon RDS and Amazon S3. Assign users to groups based on their team roles and map those groups to the appropriate permission sets

</details>

---

## Câu 336

**Chủ đề:** Design Resilient Architectures

A systems administration team has a requirement to run certain custom scripts only once during the launch of the Amazon Elastic Compute Cloud (Amazon EC2) instances that host their application.

Which of the following represents the best way of configuring a solution for this requirement with minimal effort?

**Lựa chọn:**

<label for="q336-a"><input type="radio" id="q336-a" name="q336" value="A"> <strong>A.</strong> Update Amazon EC2 instance configuration to ensure that the custom scripts, added as user data scripts, are run only during the boot process</label><br>
<label for="q336-b"><input type="radio" id="q336-b" name="q336" value="B"> <strong>B.</strong> Run the custom scripts as user data scripts on the Amazon EC2 instances</label><br>
<label for="q336-c"><input type="radio" id="q336-c" name="q336" value="C"> <strong>C.</strong> Run the custom scripts as instance metadata scripts on the Amazon EC2 instances</label><br>
<label for="q336-d"><input type="radio" id="q336-d" name="q336" value="D"> <strong>D.</strong> Use AWS CLI to run the user data scripts only once while launching the instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Run the custom scripts as user data scripts on the Amazon EC2 instances

</details>

---

## Câu 337

**Chủ đề:** Design Secure Architectures

A company has many Amazon Virtual Private Cloud (Amazon VPC) in various accounts, that need to be connected in a star network with one another and connected with on-premises networks through AWS Direct Connect.

What do you recommend?

**Lựa chọn:**

<label for="q337-a"><input type="radio" id="q337-a" name="q337" value="A"> <strong>A.</strong> VPC Peering Connection</label><br>
<label for="q337-b"><input type="radio" id="q337-b" name="q337" value="B"> <strong>B.</strong> Virtual private gateway (VGW)</label><br>
<label for="q337-c"><input type="radio" id="q337-c" name="q337" value="C"> <strong>C.</strong> AWS Transit Gateway</label><br>
<label for="q337-d"><input type="radio" id="q337-d" name="q337" value="D"> <strong>D.</strong> AWS PrivateLink</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. AWS Transit Gateway

</details>

---

## Câu 338

**Chủ đề:** Design Resilient Architectures

A healthcare company runs a fleet of Amazon EC2 instances in two private subnets (named PR1 and PR2) across two Availability Zones (AZs) named A1 and A2. The Amazon EC2 instances need access to the internet for operating system patch management and third-party software maintenance. To facilitate this, the engineering team at the company wants to set up two Network Address Translation gateways (NAT gateways) in a highly available configuration.

Which of the following options would you suggest?

**Lựa chọn:**

<label for="q338-a"><input type="radio" id="q338-a" name="q338" value="A"> <strong>A.</strong> Set up a total of two NAT gateways. NAT gateway N1 should be set up in private subnet PR1 in Availability Zone A1. NAT gateway N2 should be set up in private subnet PR2 in Availability Zone A2</label><br>
<label for="q338-b"><input type="radio" id="q338-b" name="q338" value="B"> <strong>B.</strong> Set up a total of two NAT gateways. Both NAT gateways N1 and N2 should be set up in a single public subnet PU1 in any of the Availability Zones A1 or A2</label><br>
<label for="q338-c"><input type="radio" id="q338-c" name="q338" value="C"> <strong>C.</strong> Set up a total of one NAT gateway. NAT gateway N1 should be set up in public subnet PU1 in any of the Availability Zones A1 or A2</label><br>
<label for="q338-d"><input type="radio" id="q338-d" name="q338" value="D"> <strong>D.</strong> Set up a total of two NAT gateways. NAT gateway N1 should be set up in public subnet PU1 in Availability Zone A1. NAT gateway N2 should be set up in public subnet PU2 in Availability Zone A2</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up a total of two NAT gateways. NAT gateway N1 should be set up in public subnet PU1 in Availability Zone A1. NAT gateway N2 should be set up in public subnet PU2 in Availability Zone A2

</details>

---

## Câu 339

**Chủ đề:** Design Secure Architectures

During a review, a security team has flagged concerns over an Amazon EC2 instance querying IP addresses used for cryptocurrency mining. The Amazon EC2 instance does not host any authorized application related to cryptocurrency mining.

Which AWS service can be used to protect the Amazon EC2 instances from such unauthorized behavior in the future?

**Lựa chọn:**

<label for="q339-a"><input type="radio" id="q339-a" name="q339" value="A"> <strong>A.</strong> AWS Web Application Firewall (AWS WAF)</label><br>
<label for="q339-b"><input type="radio" id="q339-b" name="q339" value="B"> <strong>B.</strong> AWS Shield Advanced</label><br>
<label for="q339-c"><input type="radio" id="q339-c" name="q339" value="C"> <strong>C.</strong> AWS Firewall Manager</label><br>
<label for="q339-d"><input type="radio" id="q339-d" name="q339" value="D"> <strong>D.</strong> Amazon GuardDuty</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Amazon GuardDuty

</details>

---

## Câu 340

**Chủ đề:** Design Resilient Architectures

A company is developing a document management application on AWS. The application runs on Amazon EC2 instances in multiple Availability Zones (AZs). The company requires the document store to be highly available and the documents need to be returned immediately when requested. The engineering team has configured the application to use Amazon Elastic Block Store (Amazon EBS) to store the documents but the team is willing to consider other options to meet the availability requirement.

As a solutions architect, which of the following will you recommend?

**Lựa chọn:**

<label for="q340-a"><input type="radio" id="q340-a" name="q340" value="A"> <strong>A.</strong> Set up Amazon EBS as the Amazon EC2 instance root volume and then configure the application to use Amazon S3 Glacier as the document store</label><br>
<label for="q340-b"><input type="radio" id="q340-b" name="q340" value="B"> <strong>B.</strong> Create snapshots for the Amazon EBS volumes regularly and then build new volumes using those snapshots in additional Availability Zones</label><br>
<label for="q340-c"><input type="radio" id="q340-c" name="q340" value="C"> <strong>C.</strong> Provision at least three Provisioned IOPS Amazon Instance Store volumes for the Amazon EC2 instances and then mount these volumes to multiple Amazon EC2 instances</label><br>
<label for="q340-d"><input type="radio" id="q340-d" name="q340" value="D"> <strong>D.</strong> Set up Amazon EBS as the Amazon EC2 instance root volume and then configure the application to use Amazon S3 as the document store</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Set up Amazon EBS as the Amazon EC2 instance root volume and then configure the application to use Amazon S3 as the document store

</details>

---

## Câu 341

**Chủ đề:** Design High-Performing Architectures

A development team is looking for a solution that saves development time and deployment costs for an application that uses a high-throughput request-response message pattern.

Which of the following Amazon SQS queue types is the best fit to meet this requirement?

**Lựa chọn:**

<label for="q341-a"><input type="radio" id="q341-a" name="q341" value="A"> <strong>A.</strong> Amazon Simple Queue Service (Amazon SQS) dead-letter queues</label><br>
<label for="q341-b"><input type="radio" id="q341-b" name="q341" value="B"> <strong>B.</strong> Amazon Simple Queue Service (Amazon SQS) FIFO queues</label><br>
<label for="q341-c"><input type="radio" id="q341-c" name="q341" value="C"> <strong>C.</strong> Amazon Simple Queue Service (Amazon SQS) temporary queues</label><br>
<label for="q341-d"><input type="radio" id="q341-d" name="q341" value="D"> <strong>D.</strong> Amazon Simple Queue Service (Amazon SQS) delay queues</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Amazon Simple Queue Service (Amazon SQS) temporary queues

</details>

---

## Câu 342

**Chủ đề:** Design Resilient Architectures

The engineering team at an IT company is deploying an Online Transactional Processing (OLTP) application that needs to support relational queries. The application will have unpredictable spikes of usage that the team does not know in advance.

Which database would you recommend using?

**Lựa chọn:**

<label for="q342-a"><input type="radio" id="q342-a" name="q342" value="A"> <strong>A.</strong> Amazon Aurora Serverless</label><br>
<label for="q342-b"><input type="radio" id="q342-b" name="q342" value="B"> <strong>B.</strong> Amazon ElastiCache</label><br>
<label for="q342-c"><input type="radio" id="q342-c" name="q342" value="C"> <strong>C.</strong> Amazon DynamoDB with Provisioned Capacity and Auto Scaling</label><br>
<label for="q342-d"><input type="radio" id="q342-d" name="q342" value="D"> <strong>D.</strong> Amazon DynamoDB with On-Demand Capacity</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon Aurora Serverless

</details>

---

## Câu 343

**Chủ đề:** Design Cost-Optimized Architectures

The development team at a company manages a Python based nightly process with a runtime of 30 minutes. The process can withstand any interruptions in its execution and start over again. The process currently runs on the on-premises infrastructure and it needs to be migrated to AWS.

Which of the following options do you recommend as the MOST cost-effective solution?

**Lựa chọn:**

<label for="q343-a"><input type="radio" id="q343-a" name="q343" value="A"> <strong>A.</strong> Run on a Spot Instance with a persistent request type</label><br>
<label for="q343-b"><input type="radio" id="q343-b" name="q343" value="B"> <strong>B.</strong> Run on Amazon EMR</label><br>
<label for="q343-c"><input type="radio" id="q343-c" name="q343" value="C"> <strong>C.</strong> Run on AWS Lambda</label><br>
<label for="q343-d"><input type="radio" id="q343-d" name="q343" value="D"> <strong>D.</strong> Run on an Application Load Balancer</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Run on a Spot Instance with a persistent request type

</details>

---

## Câu 344

**Chủ đề:** Design Cost-Optimized Architectures

Your e-commerce application is using an Amazon RDS PostgreSQL database and an analytics workload also runs on the same database. When the analytics workload is run, your e-commerce application slows down which further affects your sales.

Which of the following is the MOST cost-optimal solution to fix this issue?

**Lựa chọn:**

<label for="q344-a"><input type="radio" id="q344-a" name="q344" value="A"> <strong>A.</strong> Create a Read Replica in the same Region as the Master database and point the analytics workload there</label><br>
<label for="q344-b"><input type="radio" id="q344-b" name="q344" value="B"> <strong>B.</strong> Migrate the analytics application to AWS Lambda</label><br>
<label for="q344-c"><input type="radio" id="q344-c" name="q344" value="C"> <strong>C.</strong> Enable Multi-AZ for the Amazon RDS database and run the analytics workload on the standby database</label><br>
<label for="q344-d"><input type="radio" id="q344-d" name="q344" value="D"> <strong>D.</strong> Create a Read Replica in another Region as the Master database and point the analytics workload there</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a Read Replica in the same Region as the Master database and point the analytics workload there

</details>

---

## Câu 345

**Chủ đề:** Design High-Performing Architectures

You are looking to build an index of your files in Amazon S3, using Amazon RDS PostgreSQL. To build this index, it is necessary to read the first 250 bytes of each object in Amazon S3, which contains some metadata about the content of the file itself. There are over 100,000 files in your S3 bucket, amounting to 50 terabytes of data.

How can you build this index efficiently?

**Lựa chọn:**

<label for="q345-a"><input type="radio" id="q345-a" name="q345" value="A"> <strong>A.</strong> Create an application that will traverse the S3 bucket, issue a Byte Range Fetch for the first 250 bytes, and store that information in Amazon RDS</label><br>
<label for="q345-b"><input type="radio" id="q345-b" name="q345" value="B"> <strong>B.</strong> Use the Amazon RDS Import feature to load the data from Amazon S3 to PostgreSQL, and run a SQL query to build the index</label><br>
<label for="q345-c"><input type="radio" id="q345-c" name="q345" value="C"> <strong>C.</strong> Create an application that will traverse the Amazon S3 bucket, read all the files one by one, extract the first 250 bytes, and store that information in Amazon RDS</label><br>
<label for="q345-d"><input type="radio" id="q345-d" name="q345" value="D"> <strong>D.</strong> Create an application that will traverse the Amazon S3 bucket, then use S3 Select Byte Range Fetch parameter to get the first 250 bytes, and store that information in Amazon RDS</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an application that will traverse the S3 bucket, issue a Byte Range Fetch for the first 250 bytes, and store that information in Amazon RDS

</details>

---

## Câu 346

**Chủ đề:** Design Secure Architectures

A healthcare company wants to run its applications on single-tenant hardware to meet compliance guidelines.

Which of the following is the MOST cost-effective way of isolating the Amazon EC2 instances to a single tenant?

**Lựa chọn:**

<label for="q346-a"><input type="radio" id="q346-a" name="q346" value="A"> <strong>A.</strong> Dedicated Instances</label><br>
<label for="q346-b"><input type="radio" id="q346-b" name="q346" value="B"> <strong>B.</strong> Spot Instances</label><br>
<label for="q346-c"><input type="radio" id="q346-c" name="q346" value="C"> <strong>C.</strong> Dedicated Hosts</label><br>
<label for="q346-d"><input type="radio" id="q346-d" name="q346" value="D"> <strong>D.</strong> On-Demand Instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Dedicated Instances

</details>

---

## Câu 347

**Chủ đề:** Design Cost-Optimized Architectures

An organization has rolled out a multi-account architecture using AWS Control Tower to isolate development environments. Each developer has their own dedicated AWS account to provision and test workloads. However, the company is concerned about unexpected spikes in resource usage and AWS spending from individual developer accounts. The leadership team wants to implement a cost control mechanism that can proactively enforce budget limits, ensure automatic responses to overspending, and require minimal ongoing administrative effort.

What is the most efficient solution to meet this goal with the least operational overhead?

**Lựa chọn:**

<label for="q347-a"><input type="radio" id="q347-a" name="q347" value="A"> <strong>A.</strong> Deploy an AWS Lambda function to run daily in each developer’s account. Use the function to analyze cost usage reports via the Cost Explorer API. If costs exceed a predefined threshold, the function invokes an AWS Config remediation rule</label><br>
<label for="q347-b"><input type="radio" id="q347-b" name="q347" value="B"> <strong>B.</strong> Use AWS Budgets to define spending thresholds for each developer’s account. Configure budget alerts to notify developers when actual or forecasted usage exceeds the set limit. Attach Budgets actions to automatically apply a restrictive DenyAll IAM policy to the developer’s primary IAM role when the budget threshold is crossed</label><br>
<label for="q347-c"><input type="radio" id="q347-c" name="q347" value="C"> <strong>C.</strong> Use AWS Service Catalog to restrict developers to predefined resource templates with pricing limits. In each developer account, create a scheduled Lambda function that stops all running resources at the end of the day and and restart these resources at the start of next business day</label><br>
<label for="q347-d"><input type="radio" id="q347-d" name="q347" value="D"> <strong>D.</strong> Use AWS Cost Explorer to enable detailed usage and cost reports for each developer account. Configure daily usage reports to be emailed to developers. Create dashboards for each developer in Cost Explorer, and require them to monitor their resource consumption and take action if they approach spending thresholds</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS Budgets to define spending thresholds for each developer’s account. Configure budget alerts to notify developers when actual or forecasted usage exceeds the set limit. Attach Budgets actions to automatically apply a restrictive DenyAll IAM policy to the developer’s primary IAM role when the budget threshold is crossed

</details>

---

## Câu 348

**Chủ đề:** Design Resilient Architectures

A financial services firm operates a mission-critical transaction processing platform hosted in the AWS us-east-2 Region. The backend is powered by a MySQL-compatible Amazon Aurora cluster, with high transaction volumes throughout the day. As part of its business continuity planning, the firm has selected us-west-2 as its designated disaster recovery (DR) Region.

The firm has defined strict DR objectives:

Recovery Point Objective (RPO): ≤ 5 minutes

Recovery Time Objective (RTO): ≤ 15 minutes

Leadership has asked for a DR solution that ensures fast cross-regional failover with minimal operational overhead and configuration effort. What do you recommend?

**Lựa chọn:**

<label for="q348-a"><input type="radio" id="q348-a" name="q348" value="A"> <strong>A.</strong> Convert the Aurora cluster to an Aurora global database, with the secondary cluster deployed in us-west-2. Rely on Aurora global database managed failover to meet RTO and RPO objectives</label><br>
<label for="q348-b"><input type="radio" id="q348-b" name="q348" value="B"> <strong>B.</strong> Provision a separate Aurora MySQL-compatible cluster in us-west-2, and configure AWS Database Migration Service (AWS DMS) to replicate data from the primary database to the DR cluster continuously. Perform manual failover during DR events</label><br>
<label for="q348-c"><input type="radio" id="q348-c" name="q348" value="C"> <strong>C.</strong> Create an Aurora read replica in us-west-2 with equivalent capacity to the primary cluster's writer node in us-east-2. Monitor replication health and configure a manual promotion process for failover</label><br>
<label for="q348-d"><input type="radio" id="q348-d" name="q348" value="D"> <strong>D.</strong> Deploy a separate Aurora cluster in us-west-2, and use scheduled AWS Lambda functions with custom scripts to export and import snapshots from us-east-2 every 5 minutes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Convert the Aurora cluster to an Aurora global database, with the secondary cluster deployed in us-west-2. Rely on Aurora global database managed failover to meet RTO and RPO objectives

</details>

---

## Câu 349

**Chủ đề:** Design Resilient Architectures

An application is hosted on multiple Amazon EC2 instances in the same Availability Zone (AZ). The engineering team wants to set up shared data access for these Amazon EC2 instances using Amazon EBS Multi-Attach volumes.

Which Amazon EBS volume type is the correct choice for these Amazon EC2 instances?

**Lựa chọn:**

<label for="q349-a"><input type="radio" id="q349-a" name="q349" value="A"> <strong>A.</strong> Provisioned IOPS SSD Amazon EBS volumes</label><br>
<label for="q349-b"><input type="radio" id="q349-b" name="q349" value="B"> <strong>B.</strong> General-purpose SSD-based Amazon EBS volumes</label><br>
<label for="q349-c"><input type="radio" id="q349-c" name="q349" value="C"> <strong>C.</strong> Throughput Optimized HDD Amazon EBS volumes</label><br>
<label for="q349-d"><input type="radio" id="q349-d" name="q349" value="D"> <strong>D.</strong> Cold HDD Amazon EBS volumes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Provisioned IOPS SSD Amazon EBS volumes

</details>

---

## Câu 350

**Chủ đề:** Design Secure Architectures

A retail company needs a secure connection between its on-premises data center and AWS Cloud. This connection does not need high bandwidth and will handle a small amount of traffic. The company wants a quick turnaround time to set up the connection.

What is the MOST cost-effective way to establish such a connection?

**Lựa chọn:**

<label for="q350-a"><input type="radio" id="q350-a" name="q350" value="A"> <strong>A.</strong> Set up a bastion host on Amazon EC2</label><br>
<label for="q350-b"><input type="radio" id="q350-b" name="q350" value="B"> <strong>B.</strong> Set up AWS Direct Connect</label><br>
<label for="q350-c"><input type="radio" id="q350-c" name="q350" value="C"> <strong>C.</strong> Set up an AWS Site-to-Site VPN connection</label><br>
<label for="q350-d"><input type="radio" id="q350-d" name="q350" value="D"> <strong>D.</strong> Set up an Internet Gateway between the on-premises data center and AWS cloud</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set up an AWS Site-to-Site VPN connection

</details>

---

## Câu 351

**Chủ đề:** Design Cost-Optimized Architectures

Your company has created a data warehouse using Amazon Redshift that is used to analyze data from Amazon S3. From the usage pattern, you have detected that after 30 days, the data is rarely queried in Amazon Redshift and it's not "hot data" anymore. You would like to preserve the SQL querying capability on your data and get the queries started immediately. Also, you want to adopt a pricing model that allows you to save the maximum amount of cost on Amazon Redshift.

What do you recommend? (Select two)

**Lựa chọn:**

<label for="q351-a"><input type="checkbox" id="q351-a" name="q351" value="A"> <strong>A.</strong> Migrate the Amazon Redshift underlying storage to Amazon S3 IA</label><br>
<label for="q351-b"><input type="checkbox" id="q351-b" name="q351" value="B"> <strong>B.</strong> Create a smaller Amazon Redshift Cluster with the cold data</label><br>
<label for="q351-c"><input type="checkbox" id="q351-c" name="q351" value="C"> <strong>C.</strong> Move the data to Amazon S3 Glacier Deep Archive after 30 days</label><br>
<label for="q351-d"><input type="checkbox" id="q351-d" name="q351" value="D"> <strong>D.</strong> Move the data to Amazon S3 Standard IA after 30 days</label><br>
<label for="q351-e"><input type="checkbox" id="q351-e" name="q351" value="E"> <strong>E.</strong> Analyze the cold data with Amazon Athena</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Move the data to Amazon S3 Standard IA after 30 days

E. Analyze the cold data with Amazon Athena

</details>

---

## Câu 352

**Chủ đề:** Design Resilient Architectures

A media company is relocating its legacy infrastructure to AWS. The on-premises environment consists of multiple virtualized workloads that are tightly coupled to their host operating systems and cannot be containerized or re-architected due to software constraints. Each workload currently runs on a standalone virtual machine. The engineering team plans to run these workloads on Amazon EC2 instances without modifying their core design. The company needs a solution that ensures high availability and fault tolerance in the AWS Cloud.

Which solution will meet these requirements?

**Lựa chọn:**

<label for="q352-a"><input type="radio" id="q352-a" name="q352" value="A"> <strong>A.</strong> Create Amazon Machine Images (AMIs) for each legacy workload. Use the AMIs to launch Auto Scaling groups with a minimum and maximum capacity of 1 EC2 instance. Place an Application Load Balancer (ALB) in front of the Auto Scaling group to provide routing and health check-based failover.</label><br>
<label for="q352-b"><input type="radio" id="q352-b" name="q352" value="B"> <strong>B.</strong> Generate an Amazon Machine Image (AMI) for each legacy server. Launch two EC2 instances from this AMI, placing one instance in each of two different Availability Zones. Set up a Network Load Balancer (NLB) to route traffic to the instances and to monitor instance health for automatic traffic redirection in case of failure</label><br>
<label for="q352-c"><input type="radio" id="q352-c" name="q352" value="C"> <strong>C.</strong> Use AWS Backup to schedule hourly backups of each EC2 instance to Amazon S3 in a separate Availability Zone. Create a recovery plan that includes manual restoration of instances from backup in the event of a failure</label><br>
<label for="q352-d"><input type="radio" id="q352-d" name="q352" value="D"> <strong>D.</strong> Containerize the legacy applications and deploy them to Amazon ECS using the Fargate launch type. Define a task for each workload, and use an Application Load Balancer to route traffic across multiple Fargate tasks running in separate Availability Zones</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Generate an Amazon Machine Image (AMI) for each legacy server. Launch two EC2 instances from this AMI, placing one instance in each of two different Availability Zones. Set up a Network Load Balancer (NLB) to route traffic to the instances and to monitor instance health for automatic traffic redirection in case of failure

</details>

---

## Câu 353

**Chủ đề:** Design Cost-Optimized Architectures

A research firm archives experimental datasets generated by automated laboratory equipment. Each dataset is about 10 MB in size and is initially accessed frequently for analysis within the first month. After this period, the access rate drops significantly, but the data must remain immediately retrievable if needed. Due to compliance policies, each dataset must be retained in AWS storage for exactly 4 years before deletion. The firm currently stores the data in Amazon S3 Standard storage and wants to minimize costs without compromising data availability or retrieval speed.

Which solution meets these requirements most cost-effectively?

**Lựa chọn:**

<label for="q353-a"><input type="radio" id="q353-a" name="q353" value="A"> <strong>A.</strong> Define an S3 Lifecycle policy that transitions datasets to S3 Glacier Instant Retrieval 30 days after creation and schedules the deletion of each object exactly 4 years after its creation</label><br>
<label for="q353-b"><input type="radio" id="q353-b" name="q353" value="B"> <strong>B.</strong> Define an S3 Lifecycle policy that transitions datasets to S3 Standard-Infrequent Access (S3 Standard-IA) 30 days after creation and schedules the deletion of each object exactly 4 years after its creation</label><br>
<label for="q353-c"><input type="radio" id="q353-c" name="q353" value="C"> <strong>C.</strong> Configure an S3 Lifecycle policy to migrate datasets to S3 Glacier Flexible Retrieval after 30 days and delete them automatically 4 years after creation</label><br>
<label for="q353-d"><input type="radio" id="q353-d" name="q353" value="D"> <strong>D.</strong> Set up an S3 Lifecycle configuration to transfer all datasets to S3 One Zone-Infrequent Access (S3 One Zone-IA) after 30 days, and permanently delete them 4 years after creation</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Define an S3 Lifecycle policy that transitions datasets to S3 Standard-Infrequent Access (S3 Standard-IA) 30 days after creation and schedules the deletion of each object exactly 4 years after its creation

</details>

---

## Câu 354

**Chủ đề:** Design Secure Architectures

A team has around 200 users, each of these having an IAM user account in AWS. Currently, they all have read access to an Amazon S3 bucket. The team wants 50 among them to have write and read access to the buckets.

How can you provide these users access in the least possible time, with minimal changes?

**Lựa chọn:**

<label for="q354-a"><input type="radio" id="q354-a" name="q354" value="A"> <strong>A.</strong> Update the Amazon S3 bucket policy</label><br>
<label for="q354-b"><input type="radio" id="q354-b" name="q354" value="B"> <strong>B.</strong> Create a group, attach the policy to the group and place the users in the group</label><br>
<label for="q354-c"><input type="radio" id="q354-c" name="q354" value="C"> <strong>C.</strong> Create a policy and assign it manually to the 50 users</label><br>
<label for="q354-d"><input type="radio" id="q354-d" name="q354" value="D"> <strong>D.</strong> Create an AWS Multi-Factor Authentication (AWS MFA) user with read / write access and link 50 IAM with AWS MFA</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create a group, attach the policy to the group and place the users in the group

</details>

---

## Câu 355

**Chủ đề:** Design Secure Architectures

A global financial services provider operates data analytics workloads across multiple AWS Regions. The company stores regulated datasets in Amazon S3 buckets and requires visibility into security and compliance configurations. As part of a new audit initiative, the compliance team must identify all S3 buckets across the environment that do not have versioning enabled. The solution must scale across all Regions and accounts with minimal manual intervention.

Which solution will meet these requirements with the LEAST operational overhead?

**Lựa chọn:**

<label for="q355-a"><input type="radio" id="q355-a" name="q355" value="A"> <strong>A.</strong> Configure an AWS CloudTrail trail across all Regions. Create an Amazon EventBridge rule that filters for PutBucketVersioning and DeleteBucketVersioning API calls. Trigger an AWS Lambda function to analyze the bucket configurations and generate a report of unversioned buckets</label><br>
<label for="q355-b"><input type="radio" id="q355-b" name="q355" value="B"> <strong>B.</strong> Enable IAM Access Analyzer for all Regions. Review the analyzer reports to identify S3 buckets without versioning enabled and configure IAM policies to restrict access to such buckets</label><br>
<label for="q355-c"><input type="radio" id="q355-c" name="q355" value="C"> <strong>C.</strong> Create a centralized Amazon S3 Multi-Region Access Point for all buckets. Use this access point to perform versioning checks programmatically by inspecting objects' metadata from each bucket</label><br>
<label for="q355-d"><input type="radio" id="q355-d" name="q355" value="D"> <strong>D.</strong> Enable Amazon S3 Storage Lens with advanced metrics and recommendations. Use the per-bucket dashboard to filter and view versioning status across Regions and identify all buckets that do not have versioning enabled</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Enable Amazon S3 Storage Lens with advanced metrics and recommendations. Use the per-bucket dashboard to filter and view versioning status across Regions and identify all buckets that do not have versioning enabled

</details>

---

## Câu 356

**Chủ đề:** Design High-Performing Architectures

A digital media company wants to track user engagement across its streaming platform by capturing events such as video starts, pauses, and search queries. These events must be ingested and analyzed in real time to improve user experience and optimize recommendations. The platform experiences unpredictable spikes in traffic during popular content releases. The company needs a highly scalable and serverless solution that can seamlessly adjust to changing workloads without manual provisioning.

Which solution will meet these requirements in the MOST efficient and scalable way?

**Lựa chọn:**

<label for="q356-a"><input type="radio" id="q356-a" name="q356" value="A"> <strong>A.</strong> Use an Amazon Kinesis Data Streams stream in on-demand capacity mode to ingest user engagement data. Configure an AWS Lambda function as a consumer to process the events in real time</label><br>
<label for="q356-b"><input type="radio" id="q356-b" name="q356" value="B"> <strong>B.</strong> Use Amazon Kinesis Data Firehose to ingest user events. Set the destination as Amazon S3. Use Amazon Athena with scheduled queries to analyze the data periodically</label><br>
<label for="q356-c"><input type="radio" id="q356-c" name="q356" value="C"> <strong>C.</strong> Use Amazon Simple Notification Service (Amazon SNS) to publish clickstream events. Subscribe an Amazon SQS standard queue to receive the events. Process the events in batches with AWS Glue jobs scheduled at fixed intervals</label><br>
<label for="q356-d"><input type="radio" id="q356-d" name="q356" value="D"> <strong>D.</strong> Deploy a fleet of Amazon EC2 instances running Apache Kafka to ingest clickstream data. Set up custom scripts to manually scale the Kafka cluster based on CPU usage. Use Amazon Athena to run periodic queries on stored clickstream logs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use an Amazon Kinesis Data Streams stream in on-demand capacity mode to ingest user engagement data. Configure an AWS Lambda function as a consumer to process the events in real time

</details>

---

## Câu 357

**Chủ đề:** Design Resilient Architectures

A social media application lets users upload photos and perform image editing operations. The application offers two classes of service: pro and lite. The product team wants the photos submitted by pro users to be processed before those submitted by lite users. Photos are uploaded to Amazon S3 and the job information is sent to Amazon SQS.

As a solutions architect, which of the following solutions would you recommend?

**Lựa chọn:**

<label for="q357-a"><input type="radio" id="q357-a" name="q357" value="A"> <strong>A.</strong> Create two Amazon SQS standard queues: one for pro and one for lite. Set the lite queue to use short polling and the pro queue to use long polling</label><br>
<label for="q357-b"><input type="radio" id="q357-b" name="q357" value="B"> <strong>B.</strong> Create two Amazon SQS standard queues: one for pro and one for lite. Set up Amazon EC2 instances to prioritize polling for the pro queue over the lite queue</label><br>
<label for="q357-c"><input type="radio" id="q357-c" name="q357" value="C"> <strong>C.</strong> Create two Amazon SQS FIFO queues: one for pro and one for lite. Set the lite queue to use short polling and the pro queue to use long polling</label><br>
<label for="q357-d"><input type="radio" id="q357-d" name="q357" value="D"> <strong>D.</strong> Create one Amazon SQS standard queue. Set the visibility timeout of the pro photos to zero. Set up Amazon EC2 instances to prioritize visibility settings so pro photos are processed first</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create two Amazon SQS standard queues: one for pro and one for lite. Set up Amazon EC2 instances to prioritize polling for the pro queue over the lite queue

</details>

---

## Câu 358

**Chủ đề:** Design Cost-Optimized Architectures

A financial services company is looking to move its on-premises IT infrastructure to AWS Cloud. The company has multiple long-term server bound licenses across the application stack and the CTO wants to continue to utilize those licenses while moving to AWS.

As a solutions architect, which of the following would you recommend as the MOST cost-effective solution?

**Lựa chọn:**

<label for="q358-a"><input type="radio" id="q358-a" name="q358" value="A"> <strong>A.</strong> Use Amazon EC2 on-demand instances</label><br>
<label for="q358-b"><input type="radio" id="q358-b" name="q358" value="B"> <strong>B.</strong> Use Amazon EC2 reserved instances (RI)</label><br>
<label for="q358-c"><input type="radio" id="q358-c" name="q358" value="C"> <strong>C.</strong> Use Amazon EC2 dedicated instances</label><br>
<label for="q358-d"><input type="radio" id="q358-d" name="q358" value="D"> <strong>D.</strong> Use Amazon EC2 dedicated hosts</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use Amazon EC2 dedicated hosts

</details>

---

## Câu 359

**Chủ đề:** Design Secure Architectures

A media company has its corporate headquarters in Los Angeles with an on-premises data center using an AWS Direct Connect connection to the AWS VPC. The branch offices in San Francisco and Miami use AWS Site-to-Site VPN connections to connect to the AWS VPC. The company is looking for a solution to have the branch offices send and receive data with each other as well as with their corporate headquarters.

As a solutions architect, which of the following AWS services would you recommend addressing this use-case?

**Lựa chọn:**

<label for="q359-a"><input type="radio" id="q359-a" name="q359" value="A"> <strong>A.</strong> VPC Peering connection</label><br>
<label for="q359-b"><input type="radio" id="q359-b" name="q359" value="B"> <strong>B.</strong> AWS VPN CloudHub</label><br>
<label for="q359-c"><input type="radio" id="q359-c" name="q359" value="C"> <strong>C.</strong> Software VPN</label><br>
<label for="q359-d"><input type="radio" id="q359-d" name="q359" value="D"> <strong>D.</strong> VPC Endpoint</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. AWS VPN CloudHub

</details>

---

## Câu 360

**Chủ đề:** Design High-Performing Architectures

A company's real-time streaming application is running on AWS. As the data is ingested, a job runs on the data and takes 30 minutes to complete. The workload frequently experiences high latency due to large amounts of incoming data. A solutions architect needs to design a scalable and serverless solution to enhance performance.

Which combination of steps should the solutions architect take? (Select two)

**Lựa chọn:**

<label for="q360-a"><input type="checkbox" id="q360-a" name="q360" value="A"> <strong>A.</strong> Set up AWS Database Migration Service (AWS DMS) to ingest the data</label><br>
<label for="q360-b"><input type="checkbox" id="q360-b" name="q360" value="B"> <strong>B.</strong> Set up AWS Lambda with AWS Step Functions to process the data</label><br>
<label for="q360-c"><input type="checkbox" id="q360-c" name="q360" value="C"> <strong>C.</strong> Set up Amazon Kinesis Data Streams to ingest the data</label><br>
<label for="q360-d"><input type="checkbox" id="q360-d" name="q360" value="D"> <strong>D.</strong> Provision Amazon EC2 instances in an Auto Scaling group to process the data</label><br>
<label for="q360-e"><input type="checkbox" id="q360-e" name="q360" value="E"> <strong>E.</strong> Set up AWS Fargate with Amazon ECS to process the data</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Set up Amazon Kinesis Data Streams to ingest the data

E. Set up AWS Fargate with Amazon ECS to process the data

</details>

---

## Câu 361

**Chủ đề:** Design High-Performing Architectures

A biotechnology company has multiple High Performance Computing (HPC) workflows that quickly and accurately process and analyze genomes for hereditary diseases. The company is looking to migrate these workflows from their on-premises infrastructure to AWS Cloud.

As a solutions architect, which of the following networking components would you recommend on the Amazon EC2 instances running these HPC workflows?

**Lựa chọn:**

<label for="q361-a"><input type="radio" id="q361-a" name="q361" value="A"> <strong>A.</strong> Elastic Fabric Adapter (EFA)</label><br>
<label for="q361-b"><input type="radio" id="q361-b" name="q361" value="B"> <strong>B.</strong> Elastic Network Interface (ENI)</label><br>
<label for="q361-c"><input type="radio" id="q361-c" name="q361" value="C"> <strong>C.</strong> Elastic Network Adapter (ENA)</label><br>
<label for="q361-d"><input type="radio" id="q361-d" name="q361" value="D"> <strong>D.</strong> Elastic IP Address (EIP)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Elastic Fabric Adapter (EFA)

</details>

---

## Câu 362

**Chủ đề:** Design Resilient Architectures

An IT company is using Amazon Simple Queue Service (Amazon SQS) queues for decoupling the various components of application architecture. As the consuming components need additional time to process Amazon Simple Queue Service (Amazon SQS) messages, the company wants to postpone the delivery of new messages to the queue for a few seconds.

As a solutions architect, which of the following solutions would you suggest to the company?

**Lựa chọn:**

<label for="q362-a"><input type="radio" id="q362-a" name="q362" value="A"> <strong>A.</strong> Use Amazon SQS FIFO queues to postpone the delivery of new messages to the queue for a few seconds</label><br>
<label for="q362-b"><input type="radio" id="q362-b" name="q362" value="B"> <strong>B.</strong> Use dead-letter queues to postpone the delivery of new messages to the queue for a few seconds</label><br>
<label for="q362-c"><input type="radio" id="q362-c" name="q362" value="C"> <strong>C.</strong> Use visibility timeout to postpone the delivery of new messages to the queue for a few seconds</label><br>
<label for="q362-d"><input type="radio" id="q362-d" name="q362" value="D"> <strong>D.</strong> Use delay queues to postpone the delivery of new messages to the queue for a few seconds</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Use delay queues to postpone the delivery of new messages to the queue for a few seconds

</details>

---

## Câu 363

**Chủ đề:** Design Cost-Optimized Architectures

A technology startup has stabilized its cloud infrastructure after a successful product launch. The backend services are now running at a predictable rate with minimal scaling events. The application architecture includes workloads running on Amazon EC2, AWS Lambda functions for asynchronous processing, container workloads on AWS Fargate, and machine learning inference models deployed with Amazon SageMaker. The company is now focusing on reducing long-term operational expenses without redesigning its architecture. The company wants to apply long-term pricing discounts with the least administrative overhead and the broadest service coverage possible using the fewest number of savings plans.

Which combination of savings plans will satisfy these requirements? (Select two)

**Lựa chọn:**

<label for="q363-a"><input type="checkbox" id="q363-a" name="q363" value="A"> <strong>A.</strong> Create a Reserved Instance for each EC2 instance and subscribe to AWS Support to monitor Reserved Instance utilization monthly</label><br>
<label for="q363-b"><input type="checkbox" id="q363-b" name="q363" value="B"> <strong>B.</strong> Subscribe to a hybrid deployment discount plan that includes discounts for both AWS and on-premises Kubernetes workloads</label><br>
<label for="q363-c"><input type="checkbox" id="q363-c" name="q363" value="C"> <strong>C.</strong> Purchase an EC2 Instance Savings Plan that covers EC2 and containerized tasks on Amazon ECS running with Fargate launch type</label><br>
<label for="q363-d"><input type="checkbox" id="q363-d" name="q363" value="D"> <strong>D.</strong> Purchase a Compute Savings Plan that provides cost savings for usage across EC2, Fargate, and Lambda services</label><br>
<label for="q363-e"><input type="checkbox" id="q363-e" name="q363" value="E"> <strong>E.</strong> Purchase a SageMaker Savings Plan that applies discounted pricing to SageMaker training, inference, and notebook instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Purchase a Compute Savings Plan that provides cost savings for usage across EC2, Fargate, and Lambda services

E. Purchase a SageMaker Savings Plan that applies discounted pricing to SageMaker training, inference, and notebook instances

</details>

---

## Câu 364

**Chủ đề:** Design Cost-Optimized Architectures

A big data analytics company is looking to archive the on-premises data into a POSIX compliant file storage system on AWS Cloud. The archived data would be accessed for just about a week in a year.

As a solutions architect, which of the following AWS services would you recommend as the MOST cost-optimal solution?

**Lựa chọn:**

<label for="q364-a"><input type="radio" id="q364-a" name="q364" value="A"> <strong>A.</strong> Amazon EFS Infrequent Access</label><br>
<label for="q364-b"><input type="radio" id="q364-b" name="q364" value="B"> <strong>B.</strong> Amazon EFS Standard</label><br>
<label for="q364-c"><input type="radio" id="q364-c" name="q364" value="C"> <strong>C.</strong> Amazon S3 Standard</label><br>
<label for="q364-d"><input type="radio" id="q364-d" name="q364" value="D"> <strong>D.</strong> Amazon S3 Standard-IA</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Amazon EFS Infrequent Access

</details>

---

## Câu 365

**Chủ đề:** Design Secure Architectures

A global enterprise has onboarded multiple departments into isolated AWS accounts that are part of a unified AWS Organizations structure. Recently, a critical operational alert was missed because it was delivered to the root user’s email address of an account, which is only monitored intermittently. The enterprise wants to redesign its notification handling process to ensure that future communications - categorized by billing, security, and operational relevance - are received promptly by the appropriate teams. The solution should align with AWS security best practices and offer centralized oversight without depending on individual users.

Which solution meets these requirements in the most secure and scalable way?

**Lựa chọn:**

<label for="q365-a"><input type="radio" id="q365-a" name="q365" value="A"> <strong>A.</strong> Configure each AWS account’s root user to use an alias that redirects messages to a centralized mailbox monitored by platform administrators. Then assign alternate contacts for each account using company-managed distribution lists for billing, security, and operations to handle service-specific notifications</label><br>
<label for="q365-b"><input type="radio" id="q365-b" name="q365" value="B"> <strong>B.</strong> Change each AWS account’s root email to a unique departmental email list and configure IAM notification settings to send alerts based on service type. Do not use AWS alternate contacts since notifications are already routed by service in the IAM console</label><br>
<label for="q365-c"><input type="radio" id="q365-c" name="q365" value="C"> <strong>C.</strong> Set up a centralized email forwarding service with rules that inspect notification content and forward emails to the appropriate team based on keywords such as “billing,” “security,” or “operations.” Keep the current root email addresses as they are, and rely on this service to triage alerts</label><br>
<label for="q365-d"><input type="radio" id="q365-d" name="q365" value="D"> <strong>D.</strong> Assign each AWS account’s root user email to a single designated member of the respective department (e.g., security lead or billing analyst). Encourage these individuals to monitor the email accounts regularly. Also configure alternate contacts with the same individual email addresses</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Configure each AWS account’s root user to use an alias that redirects messages to a centralized mailbox monitored by platform administrators. Then assign alternate contacts for each account using company-managed distribution lists for billing, security, and operations to handle service-specific notifications

</details>

---

## Câu 366

**Chủ đề:** Design Secure Architectures

A digital media firm is scaling its cloud footprint and wants to isolate development, testing, and production workloads using separate AWS accounts. It also wants a centralized approach to managing networking infrastructure such as subnets and gateways, without repeating configurations in every account. Additionally, the solution must enforce security best practices—like mandatory logging and guardrails—when new accounts are created. The firm prefers a low-maintenance, governance-driven setup.

Which solution best meets these goals while minimizing operational overhead?

**Lựa chọn:**

<label for="q366-a"><input type="radio" id="q366-a" name="q366" value="A"> <strong>A.</strong> Use AWS Control Tower to create and govern accounts. Deploy a centralized VPC in a shared networking account and share its subnets across workload accounts using AWS Resource Access Manager (AWS RAM)</label><br>
<label for="q366-b"><input type="radio" id="q366-b" name="q366" value="B"> <strong>B.</strong> Use AWS Organizations to create new accounts and a shared networking account with a central VPC. Share the VPC subnets via AWS RAM and rely on service control policies (SCPs) to enforce guardrails manually</label><br>
<label for="q366-c"><input type="radio" id="q366-c" name="q366" value="C"> <strong>C.</strong> Use AWS Control Tower to launch accounts. Deploy separate VPCs in each workload account and centralize security inspection by using Gateway Load Balancers to route traffic through a shared security appliance</label><br>
<label for="q366-d"><input type="radio" id="q366-d" name="q366" value="D"> <strong>D.</strong> Use AWS Service Catalog to define pre-approved VPC templates. Launch one VPC per workload account from the catalog, and enforce networking guardrails using AWS Config conformance packs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use AWS Control Tower to create and govern accounts. Deploy a centralized VPC in a shared networking account and share its subnets across workload accounts using AWS Resource Access Manager (AWS RAM)

</details>

---

## Câu 367

**Chủ đề:** Design High-Performing Architectures

The engineering team at a startup is evaluating the most optimal block storage volume type for the Amazon EC2 instances hosting its flagship application. The storage volume should support very low latency but it does not need to persist the data when the instance terminates. As a solutions architect, you have proposed using Instance Store volumes to meet these requirements.

Which of the following would you identify as the key characteristics of the Instance Store volumes? (Select two)

**Lựa chọn:**

<label for="q367-a"><input type="checkbox" id="q367-a" name="q367" value="A"> <strong>A.</strong> You can't detach an instance store volume from one instance and attach it to a different instance</label><br>
<label for="q367-b"><input type="checkbox" id="q367-b" name="q367" value="B"> <strong>B.</strong> Instance store is reset when you stop or terminate an instance. Instance store data is preserved during hibernation</label><br>
<label for="q367-c"><input type="checkbox" id="q367-c" name="q367" value="C"> <strong>C.</strong> You can specify instance store volumes for an instance when you launch or restart it</label><br>
<label for="q367-d"><input type="checkbox" id="q367-d" name="q367" value="D"> <strong>D.</strong> An instance store is a network storage type</label><br>
<label for="q367-e"><input type="checkbox" id="q367-e" name="q367" value="E"> <strong>E.</strong> If you create an Amazon Machine Image (AMI) from an instance, the data on its instance store volumes isn't preserved</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. You can't detach an instance store volume from one instance and attach it to a different instance

E. If you create an Amazon Machine Image (AMI) from an instance, the data on its instance store volumes isn't preserved

</details>

---

## Câu 368

**Chủ đề:** Design Secure Architectures

A company is deploying a publicly accessible web application. To accomplish this, the engineering team has designed the VPC with a public subnet and a private subnet. The application will be hosted on several Amazon EC2 instances in an Auto Scaling group. The team also wants Transport Layer Security (TLS) termination to be offloaded from the Amazon EC2 instances.

Which solution should a solutions architect implement to address these requirements in the most secure manner?

**Lựa chọn:**

<label for="q368-a"><input type="radio" id="q368-a" name="q368" value="A"> <strong>A.</strong> Set up a Network Load Balancer in the public subnet. Create an Auto Scaling group in the public subnet and associate it with the Network Load Balancer</label><br>
<label for="q368-b"><input type="radio" id="q368-b" name="q368" value="B"> <strong>B.</strong> Set up a Network Load Balancer in the public subnet. Create an Auto Scaling group in the private subnet and associate it with the Network Load Balancer</label><br>
<label for="q368-c"><input type="radio" id="q368-c" name="q368" value="C"> <strong>C.</strong> Set up a Network Load Balancer in the private subnet. Create an Auto Scaling group in the public subnet and associate it with the Network Load Balancer</label><br>
<label for="q368-d"><input type="radio" id="q368-d" name="q368" value="D"> <strong>D.</strong> Set up a Network Load Balancer in the private subnet. Create an Auto Scaling group in the private subnet and associate it with the Network Load Balancer</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Set up a Network Load Balancer in the public subnet. Create an Auto Scaling group in the private subnet and associate it with the Network Load Balancer

</details>

---

## Câu 369

**Chủ đề:** Design Secure Architectures

A company needs an Active Directory service to run directory-aware workloads in the AWS Cloud and it should also support configuring a trust relationship with any existing on-premises Microsoft Active Directory.

Which AWS Directory Service is the best fit for this requirement?

**Lựa chọn:**

<label for="q369-a"><input type="radio" id="q369-a" name="q369" value="A"> <strong>A.</strong> Active Directory Connector</label><br>
<label for="q369-b"><input type="radio" id="q369-b" name="q369" value="B"> <strong>B.</strong> Simple Active Directory (Simple AD)</label><br>
<label for="q369-c"><input type="radio" id="q369-c" name="q369" value="C"> <strong>C.</strong> AWS Transit Gateway</label><br>
<label for="q369-d"><input type="radio" id="q369-d" name="q369" value="D"> <strong>D.</strong> AWS Directory Service for Microsoft Active Directory (AWS Managed Microsoft AD)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. AWS Directory Service for Microsoft Active Directory (AWS Managed Microsoft AD)

</details>

---

## Câu 370

**Chủ đề:** Design Secure Architectures

A global enterprise maintains a hybrid cloud environment and wants to transfer large volumes of data between its on-premises data center and Amazon S3 for backup and analytics workflows. The company has already established a Direct Connect (DX) connection to AWS and wants to ensure high-bandwidth, low-latency, and secure private connectivity without traversing the public internet. The architecture must be designed to access Amazon S3 directly from on-premises systems using this DX connection.

Which configuration should the network engineering team implement to allow direct access to Amazon S3 from the on-premises data center using Direct Connect?

**Lựa chọn:**

<label for="q370-a"><input type="radio" id="q370-a" name="q370" value="A"> <strong>A.</strong> Use a Private Virtual Interface (Private VIF) on the Direct Connect connection and create a VPC endpoint to route traffic to S3 over the private network</label><br>
<label for="q370-b"><input type="radio" id="q370-b" name="q370" value="B"> <strong>B.</strong> Configure a VPN connection over the public internet to AWS and route S3 traffic through the tunnel instead of using Direct Connect</label><br>
<label for="q370-c"><input type="radio" id="q370-c" name="q370" value="C"> <strong>C.</strong> Provision a Public Virtual Interface (Public VIF) on the Direct Connect connection to access Amazon S3 public IP addresses from the on-premises data center</label><br>
<label for="q370-d"><input type="radio" id="q370-d" name="q370" value="D"> <strong>D.</strong> Use a Transit Gateway with Direct Connect Gateway to route on-premises traffic through a VPC and then to Amazon S3 using private IP addressing</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Provision a Public Virtual Interface (Public VIF) on the Direct Connect connection to access Amazon S3 public IP addresses from the on-premises data center

</details>

---

## Câu 371

**Chủ đề:** Design Resilient Architectures

An e-commerce company uses Amazon RDS MySQL DB to store the data. The analytics department at the company runs its reports on the same database. The engineering team has noticed sluggish performance on the database when the analytics reporting process is in progress.

As an AWS Certified Solutions Architect - Associate, which of the following would you suggest as the MOST cost-optimal solution to improve the performance?

**Lựa chọn:**

<label for="q371-a"><input type="radio" id="q371-a" name="q371" value="A"> <strong>A.</strong> Create a read-replica with the same compute capacity and the same storage capacity as the primary. Point the reporting queries to run against the read replica</label><br>
<label for="q371-b"><input type="radio" id="q371-b" name="q371" value="B"> <strong>B.</strong> Create a read-replica with half compute capacity and half storage capacity as the primary. Point the reporting queries to run against the read replica</label><br>
<label for="q371-c"><input type="radio" id="q371-c" name="q371" value="C"> <strong>C.</strong> Create a standby instance in a multi-AZ configuration with the same compute capacity and the same storage capacity as the primary. Point the reporting queries to run against the standby instance</label><br>
<label for="q371-d"><input type="radio" id="q371-d" name="q371" value="D"> <strong>D.</strong> Create a standby instance in a multi-AZ configuration with half compute capacity and half storage capacity as the primary. Point the reporting queries to run against the standby instance</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a read-replica with the same compute capacity and the same storage capacity as the primary. Point the reporting queries to run against the read replica

</details>

---

## Câu 372

**Chủ đề:** Design Resilient Architectures

An e-commerce application uses a relational database that runs several queries that perform joins on multiple tables. The development team has found that these queries are slow and expensive, therefore these are a good candidate for caching. The application needs to use a caching service that supports multi-threading.

As a solutions architect, which of the following services would you recommend for the given use case?

**Lựa chọn:**

<label for="q372-a"><input type="radio" id="q372-a" name="q372" value="A"> <strong>A.</strong> Amazon ElastiCache for Redis</label><br>
<label for="q372-b"><input type="radio" id="q372-b" name="q372" value="B"> <strong>B.</strong> Amazon DynamoDB Accelerator (DAX)</label><br>
<label for="q372-c"><input type="radio" id="q372-c" name="q372" value="C"> <strong>C.</strong> AWS Global Accelerator</label><br>
<label for="q372-d"><input type="radio" id="q372-d" name="q372" value="D"> <strong>D.</strong> Amazon ElastiCache for Memcached</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Amazon ElastiCache for Memcached

</details>

---

## Câu 373

**Chủ đề:** Design High-Performing Architectures

A global logistics provider operates several legacy applications on virtual machines (VMs) within a private data center. Due to accelerated business growth and limited capacity in its existing infrastructure, the provider decides to migrate select applications to AWS. The company opts for a lift-and-shift strategy for its non-mission-critical systems to meet tight migration deadlines. The solution must support rapid migration without requiring extensive application refactoring.

Which combination of actions will best support this migration approach? (Select three)

**Lựa chọn:**

<label for="q373-a"><input type="checkbox" id="q373-a" name="q373" value="A"> <strong>A.</strong> Use AWS CloudEndure Disaster Recovery to continuously replicate the VMs to AWS and then promote the target instances for production use</label><br>
<label for="q373-b"><input type="checkbox" id="q373-b" name="q373" value="B"> <strong>B.</strong> Use Amazon EC2 Auto Scaling to automatically re-create the VMs in AWS by launching replacement instances with matching configurations</label><br>
<label for="q373-c"><input type="checkbox" id="q373-c" name="q373" value="C"> <strong>C.</strong> Use AWS Application Migration Service (MGN). Install the AWS Replication Agent on the source VMs</label><br>
<label for="q373-d"><input type="checkbox" id="q373-d" name="q373" value="D"> <strong>D.</strong> Shut down the source virtual machines and immediately provision EC2 replacement instances using manual AMI creation</label><br>
<label for="q373-e"><input type="checkbox" id="q373-e" name="q373" value="E"> <strong>E.</strong> Perform the initial replication. Launch test instances in AWS to validate the migrated VMs before final cutover</label><br>
<label for="q373-f"><input type="checkbox" id="q373-f" name="q373" value="F"> <strong>F.</strong> Launch a cutover instance after completing testing and confirming that replication is up-to-date</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use AWS Application Migration Service (MGN). Install the AWS Replication Agent on the source VMs

E. Perform the initial replication. Launch test instances in AWS to validate the migrated VMs before final cutover

F. Launch a cutover instance after completing testing and confirming that replication is up-to-date

</details>

---

## Câu 374

**Chủ đề:** Design Resilient Architectures

The engineering team at a retail company is planning to migrate to AWS Cloud from the on-premises data center. The team is evaluating Amazon Relational Database Service (Amazon RDS) as the database tier for its flagship application. The team has hired you as an AWS Certified Solutions Architect Associate to advise on Amazon RDS Multi-AZ capabilities.

Which of the following would you identify as correct for Amazon RDS Multi-AZ? (Select two)

**Lựa chọn:**

<label for="q374-a"><input type="checkbox" id="q374-a" name="q374" value="A"> <strong>A.</strong> To enhance read scalability, a Multi-AZ standby instance can be used to serve read requests</label><br>
<label for="q374-b"><input type="checkbox" id="q374-b" name="q374" value="B"> <strong>B.</strong> Amazon RDS applies operating system updates by performing maintenance on the standby, then promoting the standby to primary and finally performing maintenance on the old primary, which becomes the new standby</label><br>
<label for="q374-c"><input type="checkbox" id="q374-c" name="q374" value="C"> <strong>C.</strong> Amazon RDS automatically initiates a failover to the standby, in case primary database fails for any reason</label><br>
<label for="q374-d"><input type="checkbox" id="q374-d" name="q374" value="D"> <strong>D.</strong> For automated backups, I/O activity is suspended on your primary database since backups are not taken from standby database</label><br>
<label for="q374-e"><input type="checkbox" id="q374-e" name="q374" value="E"> <strong>E.</strong> Updates to your database Instance are asynchronously replicated across the Availability Zone to the standby in order to keep both in sync</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Amazon RDS applies operating system updates by performing maintenance on the standby, then promoting the standby to primary and finally performing maintenance on the old primary, which becomes the new standby

C. Amazon RDS automatically initiates a failover to the standby, in case primary database fails for any reason

</details>

---

## Câu 375

**Chủ đề:** Design Secure Architectures

An edtech startup runs its course-management platform inside a private subnet in a VPC on AWS. The application uses Amazon Cognito user pools for authentication. Now, the team wants to extend the application so that authenticated users can upload and access personal course-related documents in Amazon S3. The solution must ensure scalable, fine-grained and secure access control to the S3 bucket and maintain private network architecture for the application.

Which combination of steps will enable secure S3 integration for this workload? (Select two)

**Lựa chọn:**

<label for="q375-a"><input type="checkbox" id="q375-a" name="q375" value="A"> <strong>A.</strong> Create an Amazon Cognito identity pool to allow federated identities. Use it to generate temporary AWS credentials that grant S3 access when users successfully authenticate</label><br>
<label for="q375-b"><input type="checkbox" id="q375-b" name="q375" value="B"> <strong>B.</strong> Use the existing Amazon Cognito user pool to directly grant users permission to upload and download objects in the S3 bucket</label><br>
<label for="q375-c"><input type="checkbox" id="q375-c" name="q375" value="C"> <strong>C.</strong> Create an Amazon S3 VPC endpoint in the VPC where the application is hosted to enable private connectivity between the application and S3</label><br>
<label for="q375-d"><input type="checkbox" id="q375-d" name="q375" value="D"> <strong>D.</strong> Configure an AWS Lambda function that proxies user uploads to S3. Invoke the Lambda function after each user login to isolate the S3 access</label><br>
<label for="q375-e"><input type="checkbox" id="q375-e" name="q375" value="E"> <strong>E.</strong> Attach an S3 bucket policy that allows access only if requests include a custom HTTP header containing a valid Cognito user ID</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an Amazon Cognito identity pool to allow federated identities. Use it to generate temporary AWS credentials that grant S3 access when users successfully authenticate

C. Create an Amazon S3 VPC endpoint in the VPC where the application is hosted to enable private connectivity between the application and S3

</details>

---

## Câu 376

**Chủ đề:** Design Secure Architectures

A company helps its customers legally sign highly confidential contracts. To meet the strong industry requirements, the company must ensure that the signed contracts are encrypted using the company's proprietary algorithm. The company is now migrating to AWS Cloud using Amazon Simple Storage Service (Amazon S3) and would like you, the solution architect, to advise them on the encryption scheme to adopt.

What do you recommend?

**Lựa chọn:**

<label for="q376-a"><input type="radio" id="q376-a" name="q376" value="A"> <strong>A.</strong> Server-side encryption with Amazon S3 managed keys (SSE-S3)</label><br>
<label for="q376-b"><input type="radio" id="q376-b" name="q376" value="B"> <strong>B.</strong> Server-side encryption with AWS KMS keys (SSE-KMS)</label><br>
<label for="q376-c"><input type="radio" id="q376-c" name="q376" value="C"> <strong>C.</strong> Server-side encryption with customer-provided keys (SSE-C)</label><br>
<label for="q376-d"><input type="radio" id="q376-d" name="q376" value="D"> <strong>D.</strong> Client Side Encryption</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Client Side Encryption

</details>

---

## Câu 377

**Chủ đề:** Design High-Performing Architectures

A retail startup runs a high-traffic order processing system on AWS. The architecture includes a frontend web tier using EC2 instances behind an Application Load Balancer, a processing tier powered by EC2 instances, and a data layer using Amazon DynamoDB. The frontend and processing tiers are decoupled using Amazon SQS. Recently, the engineering team observed that during unpredictable traffic surges, order processing slows down significantly, SQS queue depth increases rapidly, and the processing-tier EC2 instances hit 100% CPU usage.

Which solution will help improve the application’s responsiveness and scalability during peak load periods?

**Lựa chọn:**

<label for="q377-a"><input type="radio" id="q377-a" name="q377" value="A"> <strong>A.</strong> Use Amazon EventBridge to schedule batch processing jobs for the queue. Configure the event rule to invoke EC2-based workers every 10 minutes to process messages in the SQS queue</label><br>
<label for="q377-b"><input type="radio" id="q377-b" name="q377" value="B"> <strong>B.</strong> Add Amazon Kinesis Data Streams to buffer order events from the web tier. Configure the processing tier to consume records from the stream and use enhanced fan-out for high throughput</label><br>
<label for="q377-c"><input type="radio" id="q377-c" name="q377" value="C"> <strong>C.</strong> Use an EC2 Auto Scaling group with a target tracking policy to automatically scale the processing tier. Configure the policy to monitor the ApproximateNumberOfMessages in the SQS queue</label><br>
<label for="q377-d"><input type="radio" id="q377-d" name="q377" value="D"> <strong>D.</strong> Use scheduled Auto Scaling for the processing tier based on past peak periods. Use average CPU utilization to define scaling thresholds</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Use an EC2 Auto Scaling group with a target tracking policy to automatically scale the processing tier. Configure the policy to monitor the ApproximateNumberOfMessages in the SQS queue

</details>

---

## Câu 378

**Chủ đề:** Design Resilient Architectures

A startup wants to create a highly available architecture for its multi-tier application. Currently, the startup manages a single Amazon EC2 instance along with a single Amazon RDS MySQL DB instance. The startup has hired you as an AWS Certified Solutions Architect - Associate to build a solution that meets these requirements while minimizing the underlying infrastructure maintenance effort.

What will you recommend?

**Lựa chọn:**

<label for="q378-a"><input type="radio" id="q378-a" name="q378" value="A"> <strong>A.</strong> Create an Auto-Scaling group with a desired capacity of a total of two Amazon EC2 instances across two Availability Zones. Configure an Application Load Balancer having a target group of these Amazon EC2 instances. Set up a read replica of the Amazon RDS MySQL DB in another Availability Zone</label><br>
<label for="q378-b"><input type="radio" id="q378-b" name="q378" value="B"> <strong>B.</strong> Create an Auto-Scaling group with a desired capacity of a total of two Amazon EC2 instances across two Availability Zones. Configure an Application Load Balancer having a target group of these Amazon EC2 instances. Set up Amazon RDS MySQL DB in a multi-AZ configuration</label><br>
<label for="q378-c"><input type="radio" id="q378-c" name="q378" value="C"> <strong>C.</strong> Create an Auto-Scaling group with a desired capacity of a total of two Amazon EC2 instances in a single Availability Zone. Configure an Application Load Balancer having a target group of these Amazon EC2 instances. Set up Amazon RDS MySQL DB in a multi-AZ configuration</label><br>
<label for="q378-d"><input type="radio" id="q378-d" name="q378" value="D"> <strong>D.</strong> Provision a second Amazon EC2 instance in another Availability Zone. Provision a second Amazon RDS MySQL DB in another Availabililty Zone. Leverage Amazon Route 53 for equal distribution of incoming traffic to the Amazon EC2 instances. Use a custom script to sync data across the two MySQL DBs</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create an Auto-Scaling group with a desired capacity of a total of two Amazon EC2 instances across two Availability Zones. Configure an Application Load Balancer having a target group of these Amazon EC2 instances. Set up Amazon RDS MySQL DB in a multi-AZ configuration

</details>

---

## Câu 379

**Chủ đề:** Design Secure Architectures

As a Solutions Architect, you would like to completely secure the communications between your Amazon CloudFront distribution and your Amazon S3 bucket which contains the static files for your website. Users should only be able to access the Amazon S3 bucket through Amazon CloudFront and not directly.

What do you recommend?

**Lựa chọn:**

<label for="q379-a"><input type="radio" id="q379-a" name="q379" value="A"> <strong>A.</strong> Create a bucket policy to only authorize the IAM role attached to the Amazon CloudFront distribution</label><br>
<label for="q379-b"><input type="radio" id="q379-b" name="q379" value="B"> <strong>B.</strong> Update the Amazon S3 bucket security groups to only allow traffic from the Amazon CloudFront security group</label><br>
<label for="q379-c"><input type="radio" id="q379-c" name="q379" value="C"> <strong>C.</strong> Make the Amazon S3 bucket public</label><br>
<label for="q379-d"><input type="radio" id="q379-d" name="q379" value="D"> <strong>D.</strong> Create an origin access identity (OAI) and update the Amazon S3 Bucket Policy</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

D. Create an origin access identity (OAI) and update the Amazon S3 Bucket Policy

</details>

---

## Câu 380

**Chủ đề:** Design High-Performing Architectures

A media company is modernizing its legacy image processing application by migrating it from an on-premises environment to AWS. The application handles a high volume of image transformation jobs, generating large output files. To support rapid growth, the company wants a cloud-native solution that automatically scales, minimizes manual intervention, and avoids managing servers or infrastructure. The team also wants to improve workflow automation to handle task sequencing and job state transitions.

Which solution best meets these requirements while ensuring the least operational overhead?

**Lựa chọn:**

<label for="q380-a"><input type="radio" id="q380-a" name="q380" value="A"> <strong>A.</strong> Deploy Amazon Elastic Kubernetes Service (Amazon EKS) with self-managed EC2 worker nodes for image processing. Use Amazon SQS to queue jobs and store processed outputs in Amazon EBS volumes</label><br>
<label for="q380-b"><input type="radio" id="q380-b" name="q380" value="B"> <strong>B.</strong> Use AWS Batch to process image jobs. Orchestrate the workflow using AWS Step Functions and store output files in Amazon S3</label><br>
<label for="q380-c"><input type="radio" id="q380-c" name="q380" value="C"> <strong>C.</strong> Use a combination of AWS Lambda functions and EC2 Spot Instances for processing. Store processed images in Amazon FSx</label><br>
<label for="q380-d"><input type="radio" id="q380-d" name="q380" value="D"> <strong>D.</strong> Use Amazon EC2 Auto Scaling groups with a static fleet of instances for image processing. Trigger each job through Step Functions and store results on attached EBS volumes</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Use AWS Batch to process image jobs. Orchestrate the workflow using AWS Step Functions and store output files in Amazon S3

</details>

---

## Câu 381

**Chủ đề:** Design High-Performing Architectures

The systems administrator at a company wants to set up a highly available architecture for a bastion host solution.

As a solutions architect, which of the following options would you recommend as the solution?

**Lựa chọn:**

<label for="q381-a"><input type="radio" id="q381-a" name="q381" value="A"> <strong>A.</strong> Create a public Network Load Balancer that links to Amazon EC2 instances that are bastion hosts managed by an Auto Scaling Group</label><br>
<label for="q381-b"><input type="radio" id="q381-b" name="q381" value="B"> <strong>B.</strong> Create a public Application Load Balancer that links to Amazon EC2 instances that are bastion hosts managed by an Auto Scaling Group</label><br>
<label for="q381-c"><input type="radio" id="q381-c" name="q381" value="C"> <strong>C.</strong> Create a VPC Endpoint for a fleet of Amazon EC2 instances that are bastion hosts managed by an Auto Scaling Group</label><br>
<label for="q381-d"><input type="radio" id="q381-d" name="q381" value="D"> <strong>D.</strong> Create an elastic IP address (EIP) and assign it to all Amazon EC2 instances that are bastion hosts managed by an Auto Scaling Group</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create a public Network Load Balancer that links to Amazon EC2 instances that are bastion hosts managed by an Auto Scaling Group

</details>

---

## Câu 382

**Chủ đề:** Design Resilient Architectures

You are deploying a critical monolith application that must be deployed on a single web server, as it hasn't been created to work in distributed mode. Still, you want to make sure your setup can automatically recover from the failure of an Availability Zone (AZ).

Which of the following options should be combined to form the MOST cost-efficient solution? (Select three)

**Lựa chọn:**

<label for="q382-a"><input type="checkbox" id="q382-a" name="q382" value="A"> <strong>A.</strong> Create an auto-scaling group that spans across 2 Availability Zones, which min=1, max=1, desired=1</label><br>
<label for="q382-b"><input type="checkbox" id="q382-b" name="q382" value="B"> <strong>B.</strong> Assign an Amazon EC2 Instance Role to perform the necessary API calls</label><br>
<label for="q382-c"><input type="checkbox" id="q382-c" name="q382" value="C"> <strong>C.</strong> Create an elastic IP address (EIP) and use the Amazon EC2 user-data script to attach it</label><br>
<label for="q382-d"><input type="checkbox" id="q382-d" name="q382" value="D"> <strong>D.</strong> Create a Spot Fleet request</label><br>
<label for="q382-e"><input type="checkbox" id="q382-e" name="q382" value="E"> <strong>E.</strong> Create an Application Load Balancer and a target group with the instance(s) of the Auto Scaling Group</label><br>
<label for="q382-f"><input type="checkbox" id="q382-f" name="q382" value="F"> <strong>F.</strong> Create an auto-scaling group that spans across 2 Availability Zones, which min=1, max=2, desired=2</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Create an auto-scaling group that spans across 2 Availability Zones, which min=1, max=1, desired=1

B. Assign an Amazon EC2 Instance Role to perform the necessary API calls

C. Create an elastic IP address (EIP) and use the Amazon EC2 user-data script to attach it

</details>

---

## Câu 383

**Chủ đề:** Design High-Performing Architectures

A global photography startup hosts a static image-sharing site on an Amazon S3 bucket. The website allows users from different parts of the world to upload, view, and download photos through their mobile devices. As the platform has gained popularity, users have started experiencing latency issues, especially when uploading and downloading images. The team needs a solution to enhance global performance but wants to implement it with minimal development effort and without redesigning the application.

Which solution will most effectively address the performance issues with the least operational overhead?

**Lựa chọn:**

<label for="q383-a"><input type="radio" id="q383-a" name="q383" value="A"> <strong>A.</strong> Deploy an Amazon CloudFront distribution with the S3 bucket as the origin to improve download speeds. Enable S3 Transfer Acceleration to reduce upload latency for global users</label><br>
<label for="q383-b"><input type="radio" id="q383-b" name="q383" value="B"> <strong>B.</strong> Migrate the website from S3 to Amazon EC2 instances in multiple Regions. Use an Application Load Balancer with AWS Global Accelerator to distribute global traffic and reduce latency</label><br>
<label for="q383-c"><input type="radio" id="q383-c" name="q383" value="C"> <strong>C.</strong> Create multiple S3 buckets in different Regions and replicate image data based on user location. Configure CloudFront to upload and download from the nearest bucket</label><br>
<label for="q383-d"><input type="radio" id="q383-d" name="q383" value="D"> <strong>D.</strong> Enable AWS Global Accelerator on the S3 bucket to accelerate both uploads and downloads. Reconfigure the website to route requests through the accelerator</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Deploy an Amazon CloudFront distribution with the S3 bucket as the origin to improve download speeds. Enable S3 Transfer Acceleration to reduce upload latency for global users

</details>

---

## Câu 384

**Chủ đề:** Design Cost-Optimized Architectures

You have deployed a database technology that has a synchronous replication mode to survive disasters in data centers. The database is therefore deployed on two Amazon EC2 instances in two Availability Zones (AZs). The database must be publicly available so you have deployed the Amazon EC2 instances in public subnets. The replication protocol currently uses the Amazon EC2 public IP addresses.

What can you do to decrease the replication cost?

**Lựa chọn:**

<label for="q384-a"><input type="radio" id="q384-a" name="q384" value="A"> <strong>A.</strong> Use the Amazon EC2 instances private IP for the replication</label><br>
<label for="q384-b"><input type="radio" id="q384-b" name="q384" value="B"> <strong>B.</strong> Assign elastic IP address (EIP) to the Amazon EC2 instances and use them for the replication</label><br>
<label for="q384-c"><input type="radio" id="q384-c" name="q384" value="C"> <strong>C.</strong> Create a Private Link between the two Amazon EC2 instances</label><br>
<label for="q384-d"><input type="radio" id="q384-d" name="q384" value="D"> <strong>D.</strong> Use an Elastic Fabric Adapter (EFA)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use the Amazon EC2 instances private IP for the replication

</details>

---

## Câu 385

**Chủ đề:** Design Secure Architectures

Your application is deployed on Amazon EC2 instances fronted by an Application Load Balancer. Recently, your infrastructure has come under attack. Attackers perform over 100 requests per second, while your normal users only make about 5 requests per second.

How can you efficiently prevent attackers from overwhelming your application?

**Lựa chọn:**

<label for="q385-a"><input type="radio" id="q385-a" name="q385" value="A"> <strong>A.</strong> Use an AWS Web Application Firewall (AWS WAF) and setup a rate-based rule</label><br>
<label for="q385-b"><input type="radio" id="q385-b" name="q385" value="B"> <strong>B.</strong> Use AWS Shield Advanced and setup a rate-based rule</label><br>
<label for="q385-c"><input type="radio" id="q385-c" name="q385" value="C"> <strong>C.</strong> Define a network access control list (network ACL) on your Application Load Balancer</label><br>
<label for="q385-d"><input type="radio" id="q385-d" name="q385" value="D"> <strong>D.</strong> Configure Sticky Sessions on the Application Load Balancer</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use an AWS Web Application Firewall (AWS WAF) and setup a rate-based rule

</details>

---

## Câu 386

**Chủ đề:** Design Resilient Architectures

A company is experiencing stability issues with their cluster of self-managed RabbitMQ message brokers and the company now wants to explore an alternate solution on AWS.

As a solutions architect, which of the following AWS services would you recommend that can provide support for quick and easy migration from RabbitMQ?

**Lựa chọn:**

<label for="q386-a"><input type="radio" id="q386-a" name="q386" value="A"> <strong>A.</strong> Amazon Simple Notification Service (Amazon SNS)</label><br>
<label for="q386-b"><input type="radio" id="q386-b" name="q386" value="B"> <strong>B.</strong> Amazon Simple Queue Service (Amazon SQS) Standard</label><br>
<label for="q386-c"><input type="radio" id="q386-c" name="q386" value="C"> <strong>C.</strong> Amazon MQ</label><br>
<label for="q386-d"><input type="radio" id="q386-d" name="q386" value="D"> <strong>D.</strong> Amazon SQS FIFO (First-In-First-Out)</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Amazon MQ

</details>

---

## Câu 387

**Chủ đề:** Design Resilient Architectures

A digital media streaming company wants to use Amazon CloudFront to distribute its content only to its service subscribers. As a solutions architect, which of the following solutions would you suggest to deliver restricted content to the bona fide end users? (Select two)

**Lựa chọn:**

<label for="q387-a"><input type="checkbox" id="q387-a" name="q387" value="A"> <strong>A.</strong> Use Amazon CloudFront signed URLs</label><br>
<label for="q387-b"><input type="checkbox" id="q387-b" name="q387" value="B"> <strong>B.</strong> Require HTTPS for communication between Amazon CloudFront and your custom origin</label><br>
<label for="q387-c"><input type="checkbox" id="q387-c" name="q387" value="C"> <strong>C.</strong> Require HTTPS for communication between Amazon CloudFront and your S3 origin</label><br>
<label for="q387-d"><input type="checkbox" id="q387-d" name="q387" value="D"> <strong>D.</strong> Forward HTTPS requests to the origin server by using the ECDSA or RSA ciphers</label><br>
<label for="q387-e"><input type="checkbox" id="q387-e" name="q387" value="E"> <strong>E.</strong> Use Amazon CloudFront signed cookies</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

A. Use Amazon CloudFront signed URLs

E. Use Amazon CloudFront signed cookies

</details>

---

## Câu 388

**Chủ đề:** Design Resilient Architectures

The engineering team at an e-commerce company wants to set up a custom domain for internal usage such as internaldomainexample.com. The team wants to use the private hosted zones feature of Amazon Route 53 to accomplish this.

Which of the following settings of the VPC need to be enabled? (Select two)

**Lựa chọn:**

<label for="q388-a"><input type="checkbox" id="q388-a" name="q388" value="A"> <strong>A.</strong> enableVpcSupport</label><br>
<label for="q388-b"><input type="checkbox" id="q388-b" name="q388" value="B"> <strong>B.</strong> enableVpcHostnames</label><br>
<label for="q388-c"><input type="checkbox" id="q388-c" name="q388" value="C"> <strong>C.</strong> enableDnsHostnames</label><br>
<label for="q388-d"><input type="checkbox" id="q388-d" name="q388" value="D"> <strong>D.</strong> enableDnsDomain</label><br>
<label for="q388-e"><input type="checkbox" id="q388-e" name="q388" value="E"> <strong>E.</strong> enableDnsSupport</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. enableDnsHostnames

E. enableDnsSupport

</details>

---

## Câu 389

**Chủ đề:** Design Cost-Optimized Architectures

A healthcare analytics firm operates a backend application within a private subnet of its VPC. The application is fronted by an Application Load Balancer (ALB) and accesses Amazon S3 to store medical reports. The VPC includes both a NAT gateway and an internet gateway, but the company's strict compliance policy prohibits any data traffic from traversing the internet. The team must redesign the architecture to comply with the security policy and improve cost-efficiency.

Which solution best satisfies these requirements in the most cost-effective manner?

**Lựa chọn:**

<label for="q389-a"><input type="radio" id="q389-a" name="q389" value="A"> <strong>A.</strong> Create an S3 interface VPC endpoint and modify the security group to allow access from the application’s private subnet. Route all S3 traffic through the interface endpoint</label><br>
<label for="q389-b"><input type="radio" id="q389-b" name="q389" value="B"> <strong>B.</strong> Modify the S3 bucket policy to allow requests only from the Elastic IP address associated with the NAT gateway</label><br>
<label for="q389-c"><input type="radio" id="q389-c" name="q389" value="C"> <strong>C.</strong> Create a gateway VPC endpoint for Amazon S3 and update the route table for the private subnet to direct S3 traffic through the endpoint</label><br>
<label for="q389-d"><input type="radio" id="q389-d" name="q389" value="D"> <strong>D.</strong> Create a VPC peering connection with another VPC that has direct access to S3. Forward the S3 API requests through the peered VPC using proxy EC2 instances</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

C. Create a gateway VPC endpoint for Amazon S3 and update the route table for the private subnet to direct S3 traffic through the endpoint

</details>

---

## Câu 390

**Chủ đề:** Design Secure Architectures

A company has multiple Amazon EC2 instances operating in a private subnet which is part of a custom VPC. These instances are running an image processing application that needs to access images stored on Amazon S3. Once each image is processed, the status of the corresponding record needs to be marked as completed in a Amazon DynamoDB table.

How would you go about providing private access to these AWS resources which are not part of this custom VPC?

**Lựa chọn:**

<label for="q390-a"><input type="radio" id="q390-a" name="q390" value="A"> <strong>A.</strong> Create a gateway endpoint for Amazon S3 and add it as a target in the route table of the custom VPC. Create an interface endpoint for Amazon DynamoDB and then add it as a target in the route table of the custom VPC</label><br>
<label for="q390-b"><input type="radio" id="q390-b" name="q390" value="B"> <strong>B.</strong> Create a separate gateway endpoint for Amazon S3 and Amazon DynamoDB each. Add two new target entries for these two gateway endpoints in the route table of the custom VPC</label><br>
<label for="q390-c"><input type="radio" id="q390-c" name="q390" value="C"> <strong>C.</strong> Create a gateway endpoint for Amazon DynamoDB and add it as a target in the route table of the custom VPC. Create an Origin Access Identity for Amazon S3 and then connect to the S3 service using the private IP address</label><br>
<label for="q390-d"><input type="radio" id="q390-d" name="q390" value="D"> <strong>D.</strong> Create a separate interface endpoint for Amazon S3 and Amazon DynamoDB each. Then connect to these services by adding these as targets in the route table of the custom VPC</label><br>

<details>
<summary>Kiểm tra đáp án</summary>

**Đáp án đúng:**

B. Create a separate gateway endpoint for Amazon S3 and Amazon DynamoDB each. Add two new target entries for these two gateway endpoints in the route table of the custom VPC

</details>

---
