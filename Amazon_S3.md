# Amazon S3

Amazon S3 (Simple Storage Service) is a scalable, high-speed, web-based cloud storage service offered by Amazon Web Services (AWS). It is designed to store and retrieve any amount of data, at any time, from anywhere on the web.

---

## Key Features of Amazon S3:

### 1. Object Storage
- S3 stores data as objects within buckets.
- Each object includes the data itself, a key (filename), and metadata.

### 2. Scalable and Durable
- Designed for 99.999999999% (11 nines) durability.
- Automatically replicates data across multiple Availability Zones.

### 3. Secure
- Supports encryption at rest and in transit.
- Integrates with AWS Identity and Access Management (IAM) for access control.

### 4. Access Management
- Fine-grained access controls via bucket policies, ACLs, and IAM roles.

### 5. Storage Classes
- Different classes based on access patterns and cost:
  - S3 Standard (frequent access)
  - S3 Intelligent-Tiering
  - S3 Standard-IA (Infrequent Access)
  - S3 One Zone-IA
  - S3 Glacier / Glacier Deep Archive (for archival)

### 6. Versioning
- Keeps multiple versions of an object for backup and recovery.

### 7. Event Notification & Data Lifecycle
- Can trigger Lambda functions, SNS, or SQS on object events.
- Supports lifecycle rules to transition or delete data automatically.

---

## Example Use Cases:
- Backup and restore
- Big data analytics
- Hosting static websites
- Storing media files (images, videos)
- Data lake storage
- Disaster recovery

---

## Simple Example:
To upload a file to S3 using AWS CLI:

```bash
aws s3 cp myfile.txt s3://my-bucket-name/
