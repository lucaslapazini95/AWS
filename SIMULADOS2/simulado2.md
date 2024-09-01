## Pergunta 1

### Correto

**Due to regulatory and compliance reasons, an organization is supposed to use a hardware device for any data encryption operations in the cloud. Which AWS service can be used to meet this compliance requirement?**

- AWS Key Management Service (AWS KMS)

**Sua resposta está correta**

- AWS CloudHSM

- AWS Secrets Manager

- AWS Trusted Advisor

### Explicação geral

**Correct option:**

**AWS CloudHSM**

AWS CloudHSM is a cloud-based Hardware Security Module (HSM) that enables you to easily generate and use your encryption keys on the AWS Cloud. With CloudHSM, you can manage your encryption keys using FIPS 140-2 Level 3 validated HSMs. It is a fully-managed service that automates time-consuming administrative tasks for you, such as hardware provisioning, software patching, high-availability, and backups.

Please review this detailed description for CloudHSM: [via AWS CloudHSM](https://aws.amazon.com/cloudhsm/)

**Incorrect options:**

- **AWS Key Management Service (AWS KMS)** - AWS Key Management Service (AWS KMS) makes it easy for you to create and manage cryptographic keys and control their use across a wide range of AWS services and in your applications. It is a secure and resilient service that uses hardware security modules that have been validated under FIPS 140-2, or are in the process of being validated, to protect your keys. It cannot be used as a Hardware Security Module for data encryption operations in AWS Cloud.

- **AWS Secrets Manager** - AWS Secrets Manager helps you protect secrets needed to access your applications, services, and IT resources. The service enables you to easily rotate, manage, and retrieve database credentials, API keys, and other secrets throughout their lifecycle. Users and applications retrieve secrets with a call to Secrets Manager APIs, eliminating the need to hardcode sensitive information in plain text. Secrets Manager cannot be used as a Hardware Security Module for data encryption operations in AWS Cloud.

- **AWS Trusted Advisor** - AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally.

**Reference:**

[https://aws.amazon.com/cloudhsm/](https://aws.amazon.com/cloudhsm/)

**Domínio:**
Security and Compliance

---

## Pergunta 2

### Correto

**Which Amazon Elastic Compute Cloud (Amazon EC2) pricing model is the most cost-effective and flexible with no requirement for a long term resource commitment or upfront payment but still guarantees that instance would not be interrupted?**

- Spot Instance

**Sua resposta está correta**

- On-demand Instance

- Reserved Instance (RI)

- Dedicated Host

### Explicação geral

**Correct option:**

**On-demand Instance** - An On-Demand Instance is an instance that you use on-demand. You have full control over its lifecycle — you decide when to launch, stop, hibernate, start, reboot, or terminate it. There is no long-term commitment required when you purchase On-Demand Instances. There is no upfront payment and you pay only for the seconds that your On-Demand Instances are running. The price per second for running an On-Demand Instance is fixed. On-demand instances cannot be interrupted.

**EC2 Pricing Options Overview:** [via EC2 Pricing](https://aws.amazon.com/ec2/pricing/)

**Incorrect options:**

- **Reserved Instance (RI)** - Reserved Instance (RI) provides you with significant savings on your Amazon EC2 costs compared to On-Demand Instance pricing. Reserved Instances (RI) are not physical instances, but rather a billing discount applied to the use of On-Demand Instances in your account. You can purchase a Reserved Instance (RI) for a one-year or three-year commitment, with the three-year commitment offering a bigger discount. You will be charged for the entire duration, irrespective of your usage. So this option is not correct for the given use-case.

- **Spot Instance** - A Spot Instance is an unused EC2 instance that is available for less than the On-Demand price. Because Spot Instances enable you to request unused EC2 instances at steep discounts, you can lower your Amazon EC2 costs significantly. Spot Instances are well-suited for data analysis, batch jobs, background processing, and optional tasks. These can be terminated at short notice, so these are not suitable for critical workloads that need to run at a specific point in time. So this option is not correct for the given use-case.

- **Dedicated Host** - Amazon EC2 Dedicated Host allows you to use your eligible software licenses from vendors such as Microsoft and Oracle on Amazon EC2 so that you get the flexibility and cost-effectiveness of using your licenses, but with the resiliency, simplicity, and elasticity of AWS. An Amazon EC2 Dedicated Host is a physical server fully dedicated for your use, so you can help address corporate compliance requirement. A Dedicated Host is not cost-efficient compared to an On-Demand instance. So this option is not correct.

**Reference:**

[https://aws.amazon.com/ec2/pricing/](https://aws.amazon.com/ec2/pricing/)

**Domínio:**
Billing and Pricing

---

## Pergunta 3

### Correto

**Which characteristic of Cloud Computing imparts the ability to acquire resources as you need and release when you no longer need them?**

- Durability

**Sua resposta está correta**

- Elasticity

- Reliability

- Resiliency

### Explicação geral

**Correct option:**

**Elasticity**

The ability to acquire resources as you need and release when they are no longer needed is termed as Elasticity of the Cloud. With cloud computing, you don’t have to over-provision resources upfront to handle peak levels of business activity in the future. Instead, you provision the number of resources that you need. You can scale these resources up or down instantly to grow and shrink capacity as your business needs change.

**What is Elasticity:** [via What is Cloud Computing](https://aws.amazon.com/what-is-cloud-computing/)

**Incorrect options:**

- **Reliability** - Refers to the ability of a system to recover from infrastructure or service disruptions, by dynamically acquiring computing resources to meet demand, and mitigate disruptions.

- **Durability** - Refers to the ability of a system to assure data is stored and data remains consistently on the system as long as it is not changed by legitimate access, i.e. data should not get corrupt or disappear from the cloud because of a system malfunction.

- **Resiliency** - Describes the ability of a system to recover from a failure induced by the load (data or network), attacks, and failures (hardware, software, or network failures).

**References:**

- [https://aws.amazon.com/what-is-cloud-computing/](https://aws.amazon.com/what-is-cloud-computing/)
- [https://wa.aws.amazon.com/wat.concept.elasticity.en.html](https://wa.aws.amazon.com/wat.concept.elasticity.en.html)

**Domínio:**
Cloud Concepts

---

## Pergunta 4

### Correto

**Access Key ID and Secret Access Key are tied to which of the following AWS Identity and Access Management (AWS IAM) entities?**

- IAM Role

- IAM Policy

**Sua resposta está correta**

- IAM User

- IAM User Group

### Explicação geral

**Correct option:**

**IAM User**

Access keys are long-term credentials for an IAM user or the AWS account root user. You can use access keys to sign programmatic requests to the AWS CLI or AWS API (directly or using the AWS SDK). Access keys consist of two parts: an access key ID (for example, AKIAIOSFODNN7EXAMPLE) and a secret access key (for example, wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY). As a user name and password, you must use both the access key ID and secret access key together to authenticate your requests. Access Keys are secret, just like a password. You should never share them.

**Incorrect options:**

- **IAM Role** - An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS. However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone who needs it.

- **IAM User Group** - An IAM User Group is a collection of IAM users. Groups let you specify permissions for multiple users, which can make it easier to manage the permissions for those users.

- **IAM Policy** - You manage access in AWS by creating policies and attaching them to IAM identities (users, groups of users, or roles) or AWS resources. A policy is an object in AWS that, when associated with an identity or resource, defines their permissions.

Access keys are not tied to the IAM role, IAM group, or AWS policy. So all three options are incorrect.

**Reference:**

[https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html)

**Domínio:**
Security and Compliance

---

## Pergunta 5

### Correto

**The engineering team at an IT company wants to monitor the CPU utilization for its fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances and send an email to the administrator if the utilization exceeds 80%. As a Cloud Practitioner, which AWS services would you recommend to build this solution? (Select two)**

- AWS CloudTrail

- Amazon Simple Queue Service (SQS)

- Amazon Simple Notification Service (SNS)

- Amazon CloudWatch

- AWS Lambda

### Explicação geral

**Correct options:**

- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. You can create an CloudWatch alarm that sends an email message using Amazon SNS when the alarm changes state from OK to ALARM. The alarm changes to the ALARM state when the average CPU use of an EC2 instance exceeds a specified threshold for consecutive specified periods.

- **Amazon Simple Notification Service (SNS)** - Amazon Simple Notification Service (SNS) is a highly available, durable, secure, fully managed pub/sub messaging service that enables you to decouple microservices, distributed systems, and serverless applications.

**How SNS Works:** [via SNS](https://aws.amazon.com/sns/)

**Incorrect options:**

- **AWS CloudTrail** - AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. Think account-specific activity and audit; think CloudTrail. CloudTrail cannot be used to monitor CPU utilization for EC2 instances or send emails.

- **AWS Lambda** - AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume. Lambda cannot be used to monitor CPU utilization for EC2 instances or send emails.

- **Amazon Simple Queue Service (SQS)** - Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. SQS offers two types of message queues - Standard queues vs FIFO queues. SQS cannot be used to monitor CPU utilization for EC2 instances or send emails.

**References:**

- [https://aws.amazon.com/cloudwatch/](https://aws.amazon.com/cloudwatch/)
- [https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/US_AlarmAtThresholdEC2.html](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/US_AlarmAtThresholdEC2.html)

**Domínio:**
Technology

---

## Pergunta 6

### Correto

**An IT company wants to run a log backup process every Monday at 2 AM. The usual runtime of the process is 5 minutes. As a Cloud Practitioner, which AWS services would you recommend to build a serverless solution for this use-case? (Select two)**

- AWS Lambda

- Amazon Eventbridge

- AWS Systems Manager

- Amazon Elastic Compute Cloud (Amazon EC2)

- AWS Step Function

### Explicação geral

**Correct option:**

- **Amazon Eventbridge** - Amazon EventBridge is a service that provides real-time access to changes in data in AWS services, your own applications, and software as a service (SaaS) applications without writing code. Amazon EventBridge Scheduler is a serverless task scheduler that simplifies creating, executing, and managing millions of schedules across AWS services without provisioning or managing underlying infrastructure.

**Amazon Eventbridge Scheduler:** [via Eventbridge](https://aws.amazon.com/eventbridge/)

- **AWS Lambda** - AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume. The lambda has a maximum execution time of 15 minutes, so it can be used to run this log backup process.

To build the solution for the given use-case, you can leverage the Amazon EventBridge Scheduler to trigger on a schedule. You can then set the Lambda as the target for this rule.

**Incorrect options:**

- **AWS Systems Manager** - AWS Systems Manager gives you visibility and control of your infrastructure on AWS. Systems Manager provides a unified user interface so you can view operational data from multiple AWS services and allows you to automate operational tasks across your AWS resources. With Systems Manager, you can group resources, like Amazon EC2 instances, Amazon S3 buckets, or Amazon RDS instances, by application, view operational data for monitoring and troubleshooting, and take action on your groups of resources. Secrets Manager cannot be used to run a process on a schedule.

- **Amazon Elastic Compute Cloud (Amazon EC2)** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud with support for per-second billing. It is the easiest way to provision servers on AWS Cloud and access the underlying OS. As the company wants a serverless solution, so this option is ruled out.

- **AWS Step Function** - AWS Step Function lets you coordinate multiple AWS services into serverless workflows. You can design and run workflows that stitch together services such as AWS Lambda, AWS Glue and Amazon SageMaker. Step Function cannot be used to run a process on a schedule.

**Reference:**

[https://aws.amazon.com/eventbridge/](https://aws.amazon.com/eventbridge/)

**Domínio:**
Technology

---

## Pergunta 7

### Correto

**A company is using a message broker service on its on-premises application and wants to move this messaging functionality to AWS Cloud. Which of the following AWS services is the right choice to move the existing functionality easily?**

- Amazon Kinesis Data Streams

- Amazon Simple Notification Service (Amazon SNS)

- Amazon Simple Queue Service (Amazon SQS)

**Sua resposta está correta**

- Amazon MQ

### Explicação geral

**Correct option:**

**Amazon MQ**

Amazon MQ is a managed message broker service for Apache ActiveMQ and RabbitMQ that makes it easy to set up and operate message brokers on AWS. Amazon MQ reduces your operational responsibilities by managing the provisioning, setup, and maintenance of message brokers for you. Because Amazon MQ connects to your current applications with industry-standard APIs and protocols, you can easily migrate to AWS without having to rewrite code.

If you're using messaging with existing applications, and want to move the messaging functionality to the cloud quickly and easily, AWS recommends you consider Amazon MQ. It supports industry-standard APIs and protocols so you can switch from any standards-based message broker to Amazon MQ without rewriting the messaging code in your applications. If you are building brand new applications in the cloud, AWS recommends you consider Amazon SQS and Amazon SNS.

**How Amazon MQ works:** [via Amazon MQ](https://aws.amazon.com/amazon-mq/)

**Incorrect options:**

- **Amazon Simple Queue Service (Amazon SQS)** - Amazon Simple Queue Service (Amazon SQS) offers a reliable, highly scalable hosted queue for storing messages as they travel between computers. Amazon SQS lets you easily move data between distributed application components and helps you build applications in which messages are processed independently (with message-level ack/fail semantics), such as automated workflows.

- **Amazon Simple Notification Service (Amazon SNS)** - Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication. The A2A pub/sub functionality provides topics for high-throughput, push-based, many-to-many messaging between distributed systems, microservices, and event-driven serverless applications. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, which implies that the receiving applications have to be present and running to receive the messages.

- **Amazon Kinesis Data Streams** - Amazon Kinesis Data Streams enables you to build custom applications that process or analyze streaming data for specialized needs. You can continuously add various types of data such as clickstreams, application logs, and social media to an Amazon Kinesis data stream from hundreds of thousands of sources. Within seconds, the data will be available for your Amazon Kinesis Applications to read and process from the stream.

**Reference:**

[https://aws.amazon.com/amazon-mq/faqs/](https://aws.amazon.com/amazon-mq/faqs/)

**Domínio:**
Technology

---

## Pergunta 8

### Correto

**The AWS Well-Architected Framework provides guidance on building cloud based applications using AWS best practices. Which of the following options are the pillars mentioned in the AWS Well-Architected Framework? (Select two)**

- Cost Optimization

- Elasticity

- Scalability

- Availability

- Reliability

### Explicação geral

**Correct options:**

- **Reliability**

- **Cost Optimization**

The AWS Well-Architected Framework provides guidance on building secure, high-performing, resilient, and efficient infrastructure for cloud based applications. Based on six pillars — operational excellence, security, reliability, performance efficiency, cost optimization and sustainability — the Framework provides a consistent approach for customers and partners to evaluate architectures, and implement designs that will scale over time.

**Incorrect options:**

- **Elasticity** - Elasticity is the ability to acquire resources as you need them and release resources when you no longer need them. In the cloud, you want to do this automatically.

- **Availability** - A system that is available is capable of delivering the designed functionality at a given point in time. Highly available systems are those that can withstand some measure of degradation while still remaining available.

- **Scalability** - A measurement of a system's ability to grow to accommodate an increase in demand.

These three options are not part of the AWS Well-Architected Framework.

**Reference:**

[https://d1.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf](https://d1.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf)

**Domínio:**
Cloud Concepts

---

## Pergunta 9

### Correto

**An online gaming company wants to block users from certain geographies from accessing its content. Which AWS service can be used to accomplish this task?**

- AWS Shield

**Sua resposta está correta**

- AWS Web Application Firewall (AWS WAF)

- Security group

- Amazon CloudWatch

### Explicação geral

**Correct option:**

**AWS Web Application Firewall (AWS WAF)**

AWS Web Application Firewall (AWS WAF) is a web application firewall that helps protect web applications from attacks by allowing you to configure rules that allow, block, or monitor (count) web requests based on conditions that you define. These conditions include IP addresses, HTTP headers, HTTP body, URI strings, SQL injection, and cross-site scripting. You can use the IP address based match rule to block specific geographies. The accuracy of the IP Address to country lookup database varies by Region. Based on recent tests, AWS mentions that the overall accuracy for the IP address to country mapping is 99.8%.

**How AWS Web Application Firewall (AWS WAF) Works:** [via AWS WAF](https://aws.amazon.com/waf/)

**Incorrect options:**

- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. Amazon CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. This is an excellent service for building Resilient systems. Think resource performance monitoring, events, and alerts; think CloudWatch. Amazon CloudWatch cannot be used to block users from certain geographies.

- **AWS Shield** - AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS. AWS Shield provides always-on detection and automatic inline mitigations that minimize application downtime and latency, so there is no need to engage AWS Support to benefit from DDoS protection. AWS Shield cannot be used to block users from certain geographies.

- **Security group** - A security group acts as a virtual firewall for your EC2 instances to control incoming and outgoing traffic. Inbound rules control the incoming traffic to your instance, and outbound rules control the outgoing traffic from your instance. Security groups only have "allow" rules. You cannot use the security groups to block users from certain geographies.

**Reference:**

[https://aws.amazon.com/waf/faqs/](https://aws.amazon.com/waf/faqs/)

**Domínio:**
Technology

---

## Pergunta 10

### Correto

**Which Amazon Route 53 routing policy would you use to improve the performance for your customers by routing the requests to the AWS endpoint that provides the fastest experience?**

- Simple routing

**Sua resposta está correta**

- Latency-based routing

- Failover routing

- Weighted routing

### Explicação geral

**Correct option:**

**Latency-based routing**

Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect to each other.

If your application is hosted in multiple AWS Regions, you can use latency-based routing policy to improve the performance for your users by serving their requests from the AWS Region that provides the lowest latency. To use latency-based routing, you create latency records for your resources in multiple AWS Regions. When Amazon Route 53 receives a DNS query for your domain or subdomain (example.com or acme.example.com), it determines which AWS Regions you've created latency records for, determines which region gives the user the lowest latency, and then selects a latency record for that region. Amazon Route 53 responds with the value from the selected record, such as the IP address for a web server.

**Amazon Route 53 Routing Policy Overview:** [via Route53](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html)

**Incorrect options:**

- **Failover routing** - This routing policy is used when you want to configure active-passive failover.

- **Weighted routing** - This routing policy is used to route traffic to multiple resources in proportions that you specify.

- **Simple routing** - With simple routing, you typically route traffic to a single resource, for example, to a web server for your website.

**Reference:**

[https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html)

**Domínio:**
Technology

## Pergunta 11

### Correto

**A social media company wants to protect its web application from common web exploits such as SQL injection and cross-site scripting. Which of the following AWS services can be used to address this use-case?**

- AWS CloudWatch

**Sua resposta está correta**

- AWS Web Application Firewall (AWS WAF)

- Amazon Inspector

- Amazon GuardDuty

### Explicação geral

**Correct option:**

**AWS Web Application Firewall (AWS WAF)**

AWS Web Application Firewall (AWS WAF) is a web application firewall that helps protect your web applications or APIs against common web exploits that may affect availability, compromise security, or consume excessive resources. AWS Web Application Firewall (AWS WAF) gives you control over how traffic reaches your applications by enabling you to create security rules that block common attack patterns such as SQL injection or cross-site scripting. You can also use rate-based rules to mitigate the Web layer DDoS attack.

**How AWS Web Application Firewall (AWS WAF) Works:** [via AWS WAF](https://aws.amazon.com/waf/)

An SQL injection attack works by exploiting any one of the known SQL vulnerabilities that allow the SQL server to run malicious code. For example, if a SQL server is vulnerable to an injection attack, it may be possible for an attacker to go to a website's search box and type in code that would force the site's SQL server to dump all of its stored usernames and passwords for the site.

Similar to an SQL injection attack, a cross-site scripting attack also involves injecting malicious code into a website, but in this case, the website itself is not being attacked. Instead, the malicious code the attacker has injected only runs in the user's browser when they visit the attacked website, and it goes after the visitor directly, not the website.

**Incorrect options:**

- **Amazon GuardDuty** - Amazon GuardDuty is a threat detection service that monitors malicious activity and unauthorized behavior to protect your AWS account. Amazon GuardDuty analyzes billions of events across your AWS accounts from AWS CloudTrail (AWS user and API activity in your accounts), Amazon VPC Flow Logs (network traffic data), and DNS Logs (name query patterns). Amazon GuardDuty cannot be used to protect from web exploits such as SQL injection and cross-site scripting.

**How Amazon GuardDuty Works:** [via Amazon GuardDuty](https://aws.amazon.com/guardduty/)

- **Amazon Inspector** - Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. Amazon Inspector cannot be used to protect from web exploits such as SQL injection and cross-site scripting.

- **AWS CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. This is an excellent service for building Resilient systems. Think resource performance monitoring, events, and alerts; think CloudWatch. CloudWatch cannot be used to protect from web exploits such as SQL injection and cross-site scripting.

**Reference:**

[https://aws.amazon.com/waf/](https://aws.amazon.com/waf/)

**Domínio:**
Security and Compliance

---

## Pergunta 12

### Correto

**Which AWS compute service provides the EASIEST way to access resizable compute capacity in the cloud with support for per-second billing and access to the underlying OS?**

- Amazon Lightsail

- Amazon Elastic Container Service (Amazon ECS)

- AWS Lambda

**Sua resposta está correta**

- Amazon Elastic Compute Cloud (Amazon EC2)

### Explicação geral

**Correct option:**

**Amazon Elastic Compute Cloud (Amazon EC2)**

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud with support for per-second billing. It is the easiest way to provision servers on AWS Cloud and access the underlying OS. Amazon EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change.

**Amazon Elastic Compute Cloud (Amazon EC2) Overview:** [via Amazon EC2](https://aws.amazon.com/ec2/)

**Incorrect options:**

- **Amazon Elastic Container Service (Amazon ECS)** - Amazon Elastic Container Service (Amazon ECS) is a highly scalable, high-performance container management service that supports Docker containers and allows you to easily run applications on a managed cluster of Amazon EC2 instances. Technically, you can access the underlying EC2 instances, but the setup is more complex than just using the EC2 service directly, so this option is ruled out.

**How Amazon Elastic Container Service (Amazon ECS) Works:** [via Amazon ECS](https://aws.amazon.com/ecs/)

- **AWS Lambda** - AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume. AWS Lambda is serverless, so you don't get access to the underlying OS.

- **Amazon Lightsail** - Amazon Lightsail is an easy-to-use cloud platform that offers you everything needed to build an application or website, plus a cost-effective, monthly plan. Amazon Lightsail offers several preconfigured, one-click-to-launch operating systems, development stacks, and web applications, including Linux, Windows OS, and WordPress. Amazon Lightsail comes with monthly payment plans and does not support per second billing, so this option is ruled out.

**Reference:**

[https://aws.amazon.com/ec2/](https://aws.amazon.com/ec2/)

**Domínio:**
Technology

---

## Pergunta 13

### Correto

**Which service gives a personalized view of the status of the AWS services that are part of your Cloud architecture so that you can quickly assess the impact on your business when AWS service(s) are experiencing issues?**

- Amazon Inspector

- AWS Health - Service Health Dashboard

- Amazon CloudWatch

**Sua resposta está correta**

- AWS Health - Your Account Health Dashboard

### Explicação geral

**Correct option:**

**AWS Health - Your Account Health Dashboard**

AWS Health - Your Account Health Dashboard provides alerts and remediation guidance when AWS is experiencing events that may impact you.

With AWS Health - Your Account Health Dashboard, alerts are triggered by changes in the health of your AWS resources, giving you event visibility, and guidance to help quickly diagnose and resolve issues.

You can check on this page [https://phd.aws.amazon.com/phd/home](https://phd.aws.amazon.com/phd/home) to get current status information.

**Incorrect options:**

- **Amazon Inspector** - Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. Amazon Inspector cannot be used to prevent Distributed Denial-of-Service (DDoS) attack. It cannot provide the status of your AWS resources.

- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. This is an excellent service for building Resilient systems. Think resource performance monitoring, events, and alerts; think CloudWatch. It cannot provide the status of your AWS resources.

- **AWS Health - Service Health Dashboard** - The AWS Health - Service Health Dashboard is the single place to learn about the availability and operations of AWS services. You can view the overall status of AWS services, and you can sign in to view personalized communications about your particular AWS account or organization.

You can check on this page [https://health.aws.amazon.com/health/status](https://health.aws.amazon.com/health/status) to get current status information.

**Exam Alert:**

While the AWS Health - Service Health Dashboard displays the general status of AWS services; the AWS Health - Your Account Health Dashboard gives you a personalized view of the performance and availability of the AWS services underlying your AWS resources.

**Reference:**

[https://docs.aws.amazon.com/health/latest/ug/what-is-aws-health.html](https://docs.aws.amazon.com/health/latest/ug/what-is-aws-health.html)

**Domínio:**
Cloud Concepts

---

## Pergunta 14

### Incorreto

**Which of the following options can be used to access and manage all AWS services (Select three)?**

**Sua seleção está correta**

- AWS Management Console

**Seleção correta**

- AWS Command Line Interface (AWS CLI)

- Amazon API Gateway

**Sua seleção está incorreta**

- AWS Systems Manager

- AWS Secrets Manager

**Sua seleção está correta**

- AWS Software Development Kit (SDK)

### Explicação geral

**Correct options:**

AWS services can be accessed in three different ways:

- **AWS Management Console**

This is a simple web interface for accessing AWS services.

- **AWS Command Line Interface (AWS CLI)**

You can access AWS services from the command line and automate service management with scripts.

- **AWS Software Development Kit (SDK)**

You can also access via AWS SDK that provides language-specific abstracted APIs for AWS services.

**Incorrect options:**

- **AWS Systems Manager** - AWS Systems Manager gives you visibility and control of your infrastructure on AWS. AWS Systems Manager provides a unified user interface so you can view operational data from multiple AWS services and allows you to automate operational tasks across your AWS resources. With AWS Systems Manager, you can group resources, like Amazon EC2 instances, Amazon S3 buckets, or Amazon RDS instances, by application, view operational data for monitoring and troubleshooting, and take action on your groups of resources.

- **AWS Secrets Manager** - AWS Secrets Manager helps you protect secrets needed to access your applications, services, and IT resources. The service enables you to easily rotate, manage, and retrieve database credentials, API keys, and other secrets throughout their lifecycle. Users and applications retrieve secrets with a call to AWS Secrets Manager APIs, eliminating the need to hardcode sensitive information in plain text.

- **Amazon API Gateway** - Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.

**Domínio:**
Technology

---

## Pergunta 15

### Correto

**Which AWS service publishes up-to-the-minute information on the general status and availability of all AWS services in all the Regions of AWS Cloud?**

**Sua resposta está correta**

- AWS Health Dashboard - service health

- AWS Health Dashboard – Your account health

- Amazon CloudWatch

- AWS CloudFormation

### Explicação geral

**Correct option:**

**AWS Health Dashboard - service health**

AWS Health Dashboard - service health is the single place to learn about the availability and operations of AWS services. You can view the overall status of AWS services, and you can sign in to view personalized communications about your particular AWS account or organization.

You can check on this page [https://health.aws.amazon.com/health/status](https://health.aws.amazon.com/health/status) to get current status information.

**Incorrect options:**

- **AWS CloudFormation** - AWS CloudFormation allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all Regions and accounts. Think infrastructure as code; think CloudFormation. CloudFormation does not provide the general status of AWS services availability for all Regions.

- **AWS Health Dashboard – Your account health** - AWS Health Dashboard – Your account health provides alerts and remediation guidance when AWS is experiencing events that may impact you.

**Exam Alert:**

While the AWS Health Dashboard - service health displays the general status of AWS services; the AWS Health Dashboard – Your account health gives you a personalized view of the performance and availability of the AWS services underlying your AWS resources.

- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. This is an excellent service for building Resilient systems. Think resource performance monitoring, events, and alerts; think CloudWatch. CloudWatch does not provide the general status of AWS services availability for all Regions.

**Reference:**

[https://status.aws.amazon.com/](https://status.aws.amazon.com/)

**Domínio:**
Cloud Concepts

---

## Pergunta 16

### Correto

**Which of the following statement is correct regarding the AWS pricing policy for data transfer charges into or out of an AWS Region?**

**Sua resposta está correta**

- Only outbound data transfer is charged

- Only inbound data transfer is charged

- Neither inbound nor outbound data transfer are charged

- Both inbound data transfer and outbound data transfer are charged

### Explicação geral

**Correct option:**

**Only outbound data transfer is charged**

One of the main benefits of cloud services is the ability it gives you to optimize costs to match your needs, even as those needs change. AWS services do not have complex dependencies or licensing requirements, so you can get exactly what you need to build innovative, cost-effective solutions using the latest technology.

There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer. These characteristics vary somewhat, depending on the AWS product and pricing model you choose. Outbound data to the internet from all AWS regions is billed at region-specific, tiered data transfer rates. Inbound data transfer into all AWS regions from the internet is free.

**Incorrect options:**

- Only inbound data transfer is charged
- Both inbound data transfer and outbound data transfer are charged
- Neither inbound nor outbound data transfer are charged

These three options contradict the explanation provided above, so these options are incorrect.

**Reference:**

[https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf](https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf)

**Domínio:**
Billing and Pricing

---

## Pergunta 17

### Correto

**Which of the following statements are correct about the AWS root user account? (Select two)**

**Sua seleção está correta**

- It is highly recommended to enable Multi-Factor Authentication (MFA) for root user account

**Sua seleção está correta**

- Root user access credentials are the email address and password used to create the AWS account

- Root user credentials should only be shared with managers requiring administrative responsibilities to complete their jobs

- Root user account password cannot be changed once it is set

- Root user account gets unrestricted permissions when the account is created, but these can be restricted using IAM policies

### Explicação geral

**Correct options:**

- **Root user access credentials are the email address and password used to create the AWS account**

- **It is highly recommended to enable Multi-Factor Authentication (MFA) for root user account**

The Email address and the password used for signing up for AWS services are the AWS root user account credentials. Root user account, therefore, has full permissions on all AWS resources under that account. Restricting root user account access is not possible. As a best practice, Multi-Factor Authentication (MFA) should be set on the root user account. The root user account password can be changed after account creation. For all employees performing various administrative jobs, create individual user accounts using AWS IAM, and give administrative permissions as needed.

**AWS Root User Account Security Best Practices:**

- [via IAM User Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html)
- [via IAM Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#lock-away-credentials)

**Incorrect options:**

- **Root user account password cannot be changed once it is set** - This is incorrect. Like any other user credentials, the root user password can be changed after creation.

- **Root user credentials should only be shared with managers requiring administrative responsibilities to complete their jobs** - This is a dangerous practice. Root user credentials should only be used only for some limited account-specific activity and root user credentials should be never be shared with anyone.

- **Root user account gets unrestricted permissions when the account is created, but these can be restricted using IAM policies** - Root user account permissions cannot be restricted, whoever has access to these credentials can perform any operation for that AWS account. The root user credentials should be kept safely.

**References:**

- [https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html)
- [https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)

**Domínio:**
Technology

---

## Pergunta 18

### Correto

**Which AWS service can be used to provision resources to run big data workloads on Hadoop clusters?**

- AWS Step Functions

**Sua resposta está correta**

- Amazon EMR

- AWS Batch

- Amazon Elastic Compute Cloud (Amazon EC2)

### Explicação geral

**Correct option:**

**Amazon EMR**

Amazon EMR is the industry-leading cloud big data platform for processing vast amounts of data using open source tools such as Hadoop, Apache Spark, Apache Hive, Apache HBase, Apache Flink, Apache Hudi, and Presto. Amazon EMR can be used to provision resources to run big data workloads on Hadoop clusters.

**Incorrect options:**

- **AWS Step Functions** - AWS Step Functions service lets you coordinate multiple AWS services into serverless workflows. You can design and run workflows that stitch together services such as AWS Lambda, AWS Glue and Amazon SageMaker.

**AWS Step Functions Overview:** [via Step Functions](https://aws.amazon.com/step-functions/)

- **AWS Batch** - You can use AWS Batch to plan, schedule and execute your batch computing workloads across the full range of AWS compute services. AWS Batch dynamically provisions the optimal quantity and type of compute resources (e.g., CPU or memory optimized instances) based on the volume and specific resource requirements of the batch jobs submitted. AWS Batch provisions compute resources and optimizes the job distribution based on the volume and resource requirements of the submitted batch jobs.

**Please review the common use-cases for AWS Batch:** [via AWS Batch](https://aws.amazon.com/batch/)

**Exam Alert:**

Understand the difference between AWS Step Functions and AWS Batch. You may get questions to choose one over the other. AWS Batch runs batch computing workloads by provisioning the compute resources. AWS Step Functions does not provision any resources. AWS Step Functions only orchestrates AWS services required for a given workflow. You cannot use AWS Step Functions to plan, schedule and execute your batch computing workloads by provisioning underlying resources.

- **Amazon Elastic Compute Cloud (Amazon EC2)** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the AWS cloud. You can use Amazon Elastic Compute Cloud (Amazon EC2) to provision virtual servers on AWS Cloud. You cannot use Amazon Elastic Compute Cloud (Amazon EC2) to plan, schedule and execute your batch computing workloads by provisioning underlying resources.

**References:**

- [https://aws.amazon.com/emr/](https://aws.amazon.com/emr/)
- [https://aws.amazon.com/batch/](https://aws.amazon.com/batch/)
- [https://aws.amazon.com/step-functions/](https://aws.amazon.com/step-functions/)

**Domínio:**
Technology

---

## Pergunta 19

### Correto

**Which of the following is the correct statement regarding the AWS Storage services?**

- Amazon Simple Storage Service (Amazon S3) is block based storage, Amazon Elastic Block Store (Amazon EBS) is object based storage and Amazon Elastic File System (Amazon EFS) is file based storage

- Amazon Simple Storage Service (Amazon S3) is file based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is object based storage

- Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is file based storage and Amazon Elastic File System (Amazon EFS) is block based storage

**Sua resposta está correta**

- Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is file based storage

### Explicação geral

**Correct option:**

**Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is file based storage**

- **Amazon Elastic File System (Amazon EFS)** provides a simple, scalable, fully managed, elastic NFS file system.

- **Amazon Elastic Block Store (Amazon EBS)** is an easy to use, high-performance block storage service designed for use with Amazon Elastic Compute Cloud (Amazon EC2) for both throughput and transaction-intensive workloads at any scale.

- **Amazon Simple Storage Service (Amazon S3)** is an object storage service that offers industry-leading scalability, data availability, security, and performance.

**Incorrect options:**

- Amazon Simple Storage Service (Amazon S3) is block based storage, Amazon Elastic Block Store (Amazon EBS) is object based storage and Amazon Elastic File System (Amazon EFS) is file based storage
- Amazon Simple Storage Service (Amazon S3) is object based storage, Amazon Elastic Block Store (Amazon EBS) is file based storage and Amazon Elastic File System (Amazon EFS) is block based storage
- Amazon Simple Storage Service (Amazon S3) is file based storage, Amazon Elastic Block Store (Amazon EBS) is block based storage and Amazon Elastic File System (Amazon EFS) is object based storage

These three options contradict the details provided earlier in the explanation, so these options are incorrect.

**References:**

- [https://aws.amazon.com/s3/](https://aws.amazon.com/s3/)
- [https://aws.amazon.com/ebs/](https://aws.amazon.com/ebs/)
- [https://aws.amazon.com/efs/](https://aws.amazon.com/efs/)

**Domínio:**
Technology

---

## Pergunta 20

### Incorreto

**What foundational capability under the operations perspective is part of the AWS Cloud Adoption Framework (AWS CAF)?**

- Vulnerability management

**Sua resposta está incorreta**

- Application portfolio management

**Resposta correta**

- Performance and capacity management

- Platform engineering

### Explicação geral

**Correct option:**

**Performance and capacity management**

The AWS Cloud Adoption Framework (AWS CAF) leverages AWS experience and best practices to help you digitally transform and accelerate your business outcomes through innovative use of AWS. Use the AWS CAF to identify and prioritize transformation opportunities, evaluate and improve your cloud readiness, and iteratively evolve your transformation roadmap.

AWS CAF groups its capabilities in six perspectives: Business, People, Governance, Platform, Security, and Operations. Each perspective comprises a set of capabilities that functionally related stakeholders own or manage in your cloud transformation journey.

Operations perspective helps ensure that your cloud services are delivered at a level that meets the needs of your business. Performance and capacity management under the Operations perspective is part of the AWS Cloud Adoption Framework (AWS CAF)

**AWS Cloud Adoption Framework (AWS CAF) - Foundational capabilities:** [via AWS CAF](https://docs.aws.amazon.com/whitepapers/latest/overview-aws-cloud-adoption-framework/foundational-capabilities.html)

**Incorrect options:**

- **Vulnerability management** - Vulnerability management is a foundational capability under the Security perspective for the AWS Cloud Adoption Framework (AWS CAF).

- **Platform engineering** - Platform engineering is a foundational capability under the Platform perspective for the AWS Cloud Adoption Framework (AWS CAF).

- **Application portfolio management** - Application Portfolio Management is a foundational capability under the Governance perspective for the AWS Cloud Adoption Framework (AWS CAF).

**Reference:**

[https://docs.aws.amazon.com/whitepapers/latest/overview-aws-cloud-adoption-framework/foundational-capabilities.html](https://docs.aws.amazon.com/whitepapers/latest/overview-aws-cloud-adoption-framework/foundational-capabilities.html)

**Domínio:**
Security and Compliance

---

## Pergunta 21

### Incorreto

**A photo sharing web application wants to store thumbnails of user-uploaded images on Amazon Simple Storage Service (Amazon S3). The thumbnails are rarely used but need to be immediately accessible from the web application. The thumbnails can be regenerated easily if they are lost. Which is the most cost-effective way to store these thumbnails on Amazon Simple Storage Service (Amazon S3)?**

- Use Amazon S3 Glacier Flexible Retrieval to store the thumbnails

- Use Amazon S3 Standard to store the thumbnails

**Resposta correta**

- Use Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) to store the thumbnails

**Sua resposta está incorreta**

- Use Amazon S3 Standard-Infrequent Access (S3 Standard-IA) to store the thumbnails

### Explicação geral

**Correct option:**

**Use Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) to store the thumbnails**

Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) is for data that is accessed less frequently but requires rapid access when needed. Unlike other S3 Storage Classes which store data in a minimum of three Availability Zones (AZs), Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) stores data in a single Availability Zone (AZ) and costs 20% less than Amazon S3 Standard-Infrequent Access (S3 Standard-IA). Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) offers the same high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee. Although Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) offers less availability than S3 Standard but that's not an issue for the given use-case since the thumbnails can be regenerated easily.

As the thumbnails are rarely used but need to be rapidly accessed when required, so Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) is the best choice for this use-case.

**Exam Alert:**

Please review this detailed comparison on S3 Storage Classes as you can expect a few questions on this aspect of S3: [via S3 Storage Classes](https://aws.amazon.com/s3/storage-classes/)

**Incorrect options:**

- **Use Amazon S3 Standard-Infrequent Access (S3 Standard-IA) to store the thumbnails** - Amazon S3 Standard-Infrequent Access (S3 Standard-IA) storage class is for data that is accessed less frequently but requires rapid access when needed. Amazon S3 Standard-Infrequent Access (S3 Standard-IA) matches the high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee. Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) costs 20% less than Amazon S3 Standard-Infrequent Access (S3 Standard-IA), so this option is incorrect.

- **Use Amazon S3 Standard to store the thumbnails** - Amazon S3 Standard offers high durability, availability, and performance object storage for frequently accessed data. As described above, Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) is a better fit than Amazon S3 Standard, hence using Amazon S3 standard is ruled out for the given use-case.

- **Use Amazon S3 Glacier Flexible Retrieval to store the thumbnails** - Amazon S3 Glacier Flexible Retrieval is a secure, durable, and low-cost storage class for data archiving. Although Amazon S3 Glacier Flexible Retrieval is cheaper than Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA), however the retrieval time ranges from a minute to hours, so this option is also ruled out for the given use-case.

**Reference:**

[https://aws.amazon.com/s3/storage-classes/](https://aws.amazon.com/s3/storage-classes/)

**Domínio:**
Technology

---

## Pergunta 22

### Incorreto

**AWS Compute Optimizer delivers recommendations for which of the following AWS resources? (Select two)**

**Seleção correta**

- Amazon Elastic Block Store (Amazon EBS), AWS Lambda functions

- Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon Elastic File System (Amazon EFS)

- Amazon Elastic File System (Amazon EFS), AWS Lambda functions

**Sua seleção está incorreta**

- AWS Lambda functions, Amazon Simple Storage Service (Amazon S3)

**Sua seleção está correta**

- Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon EC2 Auto Scaling groups

### Explicação geral

**Correct options:**

- **Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon EC2 Auto Scaling groups**

- **Amazon Elastic Block Store (Amazon EBS), AWS Lambda functions**

AWS Compute Optimizer helps you identify the optimal AWS resource configurations, such as Amazon EC2 instance types, Amazon EBS volume configurations, and AWS Lambda function memory sizes, using machine learning to analyze historical utilization metrics. AWS Compute Optimizer delivers recommendations for selected types of EC2 instances, EC2 Auto Scaling groups, Amazon EBS volumes, and AWS Lambda functions.

AWS Compute Optimizer calculates an individual performance risk score for each resource dimension of the recommended instance, including CPU, memory, EBS throughput, EBS IOPS, disk throughput, disk throughput, network throughput, and network packets per second (PPS).

AWS Compute Optimizer provides EC2 instance type and size recommendations for EC2 Auto Scaling groups with a fixed group size, meaning desired, minimum, and maximum are all set to the same value and have no scaling policy attached.

AWS Compute Optimizer supports IOPS and throughput recommendations for General Purpose (SSD) (gp3) volumes and IOPS recommendations for Provisioned IOPS (io1 and io2) volumes.

AWS Compute Optimizer helps you optimize two categories of Lambda functions. The first category includes Lambda functions that may be over-provisioned in memory sizes. The second category includes compute-intensive Lambda functions that may benefit from additional CPU power.

**Incorrect options:**

- **Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon Elastic File System (Amazon EFS)**
- **Amazon Elastic File System (Amazon EFS), AWS Lambda functions**
- **AWS Lambda functions, Amazon Simple Storage Service (Amazon S3)**

AWS Compute Optimizer does not provide optimization recommendations for S3 and EFS, so these options are incorrect.

**Reference:**

[https://aws.amazon.com/compute-optimizer/faqs/](https://aws.amazon.com/compute-optimizer/faqs/)

**Domínio:**
Technology

---

## Pergunta 23

### Incorreto

**A gaming company is looking at a technology/service that can deliver a consistent low-latency gameplay to ensure a great user experience for end-users in various locations. Which AWS technology/service will provide the necessary low-latency access to the end-users?**

**Sua resposta está incorreta**

- AWS Edge Locations

**Resposta correta**

- AWS Local Zones

- AWS Wavelength

- AWS Direct Connect

### Explicação geral

**Correct option:**

**AWS Local Zones**

AWS Local Zones allow you to use select AWS services, like compute and storage services, closer to more end-users, providing them very low latency access to the applications running locally. AWS Local Zones are also connected to the parent region via Amazon’s redundant and very high bandwidth private network, giving applications running in AWS Local Zones fast, secure, and seamless access to the rest of AWS services.

You should use AWS Local Zones to deploy workloads closer to your end-users for low-latency requirements. AWS Local Zones have their connection to the internet and support AWS Direct Connect, so resources created in the Local Zone can serve local end-users with very low-latency communications.

Various AWS services such as Amazon Elastic Compute Cloud (EC2), Amazon Virtual Private Cloud (VPC), Amazon Elastic Block Store (EBS), Amazon FSx, Amazon Elastic Load Balancing, Amazon EMR, Amazon ElastiCache, and Amazon Relational Database Service (RDS) are available locally in the AWS Local Zones. You can also use services that orchestrate or work with local services such as Amazon EC2 Auto Scaling, Amazon EKS clusters, Amazon ECS clusters, Amazon EC2 Systems Manager, Amazon CloudWatch, AWS CloudTrail, and AWS CloudFormation. AWS Local Zones also provide a high-bandwidth, secure connection to the AWS Region, allowing you to seamlessly connect to the full range of services in the AWS Region through the same APIs and toolsets.

**Incorrect options:**

- **AWS Edge Locations** - An AWS Edge location is a site that CloudFront uses to cache copies of the content for faster delivery to users at any location.

- **AWS Wavelength** - AWS Wavelength extends the AWS cloud to a global network of 5G edge locations to enable developers to innovate and build a whole new class of applications that require ultra-low latency. Wavelength Zones provide a high-bandwidth, secure connection to the parent AWS Region, allowing developers to seamlessly connect to the full range of services in the AWS Region through the same APIs and toolsets.

- **AWS Direct Connect** - AWS Direct Connect is a cloud service that links your network directly to AWS, bypassing the internet to deliver more consistent, lower-latency performance. When creating a new connection, you can choose a hosted connection provided by an AWS Direct Connect Delivery Partner, or choose a dedicated connection from AWS—and deploy at over 100 AWS Direct Connect locations around the world. AWS Direct Connect provides consistently high bandwidth, low-latency access and it is generally used between on-premises data centers and AWS network. Direct Connect is overkill for the given requirement.

**Reference:**

[https://aws.amazon.com/about-aws/global-infrastructure/localzones/](https://aws.amazon.com/about-aws/global-infrastructure/localzones/)

**Domínio:**
Technology

---

## Pergunta 24

### Correto

**As per the AWS Shared Responsibility Model, which of the following is a responsibility of the customer from a security and compliance point of view?**

- Configuration management for AWS global infrastructure

**Sua resposta está correta**

- Managing patches of the guest operating system on Amazon Elastic Compute Cloud (Amazon EC2)

- Patching/fixing flaws within the AWS infrastructure

- Availability Zone (AZ) infrastructure management

### Explicação geral

**Correct option:**

**Managing patches of the guest operating system on Amazon Elastic Compute Cloud (Amazon EC2)**

Security and Compliance is a shared responsibility between AWS and the customer. This shared model can help relieve the customer’s operational burden as AWS operates, manages, and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates.

As per the AWS shared responsibility model, the customer is responsible for security "in" the cloud. Customers that deploy an Amazon EC2 instance are responsible for the management of the guest operating system (including updates and security patches), any application software or utilities installed by the customer on the instances, and the configuration of the AWS-provided firewall (called a security group) on each instance.

**Exam Alert:**

Please review the Shared Responsibility Model in detail as you can expect multiple questions on the shared responsibility model in the exam: [via Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Incorrect options:**

- **Configuration management for AWS global infrastructure**
- **Availability Zone (AZ) infrastructure management**
- **Patching/fixing flaws within the AWS infrastructure**

AWS is responsible for “Security of the Cloud”. AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services. Hence, all of the above options - Configuration management for AWS global infrastructure, Availability Zone (AZ) infrastructure management, and patching/fixing flaws within the AWS infrastructure are responsibilities of AWS.

**Reference:**

[https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Domínio:**
Security and Compliance

---

## Pergunta 25

### Correto

**A company wants a fully managed, flexible, and scalable file storage system, with low latency access, for its Windows-based applications. Which AWS service is the right choice for the company?**

- Amazon FSx for Lustre

**Sua resposta está correta**

- Amazon FSx for Windows File Server

- Amazon Elastic File System (Amazon EFS)

- Amazon Elastic Block Storage (Amazon EBS)

### Explicação geral

**Correct option:**

**Amazon FSx for Windows File Server**

Amazon FSx for Windows File Server provides fully managed, highly reliable, and scalable file storage that is accessible over the industry-standard Service Message Block (SMB) protocol. It is built on Windows Server, delivering a wide range of administrative features such as user quotas, end-user file restore, and Microsoft Active Directory (AD) integration.

To support a wide spectrum of workloads, Amazon FSx provides high levels of throughput, IOPS and consistent sub-millisecond latencies. Amazon FSx is accessible from Windows, Linux, and macOS compute instances and devices.

For Windows-based applications, Amazon FSx provides fully managed Windows file servers with features and performance optimized for "lift-and-shift" business-critical application workloads including home directories (user shares), media workflows, and ERP applications. It is accessible from Windows and Linux instances via the SMB protocol.

**Incorrect options:**

- **Amazon Elastic File System (Amazon EFS)** - Amazon Elastic File System (Amazon EFS) is a cloud-native fully managed file system that provides simple, scalable, elastic file storage accessible from Linux instances via the NFS protocol.

- **Amazon FSx for Lustre** - For compute-intensive and fast processing workloads, like high-performance computing (HPC), machine learning, EDA, and media processing, Amazon FSx for Lustre, provides a file system that’s optimized for performance, with input and output stored on Amazon S3. Amazon FSx for Lustre is only compatible with Linux.

- **Amazon Elastic Block Storage (Amazon EBS)** - Amazon EBS is an easy-to-use, high-performance, block-storage service designed for use with Amazon EC2 instances. It is a block-storage service and not a file storage service.

**Reference:**

[https://aws.amazon.com/fsx/windows/](https://aws.amazon.com/fsx/windows/)

**Domínio:**
Technology

## Pergunta 26

**Incorreto**  
_Which AWS service can be used to store, manage, and deploy Docker container images?_

- **Amazon Elastic Compute Cloud (Amazon EC2)**  
  **Sua resposta está incorreta**

- **Amazon Elastic Container Service (Amazon ECS)**

- **AWS Lambda**

**Resposta correta:**

- **Amazon Elastic Container Registry (Amazon ECR)**

### Explicação geral

**Correct option:**

**Amazon Elastic Container Registry (Amazon ECR)** - Amazon Elastic Container Registry (Amazon ECR) can be used to store, manage, and deploy Docker container images. Amazon Elastic Container Registry (Amazon ECR) eliminates the need to operate your container repositories. You can then pull your docker images from Amazon Elastic Container Registry (Amazon ECR) and run those on Amazon Elastic Container Service (Amazon ECS).

Please see this schematic diagram to understand how Amazon Elastic Container Registry (Amazon ECR) works: [via - https://aws.amazon.com/ecr/](https://aws.amazon.com/ecr/)

**Incorrect options:**

- **Amazon Elastic Container Service (Amazon ECS)** - Amazon Elastic Container Service (Amazon ECS) is a highly scalable, fast, container management service that makes it easy to run, stop, and manage Docker containers on a cluster. You cannot use Amazon Elastic Container Service (Amazon ECS) to store and deploy docker container images.

  Please see this schematic diagram to understand how Amazon Elastic Container Service (Amazon ECS) works: [via - https://aws.amazon.com/ecs/](https://aws.amazon.com/ecs/)

- **Amazon Elastic Compute Cloud (Amazon EC2)** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the AWS cloud. You can use EC2 to provision virtual servers on AWS Cloud. You cannot use EC2 to store and deploy docker container images.

- **AWS Lambda** - AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume. You cannot use AWS Lambda to store and deploy docker container images.

**References:**

- [https://aws.amazon.com/ecr/](https://aws.amazon.com/ecr/)
- [https://aws.amazon.com/ecs/](https://aws.amazon.com/ecs/)

**Domínio:**  
Technology

---

## Pergunta 27

**Correto**  
_Which AWS service enables users to find, buy, and immediately start using software solutions in their AWS environment?_

**Sua resposta está correta**

- **AWS Marketplace**

- **AWS OpsWorks**

- **AWS Systems Manager**

- **AWS Config**

### Explicação geral

**Correct option:**

**AWS Marketplace**

AWS Marketplace is a digital catalog with thousands of software listings from independent software vendors that make it easy to find, test, buy, and deploy software that runs on AWS. AWS Marketplace includes thousands of software listings from popular categories such as security, networking, storage, machine learning, IoT, business intelligence, database, and DevOps. You can use AWS Marketplace as a buyer (subscriber) or as a seller (provider), or both. Anyone with an AWS account can use AWS Marketplace as a consumer and can register to become a seller.

**Incorrect options:**

- **AWS Config** - AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. Config continuously monitors and records your AWS resource configurations and allows you to automate the evaluation of recorded configurations against desired configurations. Think resource-specific history, audit, and compliance; think Config.

- **AWS OpsWorks** - AWS OpsWorks is a configuration management service that provides managed instances of Chef and Puppet. OpsWorks lets you use Chef and Puppet to automate how servers are configured, deployed and managed across your Amazon EC2 instances or on-premises compute environments.

- **AWS Systems Manager** - AWS Systems Manager gives you visibility and control of your infrastructure on AWS. Systems Manager provides a unified user interface so you can view operational data from multiple AWS services and allows you to automate operational tasks across your AWS resources. With Systems Manager, you can group resources, like Amazon EC2 instances, Amazon S3 buckets, or Amazon RDS instances, by application, view operational data for monitoring and troubleshooting, and take action on your groups of resources.

**Reference:**

- [https://docs.aws.amazon.com/marketplace/latest/buyerguide/what-is-marketplace.html](https://docs.aws.amazon.com/marketplace/latest/buyerguide/what-is-marketplace.html)

**Domínio:**  
Technology

---

## Pergunta 28

**Correto**  
_A developer has written a simple web application in PHP and he wants to just upload his code to AWS Cloud and have AWS handle the deployment automatically but still wants access to the underlying operating system for further enhancements. As a Cloud Practioner, which of the following AWS services would you recommend for this use-case?_

**Sua resposta está correta**

- **AWS Elastic Beanstalk**

- **AWS CloudFormation**

- **Amazon Elastic Container Service (Amazon ECS)**

- **Amazon Elastic Compute Cloud (Amazon EC2)**

### Explicação geral

**Correct option:**

**AWS Elastic Beanstalk**

AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS. Simply upload your code and AWS Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring. At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time. There is no additional charge for AWS Elastic Beanstalk - you pay only for the AWS resources needed to store and run your applications.

Key Benefits of AWS Elastic Beanstalk: [via - https://aws.amazon.com/elasticbeanstalk/](https://aws.amazon.com/elasticbeanstalk/)

**Incorrect options:**

- **AWS CloudFormation** - AWS CloudFormation allows you to use programming languages or a simple text file (in YAML or JSON format) to model and provision, in an automated and secure manner, all the resources needed for your applications across all Regions and accounts. Think infrastructure as code; think CloudFormation. This is very different from Beanstalk where you just upload your application code and Beanstalk automatically figures out what resources are required to deploy that application. In AWS CloudFormation, you have to explicitly specify which resources you want to provision.

- **Amazon Elastic Compute Cloud (Amazon EC2)** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud, per-second billing, and access to the underlying OS. It is designed to make web-scale cloud computing easier for developers. Maintaining the server and its software has to be done by the customer. EC2 cannot handle the application deployment automatically, so this option is not correct.

- **Amazon Elastic Container Service (Amazon ECS)** - Amazon Elastic Container Service (Amazon ECS) is a highly scalable, fast, container management service that makes it easy to run, stop, and manage Docker containers on a cluster. Amazon Elastic Container Service (Amazon ECS) cannot handle the application deployment automatically, so this option is not correct.

**Reference:**

- [https://aws.amazon.com/elasticbeanstalk/](https://aws.amazon.com/elasticbeanstalk/)

**Domínio:**  
Technology

---

## Pergunta 29

**Correto**  
_An e-commerce company wants to assess its applications deployed on Amazon Elastic Compute Cloud (Amazon EC2) instances for vulnerabilities and deviations from AWS best practices. Which AWS service can be used to facilitate this?_

- **AWS Secrets Manager**

- **AWS CloudHSM**

- **AWS Trusted Advisor**

**Sua resposta está correta**

- **Amazon Inspector**

### Explicação geral

**Correct option:**

**Amazon Inspector**

Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices.

Overview of Amazon Inspector: [via - https://aws.amazon.com/inspector/](https://aws.amazon.com/inspector/)

**Incorrect options:**

- **AWS Secrets Manager** - AWS Secrets Manager helps you protect secrets needed to access your applications, services, and IT resources. The service enables you to easily rotate, manage, and retrieve database credentials, API keys, and other secrets throughout their lifecycle. Users and applications retrieve secrets with a call to Secrets Manager APIs, eliminating the need to hardcode sensitive information in plain text. Secrets Manager cannot be used for security assessment of applications deployed on AWS.

- **AWS CloudHSM** - AWS CloudHSM is a cloud-based hardware security module (HSM) that enables you to easily generate and use your encryption keys on the AWS Cloud. With CloudHSM, you can manage your encryption keys using FIPS 140-2 Level 3 validated HSMs. It is a fully-managed service that automates time-consuming administrative tasks for you, such as hardware provisioning, software patching, high-availability, and backups. CloudHSM cannot be used for the security assessment of applications deployed on AWS.

- **AWS Trusted Advisor** - AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. Trusted Advisor cannot be used for assessing vulnerabilities for applications deployed on AWS.

**Reference:**

- [https://aws.amazon.com/inspector/](https://aws.amazon.com/inspector/)

**Domínio:**  
Security and Compliance

---

## Pergunta 30

**Correto**  
_Which of the following solutions can you use to connect your on-premises network with AWS Cloud (Select two)?_

- **Amazon Virtual Private Cloud (Amazon VPC)**

**Sua seleção está correta**

- **AWS Virtual Private Network (VPN)**

- **Internet Gateway**

**Sua seleção está correta**

- **AWS Direct Connect**

- **Amazon Route 53**

### Explicação geral

**Correct options:**

- **AWS Direct Connect** - AWS Direct Connect is a cloud service solution that makes it easy to establish a dedicated network connection from your premises to AWS. Using AWS Direct Connect, you can establish private connectivity between AWS and your datacenter, office, or colocation environment, which in many cases can reduce your network costs, increase bandwidth throughput, and provide a more consistent network experience than Internet-based connections.

  How AWS Direct Connect Works: [via - https://aws.amazon.com/directconnect/](https://aws.amazon.com/directconnect/)

- **AWS Virtual Private Network (VPN)** - AWS Virtual Private Network (VPN) solutions establish secure connections between on-premises networks, remote offices, client devices, and the AWS global network. AWS VPN is comprised of two services: AWS Site-to-Site VPN and AWS Client VPN. Together, they deliver a highly-available, managed, and elastic cloud VPN solution to protect your network traffic.

  How AWS Client VPN Works: [via - https://aws.amazon.com/vpn/](https://aws.amazon.com/vpn/)

  How AWS Site-to-Site VPN Works: [via - https://aws.amazon.com/vpn/](https://aws.amazon.com/vpn/)

**Incorrect options:**

- **Amazon Virtual Private Cloud (Amazon VPC)** - Amazon Virtual Private Cloud (Amazon VPC) lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including the selection of your IP address range, creation of subnets, and configuration of route tables and network gateways. You cannot use Amazon VPC to connect your on-premises network with AWS Cloud.

- **Internet Gateway** - An Internet Gateway is a horizontally scaled, redundant, and highly available VPC component that allows communication between instances in your VPC and the internet. Therefore, it imposes no availability risks or bandwidth constraints on your network traffic. You cannot use an Internet Gateway to interconnect your on-premises network with AWS Cloud, hence this option is incorrect.

- **Amazon Route 53** - Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect. You cannot use Amazon Route 53 to connect your on-premises network with AWS Cloud.

**References:**

- [https://aws.amazon.com/vpn/](https://aws.amazon.com/vpn/)
- [https://aws.amazon.com/directconnect/](https://aws.amazon.com/directconnect/)

**Domínio:**  
Security and Compliance

---

## Pergunta 31

**Correto**  
_What are the fundamental drivers of cost with AWS Cloud?_

- **Compute, Storage and Inbound Data Transfer**

- **Compute, Databases and Outbound Data Transfer**

**Sua resposta está correta**

- **Compute, Storage and Outbound Data Transfer**

- **Compute, Databases and Inbound Data Transfer**

### Explicação geral

**Correct options:**

**Compute, Storage and Outbound Data Transfer**

There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer. In most cases, there is no charge for inbound data transfer or data transfer between other AWS services within the same region. Outbound data transfer is aggregated across services and then charged at the outbound data transfer rate.

AWS Cloud Pricing Fundamentals: [via - https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf](https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf)

**Incorrect options:**

- **Compute, Storage and Inbound Data Transfer**
- **Compute, Databases and Outbound Data Transfer**
- **Compute, Databases and Inbound Data Transfer**

These three options contradict the details provided earlier in the explanation, so these options are incorrect.

**Reference:**

- [https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf](https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf)

**Domínio:**  
Technology

---

## Pergunta 32

**Correto**  
_A data analytics company stores its data on Amazon Simple Storage Service (Amazon S3) and wants to do SQL based analysis on this data with minimum effort. As a Cloud Practitioner, which of the following AWS services will you suggest for this use case?_

**Sua resposta está correta**

- **Amazon Athena**

- **Amazon Aurora**

- **Amazon DynamoDB**

- **Amazon Redshift**

### Explicação geral

**Correct option:**

**Amazon Athena**

Amazon Athena is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL. Amazon Athena is serverless, so there is no infrastructure to manage, and you pay only for the queries that you run.

Key features of Amazon Athena: [via - https://aws.amazon.com/athena/](https://aws.amazon.com/athena/)

To use Amazon Athena, simply point to your data in Amazon Simple Storage Service (Amazon S3), define the schema, and start querying using standard SQL. Most results are delivered within seconds. With Amazon Athena, there’s no need for complex ETL jobs to prepare your data for analysis. This makes it easy for anyone with SQL skills to quickly analyze large-scale datasets.

**Incorrect options:**

- **Amazon Aurora** - Amazon Aurora is a MySQL and PostgreSQL-compatible relational database built for the cloud, that combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases. You cannot use Amazon Aurora for SQL analysis on S3 based data.

- **Amazon Redshift** - Amazon Redshift is the most popular and fastest cloud data warehouse. Though analytics can be run on Redshift, in the current use case, old data is residing on S3, and Athena is the right choice since analytics can be run directly while data is sitting on S3. You cannot use Amazon Redshift for SQL analysis on S3 based data.

- **Amazon DynamoDB** - Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-Region, multi-master, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. You cannot use Amazon DynamoDB for SQL analysis on S3 based data.

**Reference:**

- [https://aws.amazon.com/athena/](https://aws.amazon.com/athena/)

**Domínio:**  
Technology

---

## Pergunta 33

**Correto**  
_An organization deploys its IT infrastructure in a combination of its on-premises data center along with AWS Cloud. How would you categorize this deployment model?_

**Sua resposta está correta**

- **Hybrid deployment**

- **Private deployment**

- **Mixed deployment**

- **Cloud deployment**

### Explicação geral

**Correct option:**

**Hybrid deployment**

A hybrid deployment is a way to connect your on-premises infrastructure to the cloud. The most common method of hybrid deployment is between the cloud and existing on-premises infrastructure to extend an organization's infrastructure into the cloud while connecting cloud resources to internal systems.

Overview of Cloud Computing Deployment Models: [via - https://aws.amazon.com/types-of-cloud-computing/](https://aws.amazon.com/types-of-cloud-computing/)

**Incorrect options:**

- **Cloud deployment** - For this type of deployment, a cloud-based application is fully deployed in the cloud, and all parts of the application run in the cloud. Applications in the cloud have either been created in the cloud or have been migrated from an existing infrastructure to take advantage of the benefits of cloud computing.

- **Private deployment** - For this deployment model, resources are deployed on-premises using virtualization technologies. On-premises deployment does not provide many of the benefits of cloud computing but is sometimes sought for its ability to provide dedicated resources.

- **Mixed deployment** - This is a made-up option and has been added as a distractor.

**References:**

- [https://aws.amazon.com/types-of-cloud-computing/](https://aws.amazon.com/types-of-cloud-computing/)
- [https://aws.amazon.com/hybrid/](https://aws.amazon.com/hybrid/)

**Domínio:**  
Cloud Concepts

---

## Pergunta 34

**Incorreto**  
_As per the AWS Shared Responsibility Model, which of the following is a responsibility of AWS from a security and compliance point of view?_

- **Identity and Access Management**

**Resposta correta:**

- **Edge Location Management**

**Sua resposta está incorreta**

- **Server-side Encryption (SSE)**

- **Customer Data**

### Explicação geral

**Correct option:**

**Edge Location Management**

Security and Compliance is a shared responsibility between AWS and the customer. The AWS Shared Responsibility Model can help relieve the customer’s operational burden as AWS operates, manages, and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates.

AWS is responsible for security "of" the cloud. This covers their global infrastructure elements including Regions, Availability Zones (AZ), and Edge Locations.

**Incorrect options:**

- **Customer Data**

- **Identity and Access Management**

- **Server-side Encryption (SSE)**

The customer is responsible for security "in" the cloud. Customers are responsible for managing their data including encryption options and using Identity and Access Management tools for implementing appropriate access control policies as per their organization requirements. For abstracted services, such as Amazon S3 and Amazon DynamoDB, AWS operates the infrastructure layer, the operating system, and platforms, and customers access the endpoints to store and retrieve data. Therefore, these three options fall under the responsibility of the customer according to the AWS shared responsibility model.

**Exam Alert:**

Please review the AWS Shared Responsibility Model in detail as you can expect multiple questions on this topic in the exam: [via - https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Reference:**

- [https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Domínio:**  
Security and Compliance

---

## Pergunta 35

**Incorreto**  
_An organization has a complex IT architecture involving a lot of system dependencies and it wants to track the history of changes to each resource. Which AWS service will help the organization track the history of configuration changes for all the resources?_

- **AWS CloudFormation**

**Resposta correta:**

- **AWS Config**

**Sua resposta está incorreta**

- **AWS CloudTrail**

- **AWS Service Catalog**

### Explicação geral

**Correct option:**

**AWS Config**

AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. Config continuously monitors and records your AWS resource configurations and allows you to automate the evaluation of recorded configurations against desired configurations. Think resource-specific history, audit, and compliance; think Config.

With AWS Config, you can do the following:

1. Evaluate your AWS resource configurations for desired settings.
2. Get a snapshot of the current configurations of the supported resources that are associated with your AWS account.
3. Retrieve configurations of one or more resources that exist in your account.
4. Retrieve historical configurations of one or more resources.
5. Receive a notification whenever a resource is created, modified, or deleted.
6. View relationships between resources. For example, you might want to find all resources that use a particular security group.

**Incorrect options:**

- **AWS Service Catalog** - AWS Service Catalog allows organizations to create and manage catalogs of IT services that are approved for use on AWS. These IT services can include everything from virtual machine images, servers, software, and databases to complete multi-tier application architectures. You cannot use Service Catalog to track changes to each resource on AWS.

- **AWS CloudFormation** - AWS CloudFormation provides a common language to model and provision AWS and third-party application resources in your cloud environment. AWS CloudFormation allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all Regions and accounts. Think infrastructure as code; think CloudFormation. You cannot use CloudFormation to track changes to each resource on AWS.

- **AWS CloudTrail** - AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. CloudTrail provides the event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command-line tools, and other AWS services. Think account-specific activity and audit; think CloudTrail. You cannot use CloudTrail to track changes to each resource on AWS.

**Reference:**

- [https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html](https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html)

**Domínio:**  
Security and Compliance

---

## Pergunta 36

**Correto**  
_Which of the following use-cases is NOT supported by Amazon Rekognition?_

- **Label objects in a photo**

**Sua resposta está correta**

- **Quickly resize photos to create thumbnails**

- **Identify person in a photo**

- **Detect text in a photo**

### Explicação geral

**Correct option:**

**Quickly resize photos to create thumbnails**

You cannot use Amazon Rekognition to resize photos to create thumbnails.

With Amazon Rekognition, you can identify objects, people, text, scenes, and activities in images and videos, as well as detect any inappropriate content. Amazon Rekognition also provides highly accurate facial analysis and facial search capabilities that you can use to detect, analyze, and compare faces for a wide variety of user verification, people counting, and public safety use cases.

Amazon Rekognition Use-Cases: [via - https://aws.amazon.com/rekognition/](https://aws.amazon.com/rekognition/)

**Incorrect options:**

- **Identify person in a photo**
- **Detect text in a photo**
- **Label objects in a photo**

As mentioned in the explanation above, Amazon Rekognition can be used to build solutions for these use-cases.

**Reference:**

- [https://aws.amazon.com/rekognition/](https://aws.amazon.com/rekognition/)

**Domínio:**  
Technology

---

## Pergunta 37

**Correto**  
_What is the primary benefit of deploying an Amazon RDS Multi-AZ database with one standby?_

- **Amazon RDS Multi-AZ reduces database usage costs**

**Sua resposta está correta**

- **Amazon RDS Multi-AZ enhances database availability**

- **Amazon RDS Multi-AZ protects the database from a regional failure**

- **Amazon RDS Multi-AZ improves database performance for read-heavy workloads**

### Explicação geral

**Correct option:**

**Amazon RDS Multi-AZ enhances database availability**

Amazon RDS Multi-AZ deployments provide enhanced availability and durability for Amazon Relational Database Service (Amazon RDS) instances, making them a natural fit for production database workloads. When you provision an Amazon RDS Multi-AZ Instance with one standby, Amazon RDS automatically creates a primary DB Instance and synchronously replicates the data to a standby instance in a different Availability Zone (AZ).

In case of an infrastructure failure, Amazon RDS performs an automatic failover to the standby so that you can resume database operations as soon as the failover is complete.

How Amazon RDS Multi-AZ Works: [via - https://aws.amazon.com/rds/features/multi-az/](https://aws.amazon.com/rds/features/multi-az/)

**Exam Alert:**

Please review the differences between Multi-AZ, Multi-Region and Read Replica deployments for RDS: [via - https://aws.amazon.com/rds/features/multi-az/](https://aws.amazon.com/rds/features/multi-az/)

**Incorrect options:**

- **Amazon RDS Multi-AZ improves database performance for read-heavy workloads** - Amazon RDS Multi-AZ with one standby does not allow read operations from the standby. Read Replicas allow you to create read-only copies that are synchronized with your master database. Read Replicas are used for improved read performance. Therefore, this option is incorrect.

- **Amazon RDS Multi-AZ protects the database from a regional failure** - You need to use RDS in Multi-Region deployment configuration to protect from a regional failure. Amazon RDS Multi-AZ cannot protect from a regional failure.

- **Amazon RDS Multi-AZ reduces database usage costs** - Amazon RDS Multi-AZ increases the database costs compared to the standard deployment. So this option is incorrect.

**Reference:**

- [https://aws.amazon.com/rds/features/multi-az/](https://aws.amazon.com/rds/features/multi-az/)

**Domínio:**  
Technology

---

## Pergunta 38

**Correto**  
_Which AWS technology/service helps you to scale your resources to match supply with demand while still keeping your cloud solution cost-effective?_

- **AWS CloudFormation**

- **AWS OpsWorks**

**Sua resposta está correta**

- **AWS Auto Scaling**

- **AWS Cost Explorer**

### Explicação geral

**Correct option:**  
**AWS Auto Scaling**

AWS Auto Scaling monitors applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it’s easy to setup application scaling for multiple resources across multiple services in minutes. The service provides a simple, powerful user interface that lets you build scaling plans for resources including Amazon EC2 instances and Spot Fleets, Amazon ECS tasks, Amazon DynamoDB tables and indexes, and Amazon Aurora Replicas. AWS Auto Scaling makes scaling simple with recommendations that allow you to optimize performance, costs, or balance between them.

How AWS Auto Scaling Works: [via - https://aws.amazon.com/autoscaling/](https://aws.amazon.com/autoscaling/)

**Incorrect options:**

- **AWS Cost Explorer** - AWS Cost Explorer lets you explore your AWS costs and usage at both a high level and at a detailed level of analysis, and empowering you to dive deeper using many filtering dimensions (e.g., AWS Service, Region, Linked Account). It's a handy tool to keep track of costs of AWS resources, but auto-scaling is not part of its feature set.

- **AWS OpsWorks** - AWS OpsWorks is a configuration management service that provides managed instances of Chef and Puppet. Chef and Puppet are automation platforms that allow you to use code to automate the configurations of your servers. OpsWorks lets you use Chef and Puppet to automate how servers are configured, deployed and managed across your Amazon EC2 instances or on-premises compute environments. OpsWorks cannot auto-scale resources.

- **AWS CloudFormation** - AWS CloudFormation allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all Regions and accounts. Think infrastructure as code; think CloudFormation. CloudFormation cannot auto-scale resources.

**References:**

- [https://aws.amazon.com/autoscaling/](https://aws.amazon.com/autoscaling/)
- [https://aws.amazon.com/aws-cost-management/aws-cost-explorer/](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)
- [https://aws.amazon.com/opsworks/](https://aws.amazon.com/opsworks/)
- [https://aws.amazon.com/cloudformation/](https://aws.amazon.com/cloudformation/)

**Domínio:**  
Cloud Concepts

---

## Pergunta 39

**Correto**  
_A customer has created a VPC and a subnet within AWS Cloud. Which of the following statements is correct?_

**Sua resposta está correta**

- **An Amazon Virtual Private Cloud (Amazon VPC) spans all of the Availability Zones (AZ) in the Region whereas a subnet spans only one Availability Zone (AZ) in the Region**

- **Both the Amazon Virtual Private Cloud (Amazon VPC) and the subnet span only one Availability Zone (AZ) in the Region**

- **Both the Amazon Virtual Private Cloud (Amazon VPC) and the subnet span all of the Availability Zones (AZ) in the Region**

- **A subnet spans all of the Availability Zones (AZ) in the Region whereas an Amazon Virtual Private Cloud (Amazon VPC) spans only one Availability Zone (AZ) in the Region**

### Explicação geral

**Correct option:**

**An Amazon Virtual Private Cloud (Amazon VPC) spans all of the Availability Zones (AZ) in the Region whereas a subnet spans only one Availability Zone (AZ) in the Region**

Amazon Virtual Private Cloud (Amazon VPC) is a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including the selection of your IP address range, creation of subnets, and configuration of route tables and network gateways. An Amazon Virtual Private Cloud (Amazon VPC) spans all of the Availability Zones (AZ) in the Region.

A subnet is a range of IP addresses within your Amazon Virtual Private Cloud (Amazon VPC). A subnet spans only one Availability Zone (AZ) in the Region.

Amazon Virtual Private Cloud (Amazon VPC) and Subnet Overview: [via - https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)

**Incorrect options:**

- **Both the Amazon Virtual Private Cloud (Amazon VPC) and the subnet span all of the Availability Zones (AZ) in the Region**
- **Both the Amazon Virtual Private Cloud (Amazon VPC) and the subnet span only one Availability Zone (AZ) in the Region**
- **A subnet spans all of the Availability Zones (AZ) in the Region whereas an Amazon Virtual Private Cloud (Amazon VPC) spans only one Availability Zone (AZ) in the Region**

These three options contradict the details provided earlier in the explanation, so these options are incorrect.

**Reference:**

- [https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)

**Domínio:**  
Technology

---

## Pergunta 40

**Correto**  
_Which tool will help you review your workloads against current AWS best practices for cost optimization, security, and performance improvement and then obtain advice to architect them better?_

- **AWS Cost Explorer**

- **Amazon CloudWatch**

**Sua resposta está correta**

- **AWS Trusted Advisor**

- **Amazon Inspector**

### Explicação geral

**Correct option:**

**AWS Trusted Advisor**

AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. All AWS customers get access to the seven core Trusted Advisor checks to help increase the security and performance of the AWS environment.

How Trusted Advisor Works: [via - https://aws.amazon.com/premiumsupport/technology/trusted-advisor/](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)

AWS Trusted Advisor Recommendations: [via - https://aws.amazon.com/premiumsupport/technology/trusted-advisor/](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)

**Incorrect options:**

- **AWS Cost Explorer** - AWS Cost Explorer lets you explore your AWS costs and usage at both a high level and at a detailed level of analysis, and empowering you to dive deeper using several filtering dimensions (e.g., AWS Service, Region, Linked Account). Cost Explorer does not offer any recommendations vis-a-vis AWS best practices for cost optimization, security, and performance improvement.

- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. This is an excellent service for building Resilient systems. Think resource performance monitoring, events, and alerts; think CloudWatch. CloudWatch does not offer any recommendations vis-a-vis AWS best practices for cost optimization, security, and performance improvement.

- **Amazon Inspector** - Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. Amazon Inspector cannot be used to prevent Distributed Denial-of-Service (DDoS) attack. Inspector does not offer any recommendations vis-a-vis AWS best practices for cost optimization, security, and performance improvement.

**Reference:**

- [https://aws.amazon.com/premiumsupport/technology/trusted-advisor/](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)

**Domínio:**  
Cloud Concepts

### Pergunta 41

**Incorreto**  
**Which of the following AWS services are global in scope? (Select two)**

**Seleção correta**

- Amazon CloudFront

**Sua seleção está incorreta**

- Amazon Relational Database Service (Amazon RDS)
- Amazon Simple Storage Service (Amazon S3)
- Amazon Elastic Compute Cloud (Amazon EC2)

**Sua seleção está correta**

- AWS Identity and Access Management (AWS IAM)

**Explicação geral**  
**Correct options:**

- **AWS Identity and Access Management (AWS IAM)**
- **Amazon CloudFront**

Most of the services that AWS offers are Region specific. But few services, by definition, need to be in a global scope because of the underlying service they offer. AWS Identity and Access Management (AWS IAM), Amazon CloudFront, Amazon Route 53, and AWS Web Application Firewall (AWS WAF) are some of the global services.

AWS Identity and Access Management (AWS IAM) enables you to manage access to AWS services and resources securely. Using AWS Identity and Access Management (AWS IAM), you can create and manage IAM users and IAM user-groups, and use permissions to allow and deny their access to AWS resources.

Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment.

**Incorrect options:**

- **Amazon Relational Database Service (Amazon RDS)** - Amazon Relational Database Service (Amazon RDS) makes it easy to set up, operate, and scale a relational database in the cloud. This is a regional service.
- **Amazon Elastic Compute Cloud (Amazon EC2)** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It comes under Infrastructure as a Service (IaaS) type of Cloud Computing. This is a regional service.

**Exam Alert:**

- **Amazon Simple Storage Service (Amazon S3)** - Amazon Simple Storage Service (Amazon S3) is a unique service in the sense that it follows a global namespace but the buckets are regional. You specify an AWS Region when you create your Amazon S3 bucket. This is a regional service.

**References:**

- [AWS IAM FAQs](https://aws.amazon.com/iam/faqs/)
- [Amazon CloudFront FAQs](https://aws.amazon.com/cloudfront/faqs/)

**Domínio**  
Technology

---

### Pergunta 42

**Correto**  
**Which of the following AWS services allows a database to have a flexible schema and supports document data models?**

- Amazon Redshift
- Amazon Relational Database Service (Amazon RDS)
- Amazon Aurora

**Sua resposta está correta**

- Amazon DynamoDB

**Explicação geral**  
**Correct option:**

- **Amazon DynamoDB**

Amazon DynamoDB is a NoSQL database that supports key-value and document data models and enables developers to build modern, serverless applications that can start small and scale globally to support petabytes of data and tens of millions of read and write requests per second.

Amazon DynamoDB supports both key-value and document data models. This enables Amazon DynamoDB to have a flexible schema, so each row can have any number of columns at any point in time. This allows you to easily adapt the tables as your business requirements change, without having to redefine the table schema as you would in relational databases.

**Incorrect options:**

- **Amazon Relational Database Service (Amazon RDS)** - Amazon Relational Database Service (Amazon RDS) is an AWS service for relational databases. Schema change on a relational database is not as easy and straightforward as it is on a NoSQL database. Amazon Relational Database Service (Amazon RDS) does not support flexible schema.
- **Amazon Redshift** - Amazon Redshift is a fully-managed petabyte-scale cloud-based data warehouse product designed for large-scale data set storage and analysis. Amazon Redshift does not support flexible schema.
- **Amazon Aurora** - Amazon Aurora is an AWS service for relational databases. Schema change on a relational database is not as easy and straightforward as it is on a NoSQL database. Amazon Aurora does not support flexible schema.

**Reference:**

- [Amazon DynamoDB Features](https://aws.amazon.com/dynamodb/features/)

**Domínio**  
Technology

---

### Pergunta 43

**Correto**  
**Which AWS support plan provides access to a designated Technical Account Manager (TAM)?**

- AWS Business Support
- AWS Enterprise On-Ramp Support

**Sua resposta está correta**

- AWS Enterprise Support

- AWS Developer Support

**Explicação geral**  
**Correct option:**

- **AWS Enterprise Support**

AWS offers four different support plans to cater to each of its customers - AWS Developer Support, AWS Business Support, AWS Enterprise On-Ramp Support, and AWS Enterprise Support plans. A basic support plan is included for all AWS customers.

AWS Enterprise Support provides customers with concierge-like service where the main focus is helping the customer achieve their outcomes and find success in the cloud. With AWS Enterprise Support, you get 24x7 technical support from high-quality engineers, tools and technology to automatically manage the health of your environment, consultative architectural guidance delivered in the context of your applications and use-cases, and a designated Technical Account Manager (TAM) to coordinate access to proactive/preventative programs and AWS subject matter experts.

**Exam Alert:**

Please review the differences between the AWS Developer Support, AWS Business Support, AWS Enterprise On-Ramp Support, and AWS Enterprise Support plans as you can expect at least a couple of questions on the exam:

- [AWS Support Plans](https://aws.amazon.com/premiumsupport/plans/)

**Incorrect options:**

- **AWS Developer Support** - You should use the AWS Developer Support plan if you are testing or doing early development on AWS and want the ability to get technical support during business hours as well as general architectural guidance as you build and test.
- **AWS Business Support** - You should use the AWS Business Support plan if you have production workloads on AWS and want 24x7 access to technical support and architectural guidance in the context of your specific use-cases.
- **AWS Enterprise On-Ramp Support** - You should use the AWS Enterprise On-Ramp Support plan if you have production/business critical workloads in AWS and want 24x7 access to technical support and need expert guidance to grow and optimize in the Cloud. With this plan, you get access to a pool of Technical Account Managers to provide proactive guidance and coordinate access to programs and AWS experts.

**Reference:**

- [AWS Enterprise Support](https://aws.amazon.com/premiumsupport/plans/enterprise/)

**Domínio**  
Billing and Pricing

---

### Pergunta 44

**Incorreto**  
**What are the different gateway types supported by AWS Storage Gateway service?**

- Object Gateway, File Gateway, and Block Gateway

**Sua resposta está incorreta**

- Tape Gateway, File Gateway, and Block Gateway

**Resposta correta**

- Tape Gateway, File Gateway, and Volume Gateway

- Tape Gateway, Object Gateway, and Volume Gateway

**Explicação geral**  
**Correct option:**

- **Tape Gateway, File Gateway, and Volume Gateway**

AWS Storage Gateway is a hybrid cloud storage service that connects your existing on-premises environments with the AWS Cloud. Customers use Storage Gateway to simplify storage management and reduce costs for key hybrid cloud storage use cases. These include moving tape backups to the cloud, reducing on-premises storage with cloud-backed file shares, providing low latency access to data in AWS for on-premises applications, as well as various migration, archiving, processing, and disaster recovery use cases.

AWS Storage Gateway service provides three different types of gateways – Tape Gateway, File Gateway, and Volume Gateway – that seamlessly connect on-premises applications to cloud storage, caching data locally for low-latency access.

**Gateway Storage Types Overview:**

- [AWS Storage Gateway Features](https://aws.amazon.com/storagegateway/features/)

**Incorrect options:**

- Object Gateway, File Gateway, and Block Gateway
- Tape Gateway, Object Gateway, and Volume Gateway
- Tape Gateway, File Gateway, and Block Gateway

Block Gateway and Object Gateway are made-up options, so these three options are incorrect.

**Reference:**

- [AWS Storage Gateway Features](https://aws.amazon.com/storagegateway/features/)

**Domínio**  
Technology

---

### Pergunta 45

**Incorreto**  
**An e-commerce company wants to store data from a recommendation engine in a database. As a Cloud Practioner, which AWS service would you recommend to provide this functionality with the LEAST operational overhead for any scale?**

- Amazon Relational Database Service (Amazon RDS)
- Amazon Simple Storage Service (Amazon S3)

**Resposta correta**

- Amazon DynamoDB

**Sua resposta está incorreta**

- Amazon Neptune

**Explicação geral**  
**Correct options:**

- **Amazon DynamoDB**

Amazon DynamoDB is a key-value and document database that delivers sub-millisecond performance at any scale. Amazon DynamoDB enables customers to offload the administrative burdens of operating and scaling distributed databases to AWS so that they don’t have to worry about hardware provisioning, setup and configuration, throughput capacity planning, replication, software patching, or cluster scaling.

You can use Amazon DynamoDB to store recommendation results with the LEAST operational overhead for any scale.

- [How to Use Amazon DynamoDB](https://catalog.us-east-1.prod.workshops.aws/workshops/ed82a5d4-6630-41f0-a6a1-9345898fa6ec/en-US/batch/dynamodb)

**Incorrect options:**

- **Amazon Relational Database Service (Amazon RDS)** - Amazon Relational Database Service (Amazon RDS) is a relational database service from AWS. Amazon RDS is less operationally efficient than Amazon DynamoDB while building a highly scalable solution.
- **Amazon Simple Storage Service (Amazon S3)** - Amazon Simple Storage Service (Amazon S3) is an object storage service and not a database service.
- **Amazon Neptune** - Amazon Neptune is a fully managed database service built for the cloud that makes it easier to build and run graph applications. It's not the right fit to store recommendation results with the LEAST operational overhead for any scale.

**Reference:**

- [How to Use Amazon DynamoDB](https://catalog.us-east-1.prod.workshops.aws/workshops/ed82a5d4-6630-41f0-a6a1-9345898fa6ec/en-US/batch/dynamodb)

**Domínio**  
Technology

---

### Pergunta 46

**Correto**  
**Which AWS service would you use to send alerts when the costs for your AWS account exceed your budgeted amount?**

- AWS Pricing Calculator

**Sua resposta está correta**

- AWS Budgets

- AWS Organizations
- AWS Cost Explorer

**Explicação geral**  
**Correct option:**

- **AWS Budgets**

AWS Budgets gives the ability to set custom budgets that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount. You can also use AWS Budgets to set reservation utilization or coverage targets and receive alerts when your utilization drops below the threshold you define. Budgets can be created at the monthly, quarterly, or yearly level, and you can customize the start and end dates. You can further refine your budget to track costs associated with multiple dimensions, such as AWS service, linked account, tag, and others. Budget alerts can be sent via email and/or Amazon Simple Notification Service (Amazon SNS) topic.

- [AWS Budgets Overview](https://aws.amazon.com/aws-cost-management/aws-budgets/)

**Exam Alert:**

It is useful to note the difference between CloudWatch Billing vs AWS Budgets:

- **CloudWatch Billing Alarms:** Sends an alarm when the actual cost exceeds a certain threshold.
- **AWS Budgets:** Sends an alarm when the actual cost exceeds the budgeted amount or even when the cost forecast exceeds the budgeted amount.

**Incorrect options:**

- **AWS Cost Explorer** - AWS Cost Explorer has an easy-to-use interface that lets you visualize, understand, and manage your AWS costs and usage over time. AWS Cost Explorer includes a default report that helps you visualize the costs and usage associated with your top five cost-accruing AWS services and gives you a detailed breakdown on all services in the table view. The reports let you adjust the time range to view historical data going back up to twelve months to gain an understanding of your cost trends.

  - [AWS Cost Explorer Reports](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)

**Exam Alert:**

Watch out for questions on AWS Cost Explorer vs AWS Budgets. AWS Budgets can alert you when your costs exceed your budgeted amount. Cost Explorer helps you visualize and manage your AWS costs and usage over time.

- **AWS Organizations** - AWS Organizations helps you centrally govern your environment as you grow and scale your workloads on AWS. Whether you are a growing startup or a large enterprise, Organizations helps you to centrally manage billing; control access, compliance, and security; and share resources across your AWS accounts.

- **AWS Pricing Calculator** - AWS Pricing Calculator lets you explore AWS services and create an estimate for the cost of your use cases on AWS. You can model your solutions before building them, explore the price points and calculations behind your estimate, and find the available instance types and contract terms that meet your needs. This enables you to make informed decisions about using AWS. You can plan your AWS costs and usage or price out setting up a new set of instances and services. AWS Pricing Calculator can be accessed at [AWS Pricing Calculator](https://calculator.aws/#/).

**Reference:**

- [AWS Budgets Overview](https://aws.amazon.com/aws-cost-management/aws-budgets/)

**Domínio**  
Billing and Pricing

---

### Pergunta 47

**Correto**  
**Which policy describes prohibited uses of the web services offered by Amazon Web Services?**

- AWS Applicable Use Policy
- AWS Fair Use Policy
- AWS Trusted Advisor

**Sua resposta está correta**

- AWS Acceptable Use Policy

**Explicação geral**  
**Correct option:**

- **AWS Acceptable Use Policy**

The Acceptable Use Policy describes prohibited uses of the web services offered by Amazon Web Services, Inc. and its affiliates (the “Services”) and the website located at http://aws.amazon.com (the “AWS Site”). This policy is present at [AWS Acceptable Use Policy](https://aws.amazon.com/aup/) and is updated on a need basis by AWS.

**Incorrect options:**

- **AWS Trusted Advisor** - AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. Trusted Advisor does not describe prohibited uses of the web services offered by Amazon Web Services.
- **AWS Fair Use Policy** - This is a made-up option and has been added as a distractor.
- **AWS Applicable Use Policy** - This is a made-up option and has been added as a distractor.

**Reference:**

- [AWS Acceptable Use Policy](https://aws.amazon.com/aup/)

**Domínio**  
Cloud Concepts

---

### Pergunta 48

**Correto**  
**Which of the following AWS services is essential for implementing security of resources in AWS Cloud?**

- AWS Shield
- Amazon CloudWatch

**Sua resposta está correta**

- AWS Identity and Access Management (IAM)

- AWS Web Application Firewall (AWS WAF)

**Explicação geral**  
**Correct option:**

- **AWS Identity and Access Management (IAM)**

AWS Identity and Access Management (IAM) enables you to manage access to AWS services and resources securely. Using IAM, you can create and manage AWS users and groups, and use permissions to allow and deny their access to AWS resources. IAM enables security best practices by allowing you to grant unique security credentials to users and groups to specify which AWS service APIs and resources they can access. These features make IAM an important service for the overall security of AWS resources in your account. IAM is secure by default; users have no access to AWS resources until permissions are explicitly granted.

**Incorrect options:**

- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. This is an excellent service for building Resilient systems. Think resource performance monitoring, events, and alerts; think CloudWatch.
- **AWS Shield** - AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS. AWS Shield provides always-on detection and automatic inline mitigations that minimize application downtime and latency, so there is no need to engage AWS Support to benefit from DDoS protection. AWS Shield cannot be used to handle resource-specific security on AWS.
- **AWS Web Application Firewall (AWS WAF)** - By using AWS Web Application Firewall (AWS WAF), you can configure web access control lists (Web ACLs) on your CloudFront distributions or Application Load Balancers to filter and block requests based on request signatures. Besides, by using AWS WAF's rate-based rules, you can automatically block the IP addresses of bad actors when requests matching a rule exceed a threshold that you define. AWS WAF cannot be used to handle resource-specific security on AWS.

**Reference:**

- [AWS Identity and Access Management (IAM)](https://aws.amazon.com/iam/)

**Domínio**  
Cloud Concepts

---

### Pergunta 49

**Incorreto**  
**The AWS Cloud Adoption Framework (AWS CAF) recommends four iterative and incremental cloud transformation phases. Which cloud transformation journey phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on demonstrating how the cloud will help accelerate your business outcomes?**

**Sua resposta está incorreta**

- Align

**Resposta correta**

- Envision

- Launch
- Scale

**Explicação geral**  
**Correct option:**

- **Envision**

The Envision phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on demonstrating how the cloud will help accelerate your business outcomes.

**Incorrect options:**

- **Align** - The Align phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on identifying capability gaps across the six AWS CAF perspectives, identifying cross-organizational dependencies, and surfacing stakeholder concerns and challenges.
- **Launch** - The Launch phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on delivering pilot initiatives in production and on demonstrating incremental business value.
- **Scale** - The Scale phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on expanding production pilots and business value to desired scale and ensuring that the business benefits associated with your cloud investments are realized and sustained.

**Reference:**

- [AWS Cloud Adoption Framework (AWS CAF)](https://d1.awsstatic.com/whitepapers/aws-caf-ebook.pdf)

**Domínio**  
Cloud Concepts

---

### Pergunta 50

**Correto**  
**Which of the following AWS services can be used to prevent Distributed Denial-of-Service (DDoS) attack? (Select three)**

- AWS CloudHSM

**Sua seleção está correta**

- AWS Web Application Firewall (AWS WAF)

- AWS Trusted Advisor

**Sua seleção está correta**

- Amazon CloudFront with Amazon Route 53

**Sua seleção está correta**

- AWS Shield

- Amazon Inspector

**Explicação geral**  
**Correct options:**

- **AWS Shield** - AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS. AWS Shield provides always-on detection and automatic inline mitigations that minimize application downtime and latency, so there is no need to engage AWS Support to benefit from DDoS protection.
- **AWS Web Application Firewall (AWS WAF)** - By using AWS Web Application Firewall (AWS WAF), you can configure web access control lists (Web ACLs) on your Amazon CloudFront distributions or Application Load Balancers to filter and block requests based on request signatures. Besides, by using the AWS Web Application Firewall (AWS WAF) rate-based rules, you can automatically block the IP addresses of bad actors when requests matching a rule exceed a threshold that you define.
- **Amazon CloudFront with Amazon Route 53** - AWS hosts Amazon CloudFront and Amazon Route 53 services on a distributed network of proxy servers in data centers throughout the world called edge locations. Using the global Amazon network of edge locations for application delivery and DNS service plays an important part in building a comprehensive defense against DDoS attacks for your dynamic web applications.

- [How AWS Shield, AWS Web Application Firewall (AWS WAF), and Amazon CloudFront with Amazon Route 53 help mitigate DDoS attacks](https://aws.amazon.com/blogs/security/how-to-protect-dynamic-web-applications-against-ddos-attacks-by-using-amazon-cloudfront-and-amazon-route-53/)

**Incorrect options:**

- **AWS CloudHSM** - AWS CloudHSM is a cloud-based hardware security module (HSM) that enables you to easily generate and use your encryption keys on the AWS Cloud. With CloudHSM, you can manage your encryption keys using FIPS 140-2 Level 3 validated HSMs. It is a fully-managed service that automates time-consuming administrative tasks for you, such as hardware provisioning, software patching, high-availability, and backups. CloudHSM cannot be used to prevent Distributed Denial-of-Service (DDoS) attack.
- **AWS Trusted Advisor** - AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. Trusted Advisor cannot be used to prevent Distributed Denial-of-Service (DDoS) attack.
- **Amazon Inspector** - Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. Amazon Inspector cannot be used to prevent Distributed Denial-of-Service (DDoS) attack.

**References:**

- [DDoS Overview](https://docs.aws.amazon.com/waf/latest/developerguide/ddos-overview.html)
- [AWS Shield](https://aws.amazon.com/shield/)
- [DDoS White Paper](https://d1.awsstatic.com/whitepapers/Security/DDoS_White_Paper.pdf)
- [How to Protect Dynamic Web Applications Against DDoS Attacks](https://aws.amazon.com/blogs/security/how-to-protect-dynamic-web-applications-against-ddos-attacks-by-using-amazon-cloudfront-and-amazon-route-53/)

**Domínio**  
Security and Compliance

---

### Pergunta 51

**Correto**  
**Which of the following statements are true about AWS Lambda? (Select two)**

- AWS Lambda provides access to the underlying operating system to control its behavior through code

**Sua seleção está correta**

- AWS Lambda lets you run code without provisioning or managing servers

**Sua seleção está correta**

- You pay for the compute time you consume for AWS Lambda

- AWS Lambda allows you to orchestrate and manage Docker containers to facilitate complex containerized applications on AWS
- AWS Lambda allows you to install databases on the underlying serverless Operating System

**Explicação geral**  
**Correct options:**

- **AWS Lambda lets you run code without provisioning or managing servers**
- **You pay for the compute time you consume for AWS Lambda**

AWS Lambda is a compute service that lets you run code without provisioning or managing servers. AWS Lambda executes your code only when needed and scales automatically, from a few requests per day to thousands per second. You pay for the compute time and the number of requests for your Lambda function - there is no charge when your code is not running. With AWS Lambda, you can run code for virtually any type of application or backend service - all with zero administration. AWS Lambda runs your code on a high-availability compute infrastructure and performs all of the administration of the compute resources, including server and operating system maintenance, capacity provisioning and automatic scaling, code monitoring and logging.

- [How AWS Lambda Works](https://aws.amazon.com/lambda/)

**Incorrect options:**

- **AWS Lambda allows you to install databases on the underlying serverless Operating System** - AWS Lambda is a serverless compute service offered by AWS. Since the underlying hardware is only provisioned for the time of compute, it is not possible to install a database.
- **AWS Lambda allows you to orchestrate and manage Docker containers to facilitate complex containerized applications on AWS** - AWS Lambda is a serverless compute service offered by AWS. While AWS Lambda can be used to package and deploy Lambda functions as container images of up to 10 GB in size. But AWS Lambda cannot be used to orchestrate and manage Docker containers. Amazon ECS is better suited for this use-case.
- **AWS Lambda provides access to the underlying operating system to control its behavior through code** - AWS Lambda is a serverless compute service offered by AWS. It is serverless, so the underlying operating system is not accessible. Amazon Beanstalk or Amazon EC2 services should be used if you need to access the underlying operating system.

**Reference:**

- [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)

**Domínio**  
Technology

---

### Pergunta 52

**Correto**  
**An organization is planning to move its infrastructure from the on-premises datacenter to AWS Cloud. As a Cloud Practioner, which options would you recommend so that the organization can identify the right AWS services to build solutions on AWS Cloud (Select two)?**

- AWS Organizations
- AWS CloudTrail

**Sua seleção está correta**

- AWS Service Catalog

- Amazon CloudWatch

**Sua seleção está correta**

- AWS Partner Network (APN)

**Explicação geral**  
**Correct options:**

- **AWS Service Catalog** - AWS Service Catalog allows organizations to create and manage catalogs of IT services that are approved for use on AWS. These IT services can include everything from virtual machine images, servers, software, and databases to complete multi-tier application architectures.
- **AWS Partner Network (APN)** - Organizations can take help from the AWS Partner Network (APN) to identify the right AWS services to build solutions on AWS Cloud. AWS Partner Network (APN) is the global partner program for technology and consulting businesses that leverage Amazon Web Services to build solutions and services for customers.

**Incorrect options:**

- **AWS Organizations** - AWS Organizations helps you centrally govern your environment as you grow and scale your workloads on AWS. AWS Organizations help you to centrally manage billing; control access, compliance, and security; and share resources across your AWS accounts. AWS Organizations cannot help in identifying the right AWS services to build solutions on AWS Cloud.
- **Amazon CloudWatch** - Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides data and actionable insights to monitor your applications, respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. Think resource performance monitoring, events, and alerts; think CloudWatch. CloudWatch cannot help in identifying the right AWS services to build solutions on AWS Cloud.
- **AWS CloudTrail** - AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. Think account-specific activity and audit; think CloudTrail. CloudTrail cannot help in identifying the right AWS services to build solutions on AWS Cloud.

**References:**

- [AWS Service Catalog](https://aws.amazon.com/servicecatalog/)
- [AWS Partner Network (APN)](https://aws.amazon.com/partners/)

**Domínio**  
Security and Compliance

---

### Pergunta 53

**Correto**  
**Which of the following AWS services comes under the Software as a Service (SaaS) Cloud Computing Type?**

- Amazon Elastic Compute Cloud (Amazon EC2)
- AWS Elastic Beanstalk
- Elastic Load Balancing (ELB)

**Sua resposta está correta**

- Amazon Rekognition

**Explicação geral**  
**Correct option:** Amazon Rekognition

Cloud Computing can be broadly divided into three types - Infrastructure as a Service (IaaS), Platform as a Service (PaaS), Software as a Service (SaaS).

IaaS contains the basic building blocks for cloud IT. It typically provides access to networking features, computers (virtual or on dedicated hardware), and data storage space. IaaS gives the highest level of flexibility and management control over IT resources. Examples - Amazon EC2 (on AWS), GCP, Azure, Rackspace, Digital Ocean, Linode.

PaaS removes the need to manage underlying infrastructure (usually hardware and operating systems) and allows you to focus on the deployment and management of your applications. You don’t need to worry about resource procurement, capacity planning, software maintenance, patching, or any of the other undifferentiated heavy lifting involved in running your application. Examples - Elastic Beanstalk (on AWS), Heroku, Google App Engine (GCP), Windows Azure (Microsoft).

SaaS provides you with a complete product that is run and managed by the service provider. With a SaaS offering, you don’t have to think about how the service is maintained or how the underlying infrastructure is managed. You only need to think about how you will use that particular software. Examples - Amazon Rekognition, Google Apps (Gmail), Dropbox, Zoom.

- [Overview of Cloud Computing Types](https://aws.amazon.com/types-of-cloud-computing/)

You can use Amazon Rekognition to add image and video analysis to your applications using proven, highly scalable, deep learning technology that requires no machine learning expertise. With Amazon Rekognition, you can identify objects, people, text, scenes, and activities in images and videos as well as detect any inappropriate content. Rekognition is an example of Software as a Service (Saas) model.

**Incorrect options:**

- **Amazon Elastic Compute Cloud (Amazon EC2)** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. Hence, it comes under Infrastructure as a Service (IaaS) type of Cloud Computing.
- **AWS Elastic Beanstalk** - AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services. You simply upload your code and Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring. Per the definitions above, Elastic Beanstalk falls under the Platform as a Service (PaaS) type.
- **Elastic Load Balancing (ELB)** - Elastic Load Balancing (ELB) automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and Lambda functions. It can handle the varying load of your application traffic in a single Availability Zone (AZ) or across multiple Availability Zones (AZ). This has been added as a distractor.

**References:**

- [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/)
- [What is Cloud Computing?](https://aws.amazon.com/what-is-cloud-computing/)

**Domínio**  
Cloud Concepts

---

### Pergunta 54

**Correto**  
**Which AWS service helps with global application availability and performance using the AWS global network?**

**Sua resposta está correta**

- AWS Global Accelerator

- Amazon CloudFront
- Amazon Route 53
- Elastic Load Balancing (ELB)

**Explicação geral**  
**Correct option:**

- **AWS Global Accelerator**

AWS Global Accelerator is a service that improves the availability and performance of your applications with local or global users. It provides static IP addresses that act as a fixed entry point to your application endpoints in a single or multiple AWS Regions, such as your Application Load Balancers, Network Load Balancers, or Amazon EC2 instances. AWS Global Accelerator uses the AWS global network to optimize the path from your users to your applications, improving the performance of your traffic by as much as 60%.

AWS Global Accelerator improves performance for a wide range of applications over TCP or UDP by proxying packets at the edge to applications running in one or more AWS Regions. AWS Global Accelerator is a good fit for non-HTTP use cases, such as gaming (UDP), IoT (MQTT), or Voice over IP, as well as for HTTP use cases that specifically require static IP addresses or deterministic, fast regional failover.

- [How AWS Global Accelerator Works](https://aws.amazon.com/global-accelerator/)

**Exam Alert:**

Please review the differences between Amazon CloudFront and AWS Global Accelerator:

- [Amazon CloudFront vs AWS Global Accelerator](https://aws.amazon.com/global-accelerator/faqs/)

**Incorrect options:**

- **Amazon CloudFront** - Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment. It cannot be used to improve application availability and performance using the AWS global network.
- **Elastic Load Balancing (ELB)** - Elastic Load Balancing (ELB) distributes incoming application or network traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses, in multiple Availability Zones. Elastic Load Balancing (ELB) scales your load balancer as traffic to your application changes over time. It can automatically scale to the vast majority of workloads. Elastic Load Balancing (ELB) cannot be used to improve application availability and performance using the AWS global network.
- **Amazon Route 53** - Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect. It cannot be used to improve application availability and performance using the AWS global network.

**Reference:**

- [AWS Global Accelerator](https://aws.amazon.com/global-accelerator/)

**Domínio**  
Technology

---

### Pergunta 55

**Incorreto**  
**A startup is looking for 24x7 phone based technical support for its AWS account. Which of the following is the MOST cost-effective AWS support plan for this use-case?**

**Resposta correta**

- AWS Business Support

- AWS Enterprise On-Ramp Support
- AWS Developer Support

**Sua resposta está incorreta**

- AWS Enterprise Support

**Explicação geral**  
**Correct option:**

AWS offers four different support plans to cater to each of its customers - AWS Developer Support, AWS Business Support, AWS Enterprise On-Ramp Support, and AWS Enterprise Support plans. A basic support plan is included for all AWS customers.

- **AWS Business Support** - You should use the AWS Business Support plan if you have production workloads on AWS and want 24x7 phone, email and chat access to technical support and architectural guidance in the context of your specific use-cases. AWS Business Support plan is the MOST cost-effective option for the given use-case.

**Exam Alert:**

Please review the differences between the AWS Developer Support, AWS Business Support, AWS Enterprise On-Ramp Support and AWS Enterprise Support plans as you can expect at least a couple of questions on the exam:

- [AWS Support Plans](https://aws.amazon.com/premiumsupport/plans/)

**Incorrect options:**

- **AWS Enterprise On-Ramp Support** - You should use the AWS Enterprise On-Ramp Support plan if you have production/business critical workloads in AWS and want 24x7 access to technical support and need expert guidance to grow and optimize in the Cloud. AWS Enterprise On-Ramp Support plan provides 24x7 phone, email and chat access to technical support however it's costlier than the AWS Business Support plan.
- **AWS Developer Support** - You should use the AWS Developer Support plan if you are testing or doing early development on AWS and want the ability to get email based technical support during business hours as well as general architectural guidance as you build and test. This plan does not support 24x7 phone based technical support.
- **AWS Enterprise Support** - You should use the AWS Enterprise Support plan to provide customers with concierge-like service where the main focus is helping the customer achieve their outcomes and find success in the cloud. With AWS Enterprise Support plan, you get 24x7 technical support from high-quality engineers, tools and technology to automatically manage the health of your environment, consultative architectural guidance delivered in the context of your applications and use-cases, and a designated Technical Account Manager (TAM) to coordinate access to proactive/preventative programs and AWS subject matter experts. AWS Enterprise Support plan provides 24x7 phone, email and chat access to technical support however it's costlier than the AWS Business Support plan.

**Reference:**

- [AWS Support Plans](https://aws.amazon.com/premiumsupport/plans/)

**Domínio**  
Billing and Pricing

### Pergunta 56

**Correto**  
**Which of the following statements is INCORRECT about AWS Auto Scaling?**

- Você pode escalar e adicionar mais instâncias do Amazon Elastic Compute Cloud (Amazon EC2) para corresponder a um aumento na demanda, bem como escalar e remover instâncias do Amazon Elastic Compute Cloud (Amazon EC2) para corresponder a uma demanda reduzida
- **Sua resposta está correta:** Você pode implantar automaticamente o AWS Shield quando um ataque DDoS é detectado
- Você pode remover automaticamente instâncias não saudáveis
- Você pode registrar automaticamente novas instâncias em um balanceador de carga

**Explicação geral**  
**Correct option:**

Você pode implantar automaticamente o AWS Shield quando um ataque DDoS é detectado.

O AWS Auto Scaling é útil durante um ataque DDoS, pois pode escalar recursos rapidamente. No entanto, não pode implantar automaticamente o serviço AWS Shield em seu grupo de recursos.

**Incorrect options:**

- O AWS Auto Scaling monitora suas aplicações e ajusta automaticamente a capacidade para manter um desempenho estável e previsível ao menor custo possível. Usando o AWS Auto Scaling, é fácil configurar o escalonamento de aplicações para vários recursos em vários serviços em minutos. O serviço oferece uma interface de usuário simples e poderosa que permite criar planos de escalonamento para recursos, incluindo instâncias Amazon EC2 e Spot Fleets, tarefas Amazon ECS, tabelas e índices Amazon DynamoDB e Réplicas do Amazon Aurora.

- Você pode escalar e adicionar mais instâncias do Amazon Elastic Compute Cloud (Amazon EC2) para corresponder a um aumento na demanda, bem como escalar e remover instâncias do Amazon Elastic Compute Cloud (Amazon EC2) para corresponder a uma demanda reduzida - Conforme explicado acima, ele pode escalar recursos sob demanda, bem como escalar recursos para corresponder a uma demanda reduzida.

- Você pode remover automaticamente instâncias não saudáveis - Com base em verificações de integridade, o Auto Scaling pode remover instâncias não saudáveis.

- Você pode registrar automaticamente novas instâncias em um balanceador de carga - Durante um processo de escalonamento, o Auto Scaling pode iniciar novas instâncias e registrá-las no balanceador de carga, também parte do grupo de escalonamento.

**Reference:**  
[https://aws.amazon.com/autoscaling/](https://aws.amazon.com/autoscaling/)

**Domínio:**  
Technology

---

### Pergunta 57

**Correto**  
**A company's flagship application runs on a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances. As per the new policies, the system administrators are looking for the best way to provide secure shell access to Amazon Elastic Compute Cloud (Amazon EC2) instances without opening new ports or using public IP addresses.**

**Which tool/service will help you achieve this requirement?**

- **Sua resposta está correta:** AWS Systems Manager Session Manager
- Amazon Inspector
- Amazon Elastic Compute Cloud (Amazon EC2) Instance Connect
- Amazon Route 53

**Explicação geral**  
**Correct option:**

AWS Systems Manager Session Manager

O AWS Systems Manager Session Manager é um serviço totalmente gerenciado que oferece uma experiência de shell interativa baseada em navegador e CLI. Ele ajuda a fornecer gerenciamento de instâncias seguro e auditável sem a necessidade de abrir portas de entrada, manter hosts bastion e gerenciar chaves SSH. O AWS Systems Manager Session Manager ajuda a habilitar a conformidade com políticas corporativas que exigem acesso controlado às instâncias, aumenta a segurança e a auditabilidade do acesso às instâncias, proporcionando simplicidade e acesso a instâncias em plataformas cruzadas para os usuários finais.

**Incorrect options:**

- Amazon Elastic Compute Cloud (Amazon EC2) Instance Connect - O Amazon Elastic Compute Cloud (Amazon EC2) Instance Connect oferece uma maneira simples e segura de se conectar às suas instâncias Linux usando o Secure Shell (SSH). Com o EC2 Instance Connect, você usa políticas e princípios do AWS Identity and Access Management (IAM) para controlar o acesso SSH às suas instâncias, eliminando a necessidade de compartilhar e gerenciar chaves SSH. O EC2 Instance Connect exigirá que a porta 22 esteja aberta para o tráfego. Portanto, não é a opção correta aqui.

- Amazon Inspector - O Amazon Inspector é um serviço automatizado de avaliação de segurança que ajuda a melhorar a segurança e a conformidade de aplicativos implantados na AWS. O Amazon Inspector avalia automaticamente os aplicativos quanto à exposição, vulnerabilidades e desvios das práticas recomendadas. Após realizar uma avaliação, o Amazon Inspector gera uma lista detalhada de achados de segurança priorizados por nível de gravidade. O Amazon Inspector não pode fornecer acesso seguro de shell a instâncias EC2.

- Amazon Route 53 - O Amazon Route 53 é um serviço de web DNS (Domain Name System) altamente disponível e escalável na nuvem. Ele é projetado para fornecer aos desenvolvedores e empresas uma maneira extremamente confiável e econômica de direcionar os usuários finais para aplicativos na Internet, traduzindo nomes como www.exemplo.com em endereços IP numéricos como 192.0.2.1, que os computadores usam para se conectar uns aos outros. O Amazon Route 53 não pode fornecer acesso seguro de shell a instâncias EC2.

**Reference:**  
[https://aws.amazon.com/systems-manager/faq/](https://aws.amazon.com/systems-manager/faq/)

**Domínio:**  
Technology

---

### Pergunta 58

**Correto**  
**According to the AWS Shared Responsibility Model, which of the following are responsibilities of the customer for Amazon RDS?**

- **Sua resposta está correta:** Database encryption
- Applying patches to the underlying OS
- Managing the underlying server hardware on which Amazon Relational Database Service (Amazon RDS) runs
- Applying patches to the Amazon Relational Database Service (Amazon RDS) database

**Explicação geral**  
**Correct option:**

Security and Compliance é uma responsabilidade compartilhada entre a AWS e o cliente. Esse modelo compartilhado pode ajudar a aliviar o ônus operacional do cliente, pois a AWS opera, gerencia e controla os componentes desde o sistema operacional host e a camada de virtualização até a segurança física das instalações nas quais o serviço opera.

Database encryption - Sob o Modelo de Responsabilidade Compartilhada da AWS, os clientes são responsáveis por gerenciar seus dados, incluindo a criptografia de dados.

**AWS Shared Responsibility Model Overview:**  
[https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Incorrect options:**

De acordo com o Modelo de Responsabilidade Compartilhada da AWS, a AWS é responsável pela "Segurança da Nuvem". Isso inclui proteger a infraestrutura que executa todos os serviços oferecidos na Nuvem AWS. Essa infraestrutura é composta por hardware, software, redes e instalações que executam os serviços da Nuvem AWS.

- Amazon Relational Database Service (Amazon RDS) é um serviço gerenciado que facilita a configuração, operação e escalonamento de um banco de dados relacional na nuvem.

- Managing the underlying server hardware on which Amazon Relational Database Service (Amazon RDS) runs - Como o Amazon Relational Database Service (Amazon RDS) é um serviço gerenciado, a infraestrutura subjacente é responsabilidade da AWS.

- Applying patches to the Amazon Relational Database Service (Amazon RDS) database - Como o Amazon Relational Database Service (Amazon RDS) é um serviço gerenciado, a infraestrutura subjacente é responsabilidade da AWS.

- Applying patches to the underlying OS - Como o Amazon Relational Database Service (Amazon RDS) é um serviço gerenciado, a infraestrutura subjacente é responsabilidade da AWS.

**Reference:**  
[https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Domínio:**  
Security and Compliance

---

### Pergunta 59

**Correto**  
**Which of the following statement is correct for a Security Group and a Network Access Control List (Network ACL)?**

- Security Group acts as a firewall at the subnet level whereas Network Access Control List (Network ACL) acts as a firewall at the instance level
- Security Group acts as a firewall at the VPC level whereas Network Access Control List (Network ACL) acts as a firewall at the Availability Zone (AZ) level
- **Sua resposta está correta:** Security Group acts as a firewall at the instance level whereas Network Access Control List (Network ACL) acts as a firewall at the subnet level
- Security Group acts as a firewall at the Availability Zone (AZ) level whereas Network Access Control List (Network ACL) acts as a firewall at the VPC level

**Explicação geral**  
**Correct option:**

Security Group acts as a firewall at the instance level whereas Network Access Control List (Network ACL) acts as a firewall at the subnet level.

Um grupo de segurança atua como um firewall virtual para sua instância para controlar o tráfego de entrada e saída. Quando você lança uma instância em uma VPC, você pode atribuir até cinco grupos de segurança à instância. Os grupos de segurança atuam no nível da instância, não no nível do sub-rede. Uma lista de controle de acesso de rede (network ACL) é uma camada opcional de segurança para sua VPC que atua como um firewall para controlar o tráfego dentro e fora de uma ou mais sub-redes (ou seja, funciona no nível da sub-rede).

**Security Group Overview:**  
[https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)

**Network Access Control List (network NACL) Overview:**  
[https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)

**Incorrect options:**

- Security Group acts as a firewall at the subnet level whereas Network Access Control List (Network ACL) acts as a firewall at the instance level - Como explicado acima, o grupo de segurança atua no nível da instância e a lista de controle de acesso de rede (network ACL) está no nível da sub-rede.

- Security Group acts as a firewall at the VPC level whereas Network Access Control List (Network ACL) acts as a firewall at the Availability Zone (AZ) level - Como explicado acima, o grupo de segurança atua no nível da instância e a lista de controle de acesso de rede (network ACL) está no nível da sub-rede.

- Security Group acts as a firewall at the Availability Zone (AZ) level whereas Network Access Control List (Network ACL) acts as a firewall at the VPC level - Como explicado acima, o grupo de segurança atua no nível da instância e a lista de controle de acesso de rede (network ACL) está no nível da sub-rede.

**References:**

- [https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)
- [https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)

**Domínio:**  
Technology

---

### Pergunta 60

**Correto**  
**Which of the following AWS services are always free to use (Select two)?**

- Amazon DynamoDB
- **Sua seleção está correta:** AWS Auto Scaling
- Amazon Elastic Compute Cloud (Amazon EC2)
- Amazon Simple Storage Service (Amazon S3)
- **Sua seleção está correta:** AWS Identity and Access Management (AWS IAM)

**Explicação geral**  
**Correct options:**

- **AWS Identity and Access Management (AWS IAM)** - O AWS Identity and Access Management (AWS IAM) permite que você gerencie o acesso com segurança aos serviços e recursos da AWS. Usando o IAM, você pode criar e gerenciar usuários e grupos do IAM e usar permissões para permitir ou negar o acesso a recursos da AWS. O IAM é um recurso da sua conta da AWS oferecido sem cobrança adicional.

- **AWS Auto Scaling** - O AWS Auto Scaling monitora suas aplicações e ajusta automaticamente a capacidade para manter um desempenho estável e previsível ao menor custo possível. Usando o AWS Auto Scaling, é fácil configurar o escalonamento de aplicações para vários recursos em vários serviços em minutos. O AWS Auto Scaling está disponível sem cobrança adicional. Você paga apenas pelos recursos da AWS necessários para executar suas aplicações e as taxas de monitoramento do Amazon CloudWatch.

**Incorrect options:**

- **Amazon Elastic Compute Cloud (Amazon EC2)** - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço da web que fornece capacidade de computação segura e redimensionável na nuvem. Ele é projetado para facilitar a computação em nuvem em escala na web para desenvolvedores. Este não é um serviço gratuito. Você paga pelo que usa ou dependendo do plano que escolher.

- **Amazon Simple Storage Service (Amazon S3)** - O Amazon Simple Storage Service (Amazon S3) é um serviço de armazenamento de objetos que oferece escalabilidade, disponibilidade de dados, segurança e desempenho líderes do setor. O serviço S3 não é gratuito e você paga dependendo da classe de armazenamento que escolher para seus dados.

- **Amazon DynamoDB** - O Amazon DynamoDB é um banco de dados de chave-valor e documento que oferece desempenho em milissegundos de um dígito em qualquer escala. É um banco de dados totalmente gerenciado, multi-região, multi-master, durável, com segurança, backup e restauração integrados e cache em memória para aplicações em escala na Internet. O DynamoDB não é gratuito e você é cobrado por leitura, gravação e armazenamento de dados em suas tabelas DynamoDB, junto com quaisquer recursos opcionais que escolher ativar.

**References:**

- [https://aws.amazon.com/iam/](https://aws.amazon.com/iam/)
- [https://aws.amazon.com/autoscaling/](https://aws.amazon.com/autoscaling/)

**Domínio:**  
Cloud Concepts

---

### Pergunta 61

**Correto**  
**Multi-AZ deployment is an example of which of the following?**

- **Sua resposta está correta:** High Availability
- Scale out
- Scale up
- Performance Efficiency

**Explicação geral**  
**Correct option:**

**High Availability**

Um sistema que está disponível é capaz de entregar a funcionalidade projetada em um determinado momento. Sistemas altamente disponíveis são aqueles que podem suportar algum nível de degradação enquanto continuam disponíveis. Na Nuvem AWS, você pode executar instâncias para uma aplicação em uma implantação Multi-AZ para alcançar Alta Disponibilidade.

**Incorrect options:**

- **Scale out** - A operação de scale out (escalonamento horizontal) refere-se a um aumento de capacidade adicionando mais computadores ao sistema. Isso contrasta com uma operação de "scale up", que é limitada a executar seus processos em apenas um computador; em tais sistemas, a única maneira de aumentar o desempenho é adicionar mais recursos em um computador na forma de CPUs, memória ou armazenamento mais rápidos (ou mais). Sistemas escalonáveis horizontalmente muitas vezes são capazes de superar sistemas escalonáveis verticalmente, permitindo a execução paralela de cargas de trabalho e distribuindo essas cargas entre vários computadores diferentes. Auto Scaling Group é um exemplo de Escalonamento Horizontal na AWS.

- **Scale up** - A operação de scale up (escalonamento vertical) implica adicionar mais recursos (como CPU, RAM) a um único nó ou máquina. Exemplo: redimensionamento de uma instância EC2.

- **Performance Efficiency** - Performance Efficiency é a capacidade de usar recursos de computação de forma eficiente para atender aos requisitos do sistema e manter essa eficiência à medida que a demanda muda e as tecnologias evoluem.

**References:**

- [https://wa.aws.amazon.com/wat.concept.availability.en.html](https://wa.aws.amazon.com/wat.concept.availability.en.html)
- [https://wa.aws.amazon.com/wat.concept.horizontal-scaling.en.html](https://wa.aws.amazon.com/wat.concept.horizontal-scaling.en.html)

**Domínio:**  
Cloud Concepts

---

### Pergunta 62

**Correto**  
**Which of the following are examples of Horizontal Scalability (aka Elasticity)? (Select two)**

- Add a bigger CPU to a computer
- Modify an EC2 instance type from t2.nano to u-12tb1.metal
- **Sua seleção está correta:** Read Replicas in Amazon Relational Database Service (Amazon RDS)
- Modify a Database instance to higher CPU and RAM
- **Sua seleção está correta:** Elastic Load Balancing (ELB)

**Explicação geral**  
**Correct options:**

Um sistema "escalonável horizontalmente" é aquele que pode aumentar a capacidade adicionando mais computadores ao sistema. Isso contrasta com um sistema "escalonável verticalmente", que é limitado a executar seus processos em apenas um computador; em tais sistemas, a única maneira de aumentar o desempenho é adicionar mais recursos em um computador na forma de CPUs, memória ou armazenamento mais rápidos (ou mais). Sistemas escalonáveis horizontalmente muitas vezes são capazes de superar sistemas escalonáveis verticalmente, permitindo a execução paralela de cargas de trabalho e distribuindo essas cargas entre vários computadores diferentes.

**Elastic Load Balancing (ELB)**

O Elastic Load Balancing (ELB) distribui automaticamente o tráfego de aplicação recebido entre vários destinos, como instâncias Amazon EC2, contêineres, endereços IP e funções Lambda. Ele pode lidar com a carga variável de tráfego de sua aplicação em uma única Zona de Disponibilidade (AZ) ou em várias Zonas de Disponibilidade (AZ). Isso se enquadra no Escalonamento Horizontal.

**Read Replicas in Amazon Relational Database Service (Amazon RDS)**

O Amazon Relational Database Service (Amazon RDS) facilita a configuração, operação e escalonamento de um banco de dados relacional na nuvem. As réplicas de leitura permitem que você crie cópias somente leitura que são sincronizadas com seu banco de dados mestre. Você também pode colocar sua réplica de leitura em uma Região AWS diferente, mais próxima de seus usuários, para melhor desempenho. Réplicas de leitura são um exemplo de escalonamento horizontal de recursos.

**Incorrect options:**

- **Add a bigger CPU to a computer** - Como explicado acima, isso se enquadra no escalonamento vertical, pois o recurso maior está sendo adicionado a um único computador ou nó.

- **Modify an EC2 instance type from t2.nano to u-12tb1.metal** - Aumentar o tipo de um único sistema Amazon EC2 também é um exemplo de escalonamento vertical, pois a capacidade extra está sendo adicionada a uma única instância.

- **Modify a Database instance to higher CPU and RAM** - Isso também é um exemplo de escalonamento vertical, pois o foco está no aumento da capacidade de uma única máquina ou instância.

**Reference:**  
[https://wa.aws.amazon.com/wat.concept.horizontal-scaling.en.html](https://wa.aws.amazon.com/wat.concept.horizontal-scaling.en.html)

**Domínio:**  
Cloud Concepts

---

### Pergunta 63

**Correto**  
**A retail company has multiple AWS accounts for each of its departments. Which of the following AWS services can be used to set up consolidated billing and a single payment method for these AWS accounts?**

- AWS Cost Explorer
- AWS Secrets Manager
- **Sua resposta está correta:** AWS Organizations
- AWS Budgets

**Explicação geral**  
**Correct option:**

**AWS Organizations**

O AWS Organizations ajuda você a gerenciar centralmente a cobrança; controlar o acesso, conformidade e segurança; e compartilhar recursos em suas contas AWS. Usando o AWS Organizations, você pode automatizar a criação de contas, criar grupos de contas para refletir suas necessidades de negócios e aplicar políticas a esses grupos para governança. Você também pode simplificar a cobrança configurando um único método de pagamento para todas as suas contas AWS. O AWS Organizations está disponível para todos os clientes da AWS sem custo adicional.

**Key Features of AWS Organizations:**  
[https://aws.amazon.com/organizations/](https://aws.amazon.com/organizations/)

**Incorrect options:**

- **AWS Cost Explorer** - O AWS Cost Explorer possui uma interface fácil de usar que permite visualizar, entender e gerenciar seus custos e uso da AWS ao longo do tempo. O AWS Cost Explorer inclui um relatório padrão que ajuda a visualizar os custos e o uso associados aos seus cinco principais serviços da AWS que mais consomem custos e oferece uma visão detalhada de todos os serviços na visualização de tabela. Os relatórios permitem que você ajuste o período de tempo para visualizar dados históricos de até doze meses para obter uma compreensão das tendências de seus custos. Você não pode usar o AWS Cost Explorer para configurar cobrança consolidada e um único método de pagamento para várias contas da AWS.

- **AWS Budgets** - O AWS Budgets oferece a capacidade de definir orçamentos personalizados que alertam quando seus custos ou uso excedem (ou são previstos para exceder) o valor orçado. Você também pode usar o AWS Budgets para definir metas de utilização ou cobertura de reservas e receber alertas quando sua utilização cair abaixo do limite que você define. Os orçamentos podem ser criados em nível mensal, trimestral ou anual, e você pode personalizar as datas de início e término. Você pode refinar ainda mais seu orçamento para rastrear custos associados a várias dimensões, como serviço AWS, conta vinculada, tag e outros. Você não pode usar o AWS Budgets para configurar cobrança consolidada e um único método de pagamento para várias contas da AWS.

- **AWS Secrets Manager** - O AWS Secrets Manager ajuda a proteger segredos necessários para acessar suas aplicações, serviços e recursos de TI. O serviço permite que você gire, gerencie e recupere facilmente credenciais de banco de dados, chaves de API e outros segredos ao longo de seu ciclo de vida. Você não pode usar o AWS Secrets Manager para configurar cobrança consolidada e um único método de pagamento para várias contas da AWS.

**Reference:**  
[https://aws.amazon.com/organizations/](https://aws.amazon.com/organizations/)

**Domínio:**  
Billing and Pricing

---

### Pergunta 64

**Incorreto**  
**A fleet of Amazon EC2 instances spread across different Availability Zones (AZ) needs to access, edit and share file-based data stored centrally on a system. As a Cloud Practitioner, which AWS service would you recommend for this use-case?**

- **Resposta correta:** Amazon Elastic File System (Amazon EFS)
- EC2 Instance Store
- Amazon Simple Storage Service (Amazon S3)
- **Sua resposta está incorreta:** Amazon Elastic Block Store (Amazon EBS)

**Explicação geral**  
**Correct option:**

**Amazon Elastic File System (Amazon EFS)**

O Amazon Elastic File System (Amazon EFS) oferece um sistema de arquivos NFS simples, escalável, totalmente gerenciado e elástico. Ele foi projetado para escalar sob demanda para petabytes sem interromper aplicações, crescendo e encolhendo automaticamente conforme você adiciona e remove arquivos, eliminando a necessidade de provisionar e gerenciar capacidade para acomodar o crescimento. O Amazon EFS foi projetado para fornecer acesso compartilhado paralelo maciço a milhares de instâncias Amazon EC2, permitindo que suas aplicações alcancem altos níveis de taxa de transferência e IOPS agregadas com latências consistentemente baixas.

**How Amazon Elastic File System (Amazon EFS) Works:**  
[https://aws.amazon.com/efs/](https://aws.amazon.com/efs/)

**Incorrect options:**

- **Amazon Elastic Block Store (Amazon EBS)** - O Amazon Elastic Block Store (EBS) é um serviço de armazenamento em bloco de alto desempenho, fácil de usar, projetado para uso com o Amazon Elastic Compute Cloud (EC2) para cargas de trabalho intensivas em taxa de transferência e transações em qualquer escala. Uma ampla gama de cargas de trabalho, como bancos de dados relacionais e não relacionais, aplicações empresariais, aplicações em contêineres, mecanismos de análise de big data, sistemas de arquivos e fluxos de trabalho de mídia são amplamente implantados no Amazon EBS. Para o exame Cloud Practitioner, você deve considerar que um volume EBS só pode ser montado em uma instância EC2 por vez, portanto, esta opção não é correta para o caso de uso dado. Como caso especial, você deve observar que o Amazon EBS Multi-Attach permite que você anexe um único volume SSD de IOPS provisionados (io1 ou io2) a várias instâncias baseadas em nitro que estão na mesma Zona de Disponibilidade (AZ).

- **EC2 Instance Store** - Um instance store fornece armazenamento temporário em nível de bloco para sua instância EC2. Este armazenamento está localizado em discos fisicamente conectados ao computador host. O armazenamento de instâncias é ideal para o armazenamento temporário de informações que mudam com frequência, como buffers, caches, dados temporários e outros conteúdos temporários, ou para dados que são replicados em uma frota de instâncias, como um pool de servidores web balanceado por carga. O armazenamento de instâncias é temporário, os dados são perdidos se a instância falhar ou for encerrada. O armazenamento de instâncias EC2 não pode ser usado para compartilhamento de arquivos entre instâncias.

- **Amazon Simple Storage Service (Amazon S3)** - O Amazon Simple Storage Service (Amazon S3) é um serviço de armazenamento de objetos que oferece escalabilidade, disponibilidade de dados, segurança e desempenho líderes do setor. Isso significa que clientes de todos os tamanhos e indústrias podem usá-lo para armazenar e proteger qualquer quantidade de dados para uma variedade de casos de uso, como sites, aplicações móveis, backup e restauração, arquivamento, aplicações empresariais, dispositivos IoT e análise de big data. Como o S3 é um armazenamento baseado em objetos, não pode ser usado para compartilhamento de arquivos entre instâncias.

**Reference:**  
[https://aws.amazon.com/efs/](https://aws.amazon.com/efs/)

**Domínio:**  
Technology

---

### Pergunta 65

**Correto**  
**Which AWS service should be used when you want to run container applications, but want to avoid the operational overhead of scaling, patching, securing, and managing servers?**

- Amazon Elastic Compute Cloud (Amazon EC2)
- **Sua resposta está correta:** Amazon Elastic Container Service (Amazon ECS) - Fargate launch type
- AWS Lambda
- Amazon Elastic Container Service (Amazon ECS) - EC2 launch type

**Explicação geral**  
**Correct option:**

**Amazon Elastic Container Service (Amazon ECS) - Fargate launch type**

O AWS Fargate é um mecanismo de computação sem servidor para contêineres. Ele funciona com o Amazon Elastic Container Service (Amazon ECS) e o Amazon Elastic Kubernetes Service (Amazon EKS). O AWS Fargate facilita para você se concentrar na construção de suas aplicações. O AWS Fargate elimina a necessidade de provisionar e gerenciar servidores, permite que você especifique e pague pelos recursos por aplicação e melhora a segurança por meio de isolamento de aplicação por design. O AWS Fargate aloca a quantidade certa de computação, eliminando a necessidade de escolher instâncias e escalar a capacidade do cluster. Você só paga pelos recursos necessários para executar seus contêineres, então não há superdimensionamento e pagamento por servidores adicionais. O AWS Fargate executa cada tarefa ou pod em seu kernel, fornecendo às tarefas e pods seu próprio ambiente de computação isolado. Isso permite que sua aplicação tenha isolamento de carga de trabalho e segurança aprimorada por design.

**How AWS Fargate Works:**  
[https://aws.amazon.com/fargate/](https://aws.amazon.com/fargate/)

**Incorrect options:**

- **Amazon Elastic Container Service (Amazon ECS) - EC2 launch type** - O Amazon Elastic Container Service (Amazon ECS) é um serviço de gerenciamento de contêineres altamente escalável e rápido que facilita a execução, parada e gerenciamento de contêineres Docker e permite que você execute facilmente aplicações em um cluster gerenciado de instâncias Amazon EC2. Ao contrário do AWS Fargate, este não é um serviço totalmente gerenciado e você precisa gerenciar os servidores subjacentes.

- **AWS Lambda** - O AWS Lambda é um serviço de computação que permite executar código sem provisionar ou gerenciar servidores. O AWS Lambda executa seu código apenas quando necessário e escala automaticamente, de algumas solicitações por dia para milhares por segundo. O AWS Lambda não suporta a execução de aplicações em contêineres.

- **Amazon Elastic Compute Cloud (Amazon EC2)** - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço da web que fornece capacidade de computação segura e redimensionável na nuvem, faturamento por segundo e acesso ao sistema operacional subjacente. Ele é projetado para facilitar a computação em nuvem em escala na web para desenvolvedores. A manutenção do servidor e seu software deve ser feita pelo cliente, então essa opção é descartada.

**Reference:**  
[https://aws.amazon.com/fargate/](https://aws.amazon.com/fargate/)

**Domínio:**  
Technology
