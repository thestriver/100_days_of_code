## AWS Certified Solutions Architect – Associate
(SAA-C02) 
To Delete: Use A Cloud Guru 7 days trial after reading

![](assets/images/saa/domain.png)

720/1000 - 65 Questions

-  Define a solution using architectural design principles based on customer requirements.
-  Provide implementation guidance based on best practices to an organization throughout the lifecycle of a
project

**Whitepapers**


Study tip: Focus on the following whitepapers

AWS Well-Architected webpage : https://aws.amazon.com/architecture/well-architected/


Study tip: Focus on the following FAQs

Amazon EC2(https://aws.amazon.com/ec2/faqs/) || Amazon S3(https://aws.amazon.com/s3/faqs/) || Amazon VPC(https://aws.amazon.com/vpc/faqs/) || Amazon Route 53(https://aws.amazon.com/route53/faqs/) || Amazon RDS(https://aws.amazon.com/rds/faqs/) || Amazon SQS(https://aws.amazon.com/sqs/faqs/)

Readinesss: https://www.aws.training/Details/Curriculum?id=20685

---

<h2>S3: Simple Storage Service - Scalable storage in the cloud</h2>
You can store 0 - 5 terabytes. Amazon S3 are managed at a regional level. Note: Amazon S3 is a global namespace but you still create your buckets within a region

- S3: object storage / S3 Glacier: low cost long-term archive and backup / Storage Gateway: Hybrid cloud storage with local caching / Snowcone (8TB)/ Snowballs Edge (50TB(compute-optimized) and 80TB(storage optimized) versions) / ~~Snowball Edge (100TB)~~, Snowmobile (100PB)

- S3 Intelligent-Tiering monitors access patterns of objects and automatically moves them between the S3 Standard and S3 Standard-IA storage classes. It is not designed for archival data.
- S3 Standard-IA is ideal for data that is infrequently accessed but requires high availability when needed.

- Buckets are private by default and access is controlled by **Bucket Policies** and **ACL**

- Encryption: a. Server side encryption(SSE) is done using S3 Managed Keys. SSE-S3 AES (key is handled using AES-256 Algorithm), SSE KMS (envelope encrption) & SSE C- where the customer provides the key (N.B To upload an object with a customer-provided encryption key (SSE-C), use the AWS CLI, AWS SDK, or Amazon S3 REST API.)
b. Client side encryption - here you encrypt your files yourself before uploading to s3

- Data Consistency: a. New Objects(PUTS) (_read after write consistency_) b. Overwrite(PUTS) or Delete (DELETE) - (_eventual consistency_) N.B Delete can only be done by a root user.

- CRR - (Cross Region Replication) - after upload, object is **automatically replicated** to other regions. Versioning has to be turned on for CRR replication to be done to another AWS account. You can't disable versioning after enabling it. It can only be suspended. MFA delete can also be done with the CLI. 

- Transfer Acceleration: CloudFront's distributed edge locations are used for secure and safe transfer of files over long distances. A distinct url is used by the users and the Amazon backbone network is used for routing data.

- Presigned URLS - generated using AWS **CLI or SDK** and provides temp access to private objects


![](assets/images/saa/s3classes.png)

