### In the S3 Intelligent-Tiering storage class, Amazon S3 moves objects between a frequent access tier and an infrequent access tier. Which storage classes are used for these tiers? (Select TWO.)

- **S3 Standard**
- ~~S3 Glacier Deep Archive~~
- **S3 Standard-IA**
- ~~S3 Glacier Flexible Retrieval~~
- ~~S3 One Zone-IA~~

> **Explanation:**
> The two correct response options are:
>
> - **S3 Standard**
> - **S3 Standard-IA**
>
> In the S3 Intelligent-Tiering storage class, Amazon S3 monitors object access patterns. If an object has not been accessed for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, **S3 Standard-IA**. If an object is accessed in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, **S3 Standard**.

---

### Which service provides review details for user activities and API calls that have occurred within an AWS environment?

- ~~Amazon CloudWatch~~
- ~~AWS Trusted Advisor~~
- **AWS CloudTrail**
- ~~Amazon Inspector~~

> **Explanation:**
> The correct response option is **AWS CloudTrail**.
>
> With CloudTrail, a person can view a complete history of user activity and API calls for their applications and resources.
>
> Events are typically updated in CloudTrail within 15 minutes after an API call was made. A person can filter events by specifying the time and date that an API call occurred, the user who requested the action, the type of resource that was involved in the API call, and more.
>
> The other response options are incorrect because:
>
> - Amazon CloudWatch is a service that provides data for monitoring applications, optimizing resource utilization, and responding to system-wide performance changes.
> - Amazon Inspector is a service that checks applications for security vulnerabilities and deviations from security best practices.
> - AWS Trusted Advisor is an online tool that inspects an AWS environment and provides real-time guidance in accordance with AWS best practices.

---

### Which statement best describes an Availability Zone?

- ~~A site that Amazon CloudFront uses to cache copies of content for faster delivery to users at any location~~
- **A fully isolated portion of the AWS global infrastructure**
- ~~A separate geographical location with multiple locations that are isolated from each other~~
- ~~The server from which Amazon CloudFront gets files~~

> **Explanation:**
> The correct response option is **"A fully isolated portion of the AWS global infrastructure."**
>
> An Availability Zone is a single data center or a group of data centers within a Region. Availability Zones are located tens of miles apart from each other. This helps them to provide interconnectivity to support the services and applications that run within a Region.
>
> The other response options are incorrect because:
>
> - A separate geographical location with multiple locations that are isolated from each other: This response option describes a **Region**.
> - The server from which Amazon CloudFront gets files: This response option describes an **origin**.
> - A site that Amazon CloudFront uses to cache copies of content for faster delivery to users at any location: This response option describes an **Edge location**.

---

### Which service is used to transfer up to 100 PB of data to AWS?

- ~~Amazon Neptune~~
- ~~Amazon CloudFront~~
- **AWS Snowmobile**
- ~~AWS DeepRacer~~

> **Explanation:**
> The correct response option is **AWS Snowmobile**.
>
> AWS Snowmobile is a service that is used for transferring up to 100 PB of data to AWS. Each Snowmobile is a 45-foot long shipping container that is pulled by a semi-trailer truck.
>
> The other response options are incorrect because:
>
> - Amazon Neptune is a graph database service. Amazon Neptune provides the capability to build and run applications that work with highly connected datasets, such as recommendation engines, fraud detection, and knowledge graphs.
> - Amazon CloudFront is a content delivery service.
> - AWS DeepRacer is an autonomous 1/18 scale race car that tests reinforcement learning models.

---

### Which pillar of the AWS Well-Architected Framework focuses on using computing resources in ways that meet system requirements?

- ~~Operational Excellence~~
- ~~Security~~
- ~~Reliability~~
- **Performance Efficiency**

> **Explanation:**
> The correct response option is **Performance Efficiency**.
>
> The Performance Efficiency pillar focuses on using computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve.
>
> The other responses are incorrect because:
>
> - The Operational Excellence pillar includes the ability to run workloads effectively, gain insights into their operations, and continuously improve supporting processes to deliver business value.
> - The Security pillar focuses on protecting data, systems, and assets. It also focuses on using cloud technologies to improve the security of your workloads.
> - The Reliability pillar focuses on the ability of a workload to consistently and correctly perform its intended functions.

---

### A cloud engineer is running an Amazon EC2 instance and wants to store data in an attached resource. Their data is temporary and will not be kept long term. Which resource should they use?

- **Instance store**
- ~~Subnet~~
- ~~Amazon S3 bucket~~
- ~~Amazon Elastic Block Store (Amazon EBS) volume~~

> **Explanation:**
> The correct response option is **instance store**.
>
> Instance stores are ideal for temporary data that does not need to be kept long term. When an Amazon EC2 instance is stopped or terminated, all the data that has been written to the attached instance store is deleted.
>
> The other response options are incorrect because:
>
> - Amazon EBS volumes are ideal for data that needs to be retained. When an Amazon EC2 instance is stopped or terminated, all of the data on the attached EBS volume is still available.
> - Amazon S3 buckets cannot be attached to Amazon EC2 instances.
> - A subnet is a section of a virtual private cloud (VPC) in which you can group resources based on security or operational needs.

---

### Which AWS Trusted Advisor category includes checks for high-utilization EC2 instances?

- ~~Security~~
- **Performance**
- ~~Cost Optimization~~
- ~~Fault Tolerance~~

> **Explanation:**
> The correct response option is **Performance**.
>
> In this category, AWS Trusted Advisor also helps improve the performance of services by providing recommendations for how to take advantage of provisioned throughput.
>
> The other response options are incorrect because:
>
> - The Security category includes checks that review permissions and identify which AWS security features to enable.
> - The Cost Optimization category includes checks for unused or idle resources that could be eliminated and provide cost savings.
> - The Fault Tolerance category includes checks to help improve an application's availability and redundancy.

---

### Which Support plans include access to all AWS Trusted Advisor checks? (Select TWO.)

- ~~Basic~~
- **Enterprise**
- **Business**
- ~~Developer~~
- ~~AWS Free Tier~~

> **Explanation:**
> The two correct response options are:
>
> - **Enterprise**
> - **Business**
>
> The other response options are incorrect because:
>
> - The Basic and Developer Support plans provide access to a limited selection of AWS Trusted Advisor checks.
> - The AWS Free Tier is not a Support plan. It is a program that consists of three types of offers that allow customers to use AWS services without incurring costs: Always free, 12 months free, and Trials.

---

### Which statement best describes Elastic Load Balancing?

- **A service that distributes incoming traffic across multiple targets, such as Amazon EC2 instances**
- ~~A service that provides data for monitoring applications, optimize resource utilization, and respond to system-wide performance changes~~
- ~~A service that monitors applications and automatically adds or removes capacity from resource groups in response to changing demand~~
- ~~A service that provides the capability to create, manage, and scale a distributed in-memory or cache environment in the cloud~~

> **Explanation:**
> The correct response option is **"A service that distributes incoming traffic across multiple targets, such as Amazon EC2 instances."**
>
> A load balancer acts as a single point of contact for all incoming web traffic to an Auto Scaling group. This means that as Amazon EC2 instances are added or removed in response to the amount of incoming traffic, these requests are routed to the load balancer first and then spread across multiple resources that will handle them.
>
> The other response options are incorrect because:
>
> - "A service that monitors applications and automatically adds or removes capacity from resource groups in response to changing demand": This response option describes **AWS Auto Scaling**.
> - "A service that provides data for monitoring applications, optimize resource utilization, and respond to system-wide performance changes": This response option describes **Amazon CloudWatch**. Although Elastic Load Balancing does optimize resource utilization by distributing incoming traffic across available resources, this would not be the best response option because Elastic Load Balancing does not provide all the other listed features.
> - "A service that provides the capability to create, manage, and scale a distributed in-memory or cache environment in the cloud": This response option describes **Amazon ElastiCache**.

---

### Which statement is TRUE for AWS Lambda?

- **Businesses pay only for compute time while their code is running.**
- ~~The first step in using AWS Lambda is provisioning a server.~~
- ~~Before using AWS Lambda, a business must prepay for their estimated compute time.~~
- ~~To use AWS Lambda, businesses must configure the servers that run their code.~~

> **Explanation:**
> The correct response option is **"Businesses pay only for compute time while their code is running."**
>
> AWS Lambda is a service that runs code without needing to provision or manage servers. While using AWS Lambda, businesses pay only for the compute time that they consume. They are charged only when their application code is running. With AWS Lambda, they can run code for virtually any type of application or backend service, all with zero administration.

---

### Which Amazon EC2 pricing option reduces costs when a business makes an hourly spend commitment to an instance family and Region for a 1-year or 3-year term?

- **EC2 Instance Savings Plans**
- ~~Spot Instances~~
- ~~Reserved Instances~~
- ~~Dedicated Hosts~~

> **Explanation:**
> The correct response option is **EC2 Instance Savings Plans**.
>
> EC2 Instance Savings Plans reduce compute costs by committing to a consistent hourly spend for a 1-year or 3-year term. This results in savings of up to 72% over On-Demand Instance costs. Any EC2 usage up to the commitment is charged at the discounted Savings Plan rate (for example, $10 an hour). Any EC2 usage beyond the commitment is charged at regular On-Demand Instance rates.
>
> The other response options are incorrect because:
>
> - Reserved Instances are a billing discount that is applied to the use of On-Demand Instances in an AWS account. A business can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term. Unlike EC2 Instance Savings Plans, Reserved Instances do not require an hourly spend commitment over the duration of the contract term.
> - Spot Instances are ideal for workloads with flexible start and end times or that can withstand interruptions. Spot Instances leverage unused EC2 computing capacity and offer cost savings at up to 90% of On-Demand Instance prices.
> - Dedicated Hosts are physical servers with EC2 instance capacity that is fully dedicated to a single customer. A business can use existing per-socket, per-core, or per-VM software licenses to help maintain license compliance. A business can purchase On-Demand Dedicated Hosts or Reserved Dedicated Hosts. Of all the Amazon EC2 options that were covered in this course, Dedicated Hosts are the most expensive.

---

### Which actions can a person perform in Amazon Route 53? (Select TWO.)

- ~~Monitor applications and respond to system-wide performance changes.~~
- ~~Access AWS security and compliance reports and select online agreements.~~
- **Manage DNS records for domain names.**
- **Connect user requests to infrastructure in AWS and outside of AWS.**
- ~~Automate the deployment of workloads into an AWS environment.~~

> **Explanation:**
> The correct two response options are:
>
> - **Connect user requests to infrastructure in AWS and outside of AWS.**
> - **Manage DNS records for domain names.**
>
> Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications that are hosted in AWS.
>
> Additionally, businesses can transfer DNS records for existing domain names that are currently managed by other domain registrars, or register new domain names directly within Amazon Route 53.
>
> The other response options are incorrect because:
>
> - Monitor applications and respond to system-wide performance changes: These actions can be performed in **Amazon CloudWatch**.
> - Access AWS security and compliance reports and select online agreements: This action can be performed in **AWS Artifact**.
> - Automate the deployment of workloads into an AWS environment: This action can be performed with **AWS Quick Starts**.

---

### Which tool provides automation actions for AWS services and applications through scripts?

- ~~AWS Snowball~~
- ~~Amazon Redshift~~
- ~~Amazon QLDB~~
- **AWS Command Line Interface**

> **Explanation:**
> The correct response option is **AWS Command Line Interface**.
>
> The AWS Command Line Interface (AWS CLI) provides the capability to control multiple AWS services directly from the command line within one tool. For example, a person can use commands to start an Amazon EC2 instance, connect an Amazon EC2 instance to a specific Auto Scaling group, and more. The AWS CLI is available for users on Windows, macOS, and Linux.
>
> The other response options are incorrect because:
>
> - Amazon Redshift is a data warehousing service for providing big data analytics. It offers the ability to collect data from many sources and provides insight into relationships and trends across a data set.
> - Amazon Quantum Ledger Database (Amazon QLDB) is a ledger database service. A person can use Amazon QLDB to review a complete history of all the changes that have been made to application data.
> - AWS Snowball is a device that transfers large amounts of data into and out of AWS.

---

### Which tasks are the responsibilities of AWS? (Select TWO.)

- ~~Creating IAM users and groups~~
- **Configuring AWS infrastructure devices**
- ~~Configuring security groups on Amazon EC2 instances~~
- **Maintaining virtualization infrastructure**
- ~~Training company employees on how to use AWS services~~

> **Explanation:**
> The two correct response options are:
>
> - **Maintaining virtualization infrastructure**
> - **Configuring AWS infrastructure devices**
>
> The other three response options are tasks that are the responsibilities of customers.

---

### Which action can a person perform in Amazon CloudFront?

- ~~Provision resources by using programming languages or a text file.~~
- ~~Run infrastructure in a hybrid cloud approach.~~
- ~~Provision an isolated section of the AWS Cloud to launch resources in a virtual network that a person defines.~~
- **Deliver content to customers through a global network of edge locations.**

> **Explanation:**
> The correct response is **"Deliver content to customers through a global network of edge locations."**
>
> Amazon CloudFront is a content delivery service that uses a network of edge locations to cache and deliver content to customers all over the world. When content is cached, it is stored locally as a copy. This content might be video files, photos, webpages, and so on.
>
> The other response options are incorrect because:
>
> - "Run infrastructure in a hybrid cloud approach": This action can be performed with **AWS Outposts**.
> - "Provision resources by using programming languages or a text file": This action can be performed in **AWS CloudFormation**.
> - "Provision an isolated section of the AWS Cloud to launch resources in a virtual network that a person defines": This action can be performed in **Amazon Virtual Private Cloud (Amazon VPC)**.

---

### Which statement best describes AWS Marketplace?

- ~~A resource that provides guidance, architectural reviews, and ongoing communication with companies as they plan, deploy, and optimize their applications~~
- ~~A resource that can answer questions about best practices and assist with troubleshooting issues~~
- **A digital catalog that includes thousands of software listings from independent software vendors**
- ~~An online tool that inspects an AWS environment and provides real-time guidance in accordance with AWS best practices~~

> **Explanation:**
> The correct response option is **"A digital catalog that includes thousands of software listings from independent software vendors."**
>
> Businesses can use AWS Marketplace to find, test, and buy software that runs on AWS.
>
> The other response options are incorrect because:
>
> - "A resource that can answer questions about best practices and assist with troubleshooting issues": This response option describes **AWS Support**.
> - "A resource that provides guidance, architectural reviews, and ongoing communication with companies as they plan, deploy, and optimize their applications": This response option describes a **Technical Account Manager (TAM)**.
> - "An online tool that inspects an AWS environment and provides real-time guidance in accordance with AWS best practices": This response option describes **AWS Trusted Advisor**.

---

### Which component or service establishes a dedicated private connection between an on-premises data center and virtual private cloud (VPC)?

- **AWS Direct Connect**
- ~~Virtual private gateway~~
- ~~Internet gateway~~
- ~~Amazon CloudFront~~

> **Explanation:**
> The correct response option is **AWS Direct Connect**.
>
> AWS Direct Connect is a service that establishes a dedicated private connection between an on-premises data center and VPC. The private connection that AWS Direct Connect provides helps reduce network costs and increase the amount of bandwidth that can travel through a network.
>
> The other response options are incorrect because:
>
> - Amazon CloudFront is a content delivery service. It uses a network of edge locations to cache content and deliver content to customers all over the world.
> - A virtual private gateway establishes a virtual private network (VPN) connection between a VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.
> - An internet gateway is a connection between a VPC and the internet. It allows public traffic from the internet to access a VPC.

---

### Which tool provides the capability to visualize, understand, and manage AWS costs and usage over time?

- ~~AWS Artifact~~
- ~~AWS Pricing Calculator~~
- ~~AWS Budgets~~
- **AWS Cost Explorer**

> **Explanation:**
> The correct response option is **AWS Cost Explorer**.
>
> With AWS Cost Explorer, businesses can quickly create custom reports to analyze their AWS cost and usage data.
>
> The other response options are incorrect because:
>
> - AWS Budgets lets businesses set custom alerts that will notify individuals when a service usage exceeds (or is forecasted to exceed) the amount that has been budgeted.
> - AWS Pricing Calculator creates an estimate for the cost of a business's use cases on AWS. In the AWS Pricing Calculator, a person can enter details for their cloud computing requirements and then receive a detailed estimate that can be exported and shared.
> - AWS Artifact is a service that provides access to AWS security and compliance reports and special online agreements.

---

### Which service runs containerized applications on AWS?

- ~~Amazon Aurora~~
- **Amazon Elastic Kubernetes Service (Amazon EKS)**
- ~~Amazon Redshift~~
- ~~Amazon SageMaker~~

> **Explanation:**
> The correct response option is **Amazon Elastic Kubernetes Service (Amazon EKS)**.
>
> Amazon EKS is a fully managed service that runs Kubernetes on AWS. Kubernetes is open-source software that deploys and manages containerized applications at scale.
>
> Containers provide a standard way to package an application's code and dependencies into a single object. Containers are frequently used for processes and workflows in which there are essential requirements for security, reliability, and scalability.
>
> The other response options are incorrect because:
>
> - Amazon SageMaker is a service that provides the capability to quickly build, train, and deploy machine learning models.
> - Amazon Aurora is an enterprise-class relational database.
> - Amazon Redshift is a data warehousing service for big data analytics.

---

### Which Perspective of the AWS Cloud Adoption Framework focuses on recovering IT workloads to meet the requirements of business stakeholders?

- ~~Governance Perspective~~
- **Operations Perspective**
- ~~People Perspective~~
- ~~Business Perspective~~

> **Explanation:**
> The correct response option is **Operations Perspective**.
>
> The Operations Perspective of the AWS Cloud Adoption Framework also includes principles for operating in the cloud by using agile best practices.
>
> The other response options are incorrect because:
>
> - The Business Perspective helps move a business from a model that separates business and IT strategies into a business model that integrates IT strategy.
> - The People Perspective helps Human Resources (HR) employees prepare their teams for cloud adoption by updating organizational processes and staff skills to include cloud-based competencies.
> - The Governance Perspective provides the capability to update the staff skills and organizational processes that are necessary to ensure business governance in the cloud.

---

### An application developer wants to send and receive messages between distributed application components. Which service should they use?

- **Amazon Simple Queue Service (Amazon SQS)**
- ~~AWS Snowball~~
- ~~Amazon ElastiCache~~
- ~~Amazon Route 53~~

> **Explanation:**
> The correct response option is **Amazon Simple Queue Service (Amazon SQS)**.
>
> Amazon SQS is a message queuing service. Using Amazon SQS, an application developer can send, store, and receive messages between software components at any volume size, without losing messages or requiring other services to be available.
>
> In Amazon SQS, an application sends messages into a queue. A user or service retrieves a message from the queue, processes it, and then deletes it from the queue.
>
> The other response options are incorrect because:
>
> - AWS Snowball is a device that transfers large amounts of data into and out of AWS.
> - Amazon ElastiCache is a service that adds caching layers on top of databases to help improve the read times of common requests.
> - Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications that are hosted in AWS. Additionally, a person can transfer DNS records for existing domain names that are currently managed by other domain registrars or register new domain names directly in Amazon Route 53.

---

### Which virtual private cloud (VPC) component controls inbound and outbound traffic for Amazon EC2 instances?

- ~~Internet gateway~~
- **Security group**
- ~~Subnet~~
- ~~Network access control list~~

> **Explanation:**
> The correct response option is **security group**.
>
> A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance. By default, a security group denies all inbound traffic and allows all outbound traffic. Businesses can add custom rules to configure which traffic should be allowed or denied.
>
> The other response options are incorrect because:
>
> - A subnet is a section of a VPC in which a person can group resources based on security or operational needs.
> - A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the subnet level.
> - An internet gateway is a connection between a VPC and the internet. It allows public traffic from the internet to access a VPC.

---

### Which service builds the workflows that are required for human review of machine learning predictions?

- ~~Amazon Lex~~
- ~~Amazon Aurora~~
- ~~Amazon Textract~~
- **Amazon Augmented AI**

> **Explanation:**
> The correct response option is **Amazon Augmented AI**.
>
> Amazon Augmented AI (Amazon A2I) provides built-in human review workflows for common machine learning use cases, such as content moderation and text extraction from documents. With Amazon A2I, a person can also create their own workflows for machine learning models built on Amazon SageMaker or any other tools.
>
> The other response options are incorrect because:
>
> - Amazon Textract is a machine learning service that automatically extracts text and data from scanned documents.
> - Amazon Lex is a service that builds conversational interfaces using voice and text.
> - Amazon Aurora is an enterprise-class relational database.

---

### Which service consolidates and manages multiple AWS accounts from a central location?

- ~~AWS Identity and Access Management (IAM)~~
- ~~AWS Key Management Service (AWS KMS)~~
- **AWS Organizations**
- ~~AWS Artifact~~

> **Explanation:**
> The correct response option is **AWS Organizations**.
>
> In AWS Organizations, businesses centrally control permissions for their accounts by using service control policies (SCPs). Additionally, businesses can use the consolidated billing feature in AWS Organizations to combine usage and receive a single bill for multiple AWS accounts.
>
> The other response options are incorrect because:
>
> - AWS Identity and Access Management (IAM) is a service that manages access to AWS services and resources.
> - AWS Artifact is a service that provides the capability to access AWS security and compliance reports and special online agreements.
> - AWS Key Management Service (AWS KMS) is a service that creates, manages, and uses cryptographic keys.

---

### Which migration strategy involves changing how an application is architected and developed, typically by using cloud-native features?

- ~~Rehosting~~
- **Refactoring**
- ~~Repurchasing~~
- ~~Replatforming~~

> **Explanation:**
> The correct response option is **Refactoring**.
>
> The other response options are incorrect because:
>
> - Repurchasing involves replacing an existing application with a cloud-based version, such as software found in AWS Marketplace.
> - Rehosting involves moving an application to the cloud with little to no modifications to the application itself. It is also known as “lift and shift.”
> - Replatforming involves selectively optimizing aspects of an application to achieve benefits in the cloud without changing the core architecture of the application. It is also known as “lift, tinker, and shift.”

---

### A cloud architect wants Amazon S3 to monitor object access patterns. Which storage class should they use?

- ~~Amazon S3 Standard-IA~~
- **Amazon S3 Intelligent-Tiering**
- ~~Amazon S3 Glacier Flexible Retrieval~~
- ~~Amazon S3 One Zone-IA~~

> **Explanation:**
> The correct response option is **Amazon S3 Intelligent-Tiering**.
>
> In the Amazon S3 Intelligent-Tiering storage class, Amazon S3 monitors object access patterns. If an object has not been accessed for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, Amazon S3 Standard-IA. If an object is accessed in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, Amazon S3 Standard.
>
> The other response options are incorrect because:
>
> - Amazon S3 Glacier Flexible Retrieval is a low-cost storage class that is ideal for data archiving. A person can retrieve objects stored in the Amazon S3 Glacier Flexible Retrieval storage class within a few minutes to a few hours.
> - The Amazon S3 Standard-IA storage class is ideal for data that is infrequently accessed but requires high availability when needed. Both Amazon S3 Standard and Amazon S3 Standard-IA store data in a minimum of three Availability Zones. Amazon S3 Standard-IA provides the same level of availability as Amazon S3 Standard but at a lower storage price.
> - Amazon S3 One Zone-IA is ideal for infrequently accessed data that does not require high availability.

---

### An application developer wants to store data in a key-value database. Which service should they use?

- **Amazon DynamoDB**
- ~~Amazon DocumentDB~~
- ~~Amazon Aurora~~
- ~~Amazon RDS~~

> **Explanation:**
> The correct response option is **Amazon DynamoDB**.
>
> Amazon DynamoDB is a key-value database service. A key-value database might include data pairs such as “Name: John Doe,” “Address: 123 Any Street,” and “City: Anytown.”
>
> In a key-value database, you can add or remove attributes from items in the table at any time. Additionally, not every item in the table has to have the same attributes.
>
> The other response options are incorrect because:
>
> - Amazon Relational Database Service (Amazon RDS) and Amazon Aurora use structured query language (SQL) to store and query data. They are not key-value databases.
> - Amazon DocumentDB is a document database service that supports MongoDB workloads.

---

### Which statement best describes Amazon GuardDuty?

- ~~A service that helps protect applications against distributed denial-of-service (DDoS) attacks~~
- ~~A service that checks applications for security vulnerabilities and deviations from security best practices~~
- ~~A service that monitors network requests for web applications~~
- **A service that provides intelligent threat detection for AWS infrastructure and resources**

> **Explanation:**
> The correct response option is **"A service that provides intelligent threat detection for your AWS infrastructure and resources."**
>
> AWS GuardDuty identifies threats by continually monitoring the network activity and account behavior within an AWS environment.
>
> The other response options are incorrect because:
>
> - "A service that helps protect applications against distributed denial-of-service (DDoS) attacks": This response option describes **AWS Shield**.
> - "A service that checks applications for security vulnerabilities and deviations from security best practices": This response option describes **Amazon Inspector**.
> - "A service that monitors network requests for web applications": This response option describes **AWS WAF**.

---

### Which service provides the capability to quickly deploy and scale applications on AWS?

- ~~Amazon CloudFront~~
- ~~AWS Snowball~~
- **AWS Elastic Beanstalk**
- ~~AWS Outposts~~

> **Explanation:**
> The correct response option is **AWS Elastic Beanstalk**.
>
> Businesses upload their application, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.
>
> The other response options are incorrect because:
>
> - AWS Outposts is a service that runs infrastructure in a hybrid cloud approach.
> - Amazon CloudFront is a content delivery service.
> - AWS Snowball is a device that transfers large amounts of data into and out of AWS.

---

### A cloud engineer wants to store data in a volume that is attached to an Amazon EC2 instance. Which service should they use?

- **Amazon Elastic Block Store (Amazon EBS)**
- ~~AWS Lambda~~
- ~~Amazon ElastiCache~~
- ~~Amazon Simple Storage Service (Amazon S3)~~

> **Explanation:**
> The correct response option is **Amazon Elastic Block Store (Amazon EBS)**.
>
> Amazon EBS provides block-level storage volumes for Amazon EC2 instances. If a person stops or terminates an Amazon EC2 instance, all the data on the attached EBS volume remains available.
>
> The other response options are incorrect because:
>
> - Amazon Simple Storage Service (Amazon S3) is a service that provides object-level storage. Amazon S3 stores data as objects within buckets.
> - AWS Lambda is a service that runs code without provisioning or managing servers.
> - Amazon ElastiCache is a service that adds caching layers on top of databases to help improve the read times of common requests.
