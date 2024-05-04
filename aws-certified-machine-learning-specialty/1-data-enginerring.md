# Data engineeering

Step 1: Create data repositories for machine learning

- AWS Lake formation
    ETL , Acccess control, source crawlers
    Output to other services
    Central data catalogue
    HIPPA Complicance/ Security of data
    Security is biggest point of lake formation (FGAC Fine Grained Access Control)
    AWS Glue
    AWS Redshift

- AWS S3 bucket
    Can story anything, extremely versatile
    S3 lifecycle configuration
        Move old data to glacier
        Expiration
    S3 data storage options
        Storage classe
        Based on data access frequency

- AWS FSx for Lustre
- Amazon EFS
    Shared FS
- Amazon EBS volumnes
    Similar to Physical hard drive attached to instance
    independent of EC2 instance

Step 2: Identify and implement a data ingestion solution

Mechanism
    - Batch Processing
        Bulk of data  ingestion

    - Stream Processing
        Ingested as soon available

Kind of data:
    - images
    - Relational
    - Sensory

Tools avaiable
    - Amazon Kinesis Data Stream
        Serverless streaming data service
        Pay as you use
        Build in transformations

    - Amazon Kinesis Data Firehouse
        ETL
        Custom data transformation using AWS Lambda
        Stream data into S3
        uswed to batch data as it is streamed in real time

    - Amazon Kinesis Data Analytics
        Time series analytics
        

    - Amazon Kinesis Video Streams
        Video processing
        Industrial processing
        IoT solutions
    
    - AWS Glue
        ETL Service
        Good for batch ingestion

    
    - Apache Kafka
        Open source 
        Event processing

    
    - AWS Data Migration Service (AWS DMS)
      Good for batch ingestion

Step 3: Identify and implement a data transformation solution

    - Apache Spark on Amazon EMR
        Managed framework to process huge amount of data
        Great for HPC
        EMR??
        EMR Studio
        EMR notebooks
        Spark sreaming on EMR
        
    - Apache Spark and Amazon SageMaker
        Apache Spark for preprocessing data
        Sagemaker for model training and hosting

    - AWS Glue
        ETL Service
        Run spark jobs on data stored in S3
        can provide metadata discovery and management
