# Data and Analytics for IoT

## Hadoop Architecture and Components

### Core Components

- **HDFS (Hadoop Distributed File System)**

  - NameNode: Manages filesystem namespace
  - DataNode: Stores and retrieves blocks
  - Block replication for reliability

- **MapReduce**
  - Programming model for large-scale data processing
  - Map phase: Data transformation
  - Reduce phase: Data aggregation
  - YARN for resource management

### Hadoop Ecosystem

- **Data Ingestion**
  - Kafka: Real-time streaming
  - Flume: Log aggregation
- **Processing**
  - Spark: In-memory processing
  - Storm: Real-time computation
  - Flink: Stream/batch processing
- **Storage**
  - HBase: Column-oriented database
  - Cassandra: Distributed database

## Edge Analytics Integration

- Processing close to data source
- Reduced latency and bandwidth usage
- Real-time decision making
- Integration with Hadoop for long-term storage
