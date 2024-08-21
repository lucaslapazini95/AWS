# STORAGE

### What are the two main benefits of Amazon Elastic Block Store (Amazon EBS)? (Select TWO.)

- ~~You use one main drive type.~~
- **Pay only for what you provision. As with Amazon EC2, you have control over how much and what type of solid-state drive (SSD) or hard disk drive (HDD) storage you provision. And if you need to scale it, you can modify your volume.**
- **Data is very important. So you have the opportunity to take incremental snapshots of the volume, and the snapshots are encrypted. You can keep them indefinitely and have the opportunity to recover the volumes when needed.**
- ~~Persistent network-attached block storage for instances does not persist after the EC2 instance to which this storage is attached is terminated.~~
- ~~When you need a serverless shared file system, you can use Amazon EBS.~~

> **Explanation:**
> Pay only for what you provision. As with Amazon EC2, you have control over how much and what type of solid-state drive (SSD) or hard disk drive (HDD) storage you provision. And if you need to scale it, you can modify your volume. Data is very important. So you can take incremental snapshots of the volume, and the snapshots are encrypted. You can keep them indefinitely and have the opportunity to recover the volumes when needed. However, Amazon EBS uses different drive types. Persistent network-attached block storage for instances can persist even after the EC2 instance to which this storage is attached is terminated. When you need a serverless shared file system, you can use Amazon Elastic File System (Amazon EFS), not Amazon EBS.

---

### What are three Amazon S3 use cases? (Select THREE.)

- ~~Creating cloud non-native applications~~
- **Building a data lake**
- **Content storage and distribution**
- ~~Deleting backup~~
- ~~Releasing critical data~~
- **Archiving data**

> **Explanation:**
> Building a data lake, archiving data, and content storage and distribution are Amazon S3 use cases. Backup and archiving is also an Amazon S3 use case, so you make sure your archives will not be deleted for a period of time (vault lock). Restoring critical data is an Amazon S3 use case. Creating cloud-native applications is an Amazon S3 use case.

---

### Which of these are reasons to use Amazon Elastic File System (Amazon EFS)? (Select TWO.)

- **When you need to build high-performing and cost-optimized file systems on AWS benefitting from the built-in-elasticity, durability, and availability**
- ~~When you don't need storage classes~~
- ~~When full AWS compute integration is not a priority~~
- **When you need a serverless shared file system**
- ~~Use fully managed EFS because it is not compatible with Network File System (NFS) or Server Message Block (SMB).~~

> **Explanation:**
> A reason for using Amazon EFS is when you need to build high-performing and cost-optimized file systems on AWS, benefitting from the built-in elasticity, durability, and availability. A reason for using Amazon EFS is when you need a serverless shared file system. However, Amazon EFS is used when you need four storage classes and when full AWS compute integration is a priority. Fully managed EFS is compatible with Network File System (NFS) and Server Message Block (SMB).
