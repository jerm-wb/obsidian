# What is EC2?
## Elastic Compute Cloud
Two storage options
### EBS - Elastic Block Store
Directly attached, reliable. Use it for storing your main data
#### Key features
- Highly available and durable
	- Suited for EC2 instances
	- Ensures data is preserved even if the instance crashes
- Scalable
	- Expands on the fly without any downtime
- Snapshot
	- Can take backups and also use these backups to create new volumes
### EFS - Elastic File System
Can serve many EC2 instances and other AWS services
#### Key features
- Fully managed
	- Removes complexity of deploying and maintaining file systems
- Automatic scaling
	- Automatically scales on demand without disrupting applications
- Concurrency
	- Multiple EC2 instances can access an EFS simultaneously
#### Use cases
- Applications with growing storage needs (content management, web serving)
- Data analytics applications
- Development and testing environments
### Instance Stores
Temporary. If you shut down the instance it's data is gone
#### Key Features
- High I/O Performance
- Temporary Storage
- No extra cost
	- Come as part of the instance
#### Use cases
- Temporary storage of cache and buffers
- Write and discard large amounts of data
- Storage for applications that replicate data across multiple instances


# 💡 Exam Tips
> [!important]
> Remember:
> - EBS is block-level storage used with EC2 instances
> - EFS is a file system scalable across multiple EC2 instances
> - Instance store provides temporary block level storage directly attached to the instance
> - While EBS and EFS have costs associated with the amount of storage provisioned, instance store comes at no additional cost, as it's included in the instance price.
> - EBS is particularly known for its provisioned IOPS, EFS is scalable file storage, and instance store for a high I/O operation's suitable for temporary data.

---
*Notes Last Updated: 2025-02-21 15:30*