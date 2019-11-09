# AWS-CloudFormations
The following AWS CloudFormation templates can be used for provisioning AWS Big Data, IoT and ML resources.

## KMSKeyTemplate.yaml:
Use this template for provisioning KMSKeys. 

# S3BucketTemplate.yaml
Use this template to create S3 bucket. 
Note: The bucket will contain a lifecycle policy to delete all objects after x number of days therefore use with caution!

# NetworkStackWithBastion.yaml:
Use this template to create a VPC spanning two AZs. Each AZ will contain a public and a private subnet with route to Internet using an IGW.
The template also creates a Linux Bastion host and a Windows Bastion host for interacting with resources deployed in VPC.

# ElasticSearchTemplate.yaml:
Use this template for provision an EMR cluster. The cluster will be deployed in the VPC created using NetworkStackWithBastion.yaml template.

# GlueIBaseTemplate.yaml:
Use this template to create IAM roles, security configuration, Glue Database and Glue VPC endpoint.

# RedShiftTemplate.yaml
Use this template to create a private or public Redshift cluster in the VPC created using NetworkStackWithBastion.yaml template.

# ElasticSearchTemplate.yaml
Use this template to create a ElasticSearch Domain. 

# KinesisStreamTemplate.yaml
Use this template to create Kinesis Data Stream.

# KinesisFirehoseTemplate.yaml
Use this template to create Kinesis Firehose.

# KinesisAnalyticsBaseTemplate.yaml 
Use this template to create IAM Role to be used by KinesisAnalytics applications

# SagemakerTemplate.yaml
Use this template to create SageMaker Notebook.

PS: The CloudFormation templates are provided as-is and are not intended for Production use.
