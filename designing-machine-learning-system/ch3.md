# Chapter 3. Data Engineering Fundamentals

Knowing how to collect, process, store, retrieve, and process an increasingly growing amount of data is essential to people who want to build ML systems in production.

## Data Sources

- user input data (text, images, videos, uploaded files, etc)
- system-generated data (logs and system outputs such as model predictions.)
  - Data storage
  - Data lifecycle
  - Regulations
- internal databases
- third-party data

## Data Formats

- The process of converting a data structure or object state into a format that can be stored or transmitted and reconstructed later is data serialization
- JSON
- CSV
- Parquet - Hadoop, Amazon Redshift
- Avro - Haddop
- Protobuf - Google , Tensorflow
- Pickle - Python

Row-Major Versus Column-Major Format

- column-major  - consecutive elements in a column are stored next to each other.
- row major - consecutive elements in a row are stored next to each other

Text Versus Binary Format

- Binary files are more compact

## Data Models

- Relational Model
- NoSQL
  - Document model
  - Graph model

## Structured Versus Unstructured Data

|                    | Structured data                                      | Unstructured data                                     |
|--------------------|------------------------------------------------------|-------------------------------------------------------|
| Schema             | Clearly defined                                      | Data doesn’t have to follow a schema                  |
| Search & Analysis  | Easy to search and analyze                          | Fast arrival                                          |
| Data Handling      | Can only handle data with a specific schema         | Can handle data from any source                      |
| Impact of Schema Changes | Changes will cause a lot of troubles           | No need to worry about schema changes (yet), as the worry is shifted to the downstream applications that use this data |
| Storage            | Stored in data warehouses                           | Stored in data lakes                                  |

## Data Storage Engines and Processing

- Transactional processing
  - ACID properties
    - Atomicity
    - Consistency
    - Isolation
    - Durability
  - need to be processed fast (low latency)
  - OLTP (Online Transaction Processing)

- Analytical processing
  - OLAP (Online Analytical Processing)
  - need to process large amounts of data (high throughput)

- ETL: Extract, Transform, and Load
  - Extract: data is extracted from the source
  - Transform: data is transformed into a format that is suitable for the target system
  - Load: data is loaded into the target system

## Modes of Dataflow

- through databases
- throguh services (RESTful API)
- through  real-time data processing systems  (Kafka, RabbitMQ)

## Batch Processing Versus Stream Processing

- Batch processing
  - process data in batches
  - Hadoop, Spark
- Stream processing
  - process data in real-time
  - Kafka, Flink
