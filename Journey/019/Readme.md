# AWS Cloud Practitioner Essentials: Module 5: Storage and Databases

Module 5 introduces AWS storage, of which there are three types and various databases within Amazon Relational Database Service.

Storage is included with AWS EC2 instaces, however the instance stores only provide a temporary block storage for the lifecycle of that EC2, meaning that data will be lost if an instance stops.


## Storage

### 1. Amazon Elastic Block Store (EBS)
AWS EBS is a service that provides block-level storage volumes that can be used with EC2 instances, to ensure that data remains available. To ensure availability EBS volumes must be backed up. Incremental backups are done using snapshots of only blocks of data that have changed, which is leaner than full back ups. 

<p align="center">
  <image src="AWS-EBS-snapshots.png">
</p>

### 2. Amazon Simple Storage Service (S3)
S3 is **object storage** where each object is a file; document, image, video or other. Each objects consists of data, metadata and key.

<p align="center">
  <image src="S3-object-storing.png">
</p>

**Use Cases**
- relational & non-relational databases
- enterprise applications
- containerised applications
- bigdata analytics engines
- file systems
- media files

AWS Simple Storage Service (S3) offers six storage classes/tiers:
1. S3 Standard - frequent accessed data with high availbility via 3 availability zones
2. S3 Standard-Infrequent Access (S3 Standard-IA) - infrequently accessed with high availiability 
3. S3 One Zone-Infrequent Access (S3 One Zone-IA) - infrequently accessed in a single zone
4. S3 Intelligent-Tiering - ideal for data with varied access. Data automatically changes tiers, for a fee
5. S3 Glacier - ideal for data archiving with quick retreival
6. S3 Glacier Deep Archive - ideal for archiving with slower retrival (12 hrs)


### 3. Amazon Elastic File System (EFS)
Amazon EFS is a file system with auto scaling. It's serverless so no need to worry about provisioning and managing the storage. Four classes/tiers are available with Elastic File System (EFS):
1. EFS Standard
2. EFS Standard-IA
3. EFS One Zone
4. EFS One Zone-IA 

**Use Cases**
- containers and serverless persistant file storage
- enterprise applications
- web applications
- application development & testing
- Content Management Systems (CMS)
- file systems
- media files

<p align="center">
  <image src="AWS-EFS.png">
</p>

## Databases

Amazon has a suite of relational and non-relational databases.

### Relational Databases 

**Amazon Relational Database Service (RDS)** offers:
- Amazon Aurora
- PostgresSQL
- MySQL
- MariaDB
- Oracle database
- Microsoft SQL Server

### Non-relational databases
- Amazon DynamoDB ***uses key-values pairs to store data***
- Amazon Redshift ***data warehouse for big data analytics***


## Additional Databases
- Amazon DocumentDB
- Amazon Neptune ***is a graph DB service***
- Amazon Quantum Ledger Database (Amazon QLDB) ***is a ledgerDB***
- Amazon Managed Blockchain 
  ***is a service used to create and manage blockchain networks with open sourced frameworks***
- Amazon ElastiCache ***adds caching layers on top of DBs***
- Amazon DynamoDB Accelerator ***is a memory cache for DynamoDB***

# End of Module 5: Databases