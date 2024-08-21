### 1) An enterprise is heavily dependent on their on-premises data center and are considering a potential migration to the cloud. One of the major concerns is security.

### How does AWS maintain the security and privacy of customer data?

- **AWS fulfills security criteria through certifications, accreditation, and other third-party attestations.**
- ~~AWS trains its users on how to manage services and set up appropriate security protocols.~~
- ~~AWS relies on its customer to fully maintain its data security.~~
- ~~AWS provides different pricing models for all uses.~~

> **Explanation:**
> AWS ensures the security and privacy of customer data through rigorous adherence to security criteria, which are validated through various certifications, accreditations, and third-party attestations. This forms a core part of AWS's commitment to secure cloud computing, complementing the shared responsibility model where AWS secures the infrastructure and customers manage their data and application security.

---

### 2) Your customer has recently moved to the AWS Cloud. The Finance department has reached out to the IT director for assistance in breaking down the costs on the invoice and identifying the costs source. You have been asked to find a way to get the cost details and usage across a variety of different views based on filters.

### Which AWS service will BEST assist to identify various expenditures?

- ~~AWS Budgets~~
- ~~AWS Cost Anomaly Detection~~
- ~~Amazon QuickSight~~
- **AWS Cost Explorer**

> **Explanation:**
> Using **AWS Cost Explorer**, you can evaluate your AWS services (e.g., EC2, S3, RDS, etc.) costs and usage across a variety of different views based on filters. This tool allows detailed analysis and reporting, helping the Finance department understand and manage cloud expenditures effectively.

---

### 3) Your company has a Business Intelligence (BI) team and they have been tasked to build a detailed overall cost intelligence dashboard to visualize cost consumption and provide insights into the trends. They need the source data from AWS to build the dashboard.

### Which report will provide the source data to build a BI dashboard?

- ~~AWS Budget report~~
- ~~Reserved Instance report~~
- **Cost and Usage Report**
- ~~Savings Plan report~~

> **Explanation:**
> The **Cost and Usage Report (AWS CUR)** provides the most comprehensive set of cost and usage data available in AWS. This report is ideal for the BI team to extract detailed data, visualize cost consumption, and analyze trends for building a robust dashboard.

---

### 4) You need a way to visualize how the AWS bill has changed over the last 6 months and determine which services are billing the most.

### What AWS tool will MOST easily allow you to see this information?

- ~~AWS Trusted Advisor~~
- ~~AWS Billing~~
- **AWS Cost Explorer**
- ~~AWS Budgets~~

> **Explanation:** > **AWS Cost Explorer** is the correct tool for visualizing how your AWS bill has changed over time, including the ability to analyze costs by service. It offers interactive graphs and filters that allow you to view cost data over a specified period, such as the last 6 months.
>
> The option you chose, **AWS Billing**, is primarily used for understanding your monthly bill, managing invoices, and setting up billing preferences. While it provides a summary of charges, it does not offer the detailed trend analysis and service-specific breakdowns that **AWS Cost Explorer** provides.

---

### 5) A financial institution wants to host their infrastructure on the AWS Cloud. They are concerned about compliance requirements.

### What service can be used to review the AWS compliance reports?

- ~~AWS WAF~~
- ~~Amazon GuardDuty~~
- ~~Amazon Inspector~~
- **AWS Artifact**

> **Explanation:** > **AWS Artifact** is the correct service for reviewing AWS compliance reports. It provides on-demand access to AWS security and compliance documents, including certifications, attestations, and agreements.
>
> The other options you considered are focused on security rather than compliance documentation:
>
> - **AWS WAF** is a web application firewall that helps protect your web applications from common web exploits but does not provide compliance reports.
> - **Amazon GuardDuty** is a threat detection service that monitors for malicious or unauthorized behavior within your AWS environment.
> - **Amazon Inspector** is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS but does not provide access to compliance reports.

---

### 6) Your organization has a savings plan and you have been tasked to monitor and report when savings plan utilization drops below a certain threshold.

### Which tool would help you achieve this with the LEAST amount of management overhead?

- ~~AWS Billing~~
- ~~AWS Trusted Advisor~~
- ~~AWS Cost Explorer~~
- **AWS Budgets**

> **Explanation:** > **AWS Budgets** is the tool that provides the least amount of management overhead for monitoring Savings Plan utilization. With AWS Budgets, you can set up alerts to notify you when utilization or coverage drops below a specified threshold. These alerts can be configured to trigger based on daily, monthly, quarterly, or annual thresholds.
>
> The other tools, while useful, do not provide the same level of automated alerting for specific utilization thresholds:
>
> - **AWS Billing** provides insights into your billing details but does not offer specific alerting capabilities for Savings Plan utilization.
> - **AWS Trusted Advisor** offers best practices checks for your AWS environment, but it does not provide specific alerts for Savings Plan utilization.
> - **AWS Cost Explorer** helps analyze your cost and usage data but does not offer direct alerting features for Savings Plan utilization thresholds.

---

### 7) A Web application company is migrating their on-premises infrastructure to the AWS Cloud. Their IT team consists of the CTO, Infrastructure/Cloud Architect, System Administrator, and Network Administrator to support their on-premises infrastructure.

### Who in this organization is responsible for building a cloud migration strategy?

- ~~Network Administrator~~
- ~~CTO~~
- ~~System Administrator~~
- **Cloud Architect**

> **Explanation:**
> The **Cloud Architect** is responsible for building a cloud migration strategy. Their role includes designing and planning the transition from on-premises infrastructure to the cloud, ensuring that the migration is cost-effective and meets the required high availability and performance standards.
>
> - **Network Administrator** focuses on managing network infrastructure, not on building migration strategies.
> - **CTO** (Chief Technology Officer) oversees technology strategy but is not typically involved in the detailed planning of cloud migrations.
> - **System Administrator** manages day-to-day operations of systems but does not usually create migration strategies.

---

### 8) Your company wants to host its infrastructure and data in an AWS region.

### Which requirement helps you determine the region to host your data?

- ~~Location of data centers~~
- ~~Lack of natural disasters~~
- ~~Hardware brands~~
- **Compliance**

> **Explanation:** > **Compliance** is the primary requirement that helps determine the AWS region for hosting data. Compliance requirements often include data sovereignty and legal regulations that dictate where data must be stored and processed. Ensuring that the chosen AWS region meets these compliance needs is crucial for adhering to legal and regulatory standards.
>
> - **Location of data centers** is less relevant than compliance, as AWS regions are chosen based on compliance and other strategic considerations.
> - **Lack of natural disasters** is a consideration but not as critical as compliance requirements for determining the region.
> - **Hardware brands** are not a factor in choosing an AWS region, as AWS provides standardized hardware across its regions.

---

### 9) A company has its application servers deployed in an AWS region in Amazon VPCs with private and public subnets. The application servers are placed in private subnets and often initiate requests to the internet.

### Which solution would BEST accomplish this task?

- ~~Create an internet gateway in the private subnet in the region.~~
- ~~Create a NAT gateway in a public subnet in one Availability Zone in the region, with a default route in the private subnet pointing to it.~~
- ~~Create a Network Access Control List to filter traffic to the private subnet.~~
- **Create a NAT gateway in a public subnet of each Availability Zone in the region, with a default route in the private subnet pointing to it.**

> **Explanation:**
> To allow instances in private subnets to initiate requests to the internet while maintaining their security and privacy, you need a NAT gateway. Placing a NAT gateway in a public subnet of each Availability Zone ensures high availability and fault tolerance. This setup allows instances in private subnets to route outbound traffic to the internet while keeping the private subnets isolated.
>
> - **Creating an internet gateway in the private subnet** is incorrect because an internet gateway must be attached to the VPC and used with public subnets. Private subnets need a NAT gateway for internet access.
> - **Creating a NAT gateway in only one Availability Zone** may not provide high availability. Deploying NAT gateways in multiple Availability Zones is recommended to ensure reliability.
> - **Creating a Network Access Control List (NACL)** does not address the need for outbound internet access for instances in private subnets.

---

### 10) Your organization is planning to migrate its on-premises infrastructure to the cloud. As part of this move, you want to ensure that the cloud technology you acquire is sustainable and environmentally friendly.

### Which is a key sustainability consideration for a successful cloud acquisition strategy?

- ~~Prioritize on-premises efficiencies, as cloud computing cannot be sustainable due to the energy consumption required to service millions of customers.~~
- ~~Ignore the environmental impact of cloud computing, as it is not a significant factor in sustainability.~~
- ~~Prioritize the lowest price over sustainability, as cost savings is always the most important consideration.~~
- **Choose a cloud service provider that focuses on energy efficiency and innovation to reduce its carbon footprint.**

> **Explanation:**
> Choosing a cloud service provider that emphasizes energy efficiency and innovation to reduce its carbon footprint is crucial for a sustainable cloud acquisition strategy. For example, AWS actively works towards using renewable energy sources and improving energy efficiency in its data centers, which aligns with environmental sustainability goals.
>
> - **Prioritizing on-premises efficiencies** is incorrect because cloud computing providers often have more resources to implement energy-saving technologies than most on-premises infrastructures.
> - **Ignoring the environmental impact** is not a responsible approach as sustainability is an important aspect of modern IT strategies.
> - **Prioritizing the lowest price** over sustainability disregards long-term environmental and ethical considerations, which are increasingly important in technology decisions.
