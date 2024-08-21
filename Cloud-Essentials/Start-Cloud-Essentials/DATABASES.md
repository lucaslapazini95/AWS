# DATABASES

### Which of these are attributes of Amazon RDS? (Select THREE.)

- ~~The service will launch the primary database in the primary Availability Zone.~~
- **Amazon RDS can be used to launch the database in the Multi-AZ configuration if you want to deploy it for high availability (HA).**
- **Amazon RDS is compatible with multiple engines and lets you launch the Amazon Aurora database.**
- ~~Amazon RDS is used to launch the database in the Single-AZ configuration if you want to deploy it for high availability (HA).~~
- **You can set up, operate, and scale a relational database in the cloud with just a few clicks.**
- ~~With Amazon RDS you can set up a fully managed, serverless, nonrelational database.~~

> **Explanation:**
> Amazon RDS can be used to launch the database in the Multi-AZ configuration if you want to deploy it for HA. Amazon RDS is compatible with multiple engines and lets you launch the Amazon Aurora database. With Amazon RDS, you can set up, operate, and scale a relational database in the cloud with just a few clicks. However, the service will launch the primary and standby databases in different Availability Zones and set up synchronous replication of data and failover strategy. If the primary database goes down, the standby picks up the traffic. Also, with Amazon DynamoDB, not Amazon RDS, you can set up a fully managed, serverless, nonrelational database.

---

### Which explanation best explains why you would choose Amazon Neptune?

- **Neptune can simplify the setup and running of your graph databases.**
- ~~Neptune is not used for social media.~~
- ~~Neptune is not used for fraud detection.~~
- ~~Neptune is a great choice when you're looking for seamless database scalability.~~

> **Explanation:**
> Amazon Neptune can simplify the setup and running of your graph databases. Amazon Neptune can be useful for social media. Amazon Neptune can be useful for fraud detection.

---

### What are some key Amazon DynamoDB features? (Select TWO.)

- **With DynamoDB, you can achieve single-digit millisecond performance at any scale.**
- ~~DynamoDB is ideal for workloads that involve working with databases, unflexible schemas, and high throughput (multiple read/write requests).~~
- ~~DynamoDB will not automatically scale to meet your demand.~~
- **DynamoDB is a fully managed, serverless, nonrelational database.**
- ~~DynamoDB is not the best choice if you are looking for seamless database scalability.~~

> **Explanation:**
> With DynamoDB, you can achieve single-digit millisecond performance at any scale. DynamoDB is a fully managed, serverless, nonrelational database. However, DynamoDB will automatically scale to meet demand. DynamoDB is ideal for workloads that involve working with databases, flexible schemas, and high throughput (with minimal read/write requests).
