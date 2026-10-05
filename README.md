# Awesome-Real-Time-Stream-Analytics

# Top Real-Time Stream Analytics Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Event Stream Processing, Complex Event Processing & Stream Analytics*  
**Last updated: October 2026**

This repository tracks notable **commercial stream analytics platforms** and **open-source projects** that process, analyze, and act on data in motion — from real-time dashboards and anomaly detection to continuous ETL and event-driven applications.

**Examples** include Azure Stream Analytics, Amazon Kinesis Analytics, Google Cloud Dataflow, Confluent Cloud, Apache Flink Cloud, Decodable, Upsolver, Databricks Streaming, StreamNative, and Hazelcast (the category leaders).

**Open-source emphasis**: Real-time stream analytics is a domain where open-source leads. **Apache Flink** is the de facto standard for stateful stream processing, with **Kafka Streams** and **Apache Spark Structured Streaming** as core alternatives. **RisingWave** and **Materialize** bring streaming SQL databases, while **Arroyo** delivers a modern Rust-based engine. **Benthos** and **Vector** handle stream pipelines without code. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Azure Stream Analytics](https://azure.microsoft.com/en-us/products/stream-analytics/)**  
  Microsoft's fully managed real-time analytics service with SQL-like query language, built-in ML functions, and native Azure integration. **The easiest on-ramp for Azure users** — no infrastructure management.

- **[Amazon Kinesis Analytics](https://aws.amazon.com/kinesis/data-analytics/)**  
  AWS's managed service for real-time analytics on streaming data using SQL or Apache Flink. **The standard for AWS-native stream processing** — integrates with Kinesis, Lambda, and S3.

- **[Google Cloud Dataflow](https://cloud.google.com/dataflow)**  
  Google's fully managed stream and batch processing based on Apache Beam. **The most unified batch/stream model** — same code for both.

- **[Confluent Cloud](https://www.confluent.io/confluent-cloud/)**  
  **The leading managed Kafka platform** with ksqlDB for stream processing, Flink for stateful operations, and connectors. **The enterprise standard for event streaming** — from Kafka creators.

- **[Apache Flink Cloud](https://flink.apache.org/)**  
  Managed Flink offerings from AWS (Managed Flink), Confluent, and others. **The reference implementation for stateful stream processing** — used by Uber, Netflix, and Alibaba.

- **[Decodable](https://www.decodable.co/)**  
  Fully managed stream processing platform with SQL-based pipelines and no infrastructure management. **The simplest path to streaming ETL** — built on Apache Flink.

- **[Upsolver](https://www.upsolver.com/)**  
  Stream data lake platform for real-time ingestion, transformation, and analytics. **The best for streaming into data lakes** — no code required.

- **[Databricks Streaming](https://www.databricks.com/)**  
  Unified analytics platform with Spark Structured Streaming and Delta Live Tables. **The standard for lakehouse streaming** — batch and stream unified.

- **[StreamNative](https://streamnative.io/)**  
  Managed Apache Pulsar and Apache Flink platform from the creators of Pulsar. **The enterprise standard for Pulsar** — multi-tenancy and geo-replication.

- **[Hazelcast](https://hazelcast.com/)**  
  In-memory data grid with stream processing capabilities. **The best for low-latency stateful processing** — co-located compute and data.

## Open-Source GitHub Projects

- **[Apache Flink](https://github.com/apache/flink)**  
  **The de facto standard for stateful stream processing**, Apache-2.0 licensed with **24,000+ GitHub stars** . **True event-at-a-time processing** with exactly-once semantics, event-time processing, and sophisticated windowing . **Savepoints for versioned state migration**, **backpressure monitoring**, and **TensorFlow/PyTorch integration for streaming ML** . Handles **millions of events per second** with millisecond latency . **The engine behind Alibaba's Singles' Day (2.5 billion events/second)** and Uber's real-time pricing . **Best for mission-critical, stateful stream processing at scale** — the most capable open-source engine.

- **[Apache Kafka Streams](https://github.com/apache/kafka)**  
  **The standard for stream processing within Kafka**, Apache-2.0 licensed with **28,000+ GitHub stars** (Kafka project) . **No separate cluster required** — runs as a library in your application . **Exactly-once semantics, event-time processing, and interactive queries** . **The simplest path to stream processing for Kafka users** — no additional infrastructure . **Best for Kafka-native applications** — when you're already using Kafka, Streams is the natural choice.

- **[Apache Spark Structured Streaming](https://github.com/apache/spark)**  
  **The unified batch and stream processing engine**, Apache-2.0 licensed with **39,000+ GitHub stars** . **Same API for batch and streaming** — DataFrame/Dataset API . **Micro-batch processing with exactly-once semantics** — higher latency than Flink but easier migration from batch . **Best for teams already using Spark** for batch processing — reuse code and skills.

- **[ksqlDB](https://github.com/confluentinc/ksql)**  
  **Streaming SQL engine for Kafka**, Confluent Community License (not OSI) . **SQL interface for Kafka Streams** — no Java/Scala code required . **Continuous queries, materialized views, and pull queries** . **Best for SQL-proficient teams** wanting stream processing without coding.

- **[RisingWave](https://github.com/risingwavelabs/risingwave)**  
  **Streaming database for real-time analytics**, Apache-2.0 licensed with **7,000+ GitHub stars** . **PostgreSQL-compatible SQL** — connect with existing drivers . **Streaming SQL with materialized views** — query real-time data like a database . **S3 as primary storage** — separation of compute and storage for cost efficiency . **Best for streaming SQL with database-like experience** — the most PostgreSQL-compatible streaming database.

- **[Materialize](https://github.com/MaterializeInc/materialize)**  
  **Streaming database built on Timely Dataflow**, BSL licensed (free for most uses) . **PostgreSQL-compatible** — standard SQL with materialized views . **Strong consistency and exactly-once semantics** . **Best for streaming SQL with strong consistency guarantees** — used for real-time dashboards and monitoring.

- **[Arroyo](https://github.com/ArroyoSystems/arroyo)**  
  **Modern stream processing engine in Rust**, Apache-2.0 licensed with **4,000+ GitHub stars** . **SQL-based pipelines** — no JVM required . **Serverless deployment model** — scales to zero . **Kafka, Pulsar, and Delta Lake sources** . **Best for teams wanting lightweight, modern stream processing** — Rust performance without JVM overhead.

- **[Apache Beam](https://github.com/apache/beam)**  
  **Unified programming model for batch and stream**, Apache-2.0 licensed with **8,000+ GitHub stars** . **Runs on Flink, Spark, Dataflow, and Samza** — portability across engines . **Java, Python, Go, and SQL APIs** . **Best for portable pipelines** — write once, run on any engine.

- **[Benthos (Redpanda Connect)](https://github.com/redpanda-data/connect)**  
  **Stream processing without code**, Apache-2.0 licensed with **8,000+ GitHub stars** . **Declarative YAML configuration** for streaming ETL . **Hundreds of connectors** — Kafka, MQTT, HTTP, databases, and more . **Best for data engineers wanting stream pipelines without programming**.

- **[Vector](https://github.com/vectordotdev/vector)**  
  **High-performance observability data pipeline**, MPL-2.0 licensed with **18,000+ GitHub stars** . **Collect, transform, and route logs, metrics, and events** . **Rust-based for performance** — single binary, low resource usage . **Best for observability and log streaming pipelines** — the leading open-source alternative to proprietary log routers.

- **[Apache Samza](https://github.com/apache/samza)**  
  **Distributed stream processing framework from LinkedIn**, Apache-2.0 licensed . **Kafka-native with YARN/Kubernetes deployment** . **Best for LinkedIn-scale stream processing** — mature but less active than Flink.

- **[Apache Storm](https://github.com/apache/storm)**  
  **Distributed real-time computation system**, Apache-2.0 licensed . **The original stream processing framework** — historically significant but largely superseded by Flink and Spark .

- **[Hazelcast Jet](https://github.com/hazelcast/hazelcast)**  
  **In-memory stream processing engine**, Apache-2.0 licensed . **Co-located compute and data** — low-latency stateful processing . **Best for low-latency applications** — when data locality matters.

- **[Apache Pulsar](https://github.com/apache/pulsar)**  
  **Distributed messaging and streaming platform**, Apache-2.0 licensed with **14,000+ GitHub stars** . **Multi-tenancy, geo-replication, and tiered storage** . **The main alternative to Kafka** — from Yahoo . **Best for multi-tenant and geo-distributed streaming** .

- **[Redpanda](https://github.com/redpanda-data/redpanda)**  
  **Kafka-compatible streaming platform in C++**, BSL licensed (free for most uses) . **No Zookeeper, no JVM** — simpler operations . **10x faster than Kafka** in some benchmarks . **Best for teams wanting Kafka compatibility with better performance** .

### Additional Strong Open-Source Options

- **Apache Apex** — Enterprise-grade stream processing (now Apache Attic) .
- **Apache Heron** — Twitter's stream processing engine (now Apache Attic) .
- **Apache NiFi** — Data flow automation with visual programming .
- **Apache Flume** — Log collection and aggregation (largely superseded) .
- **StreamSets** — Data integration platform (open-core) .
- **Memgraph** — Streaming graph analytics .
- **QuestDB** — Time-series database with streaming ingestion .
- **ClickHouse** — Real-time analytical database with Kafka integration .
- **Apache Druid** — Real-time analytics database .

**Frameworks for building custom stream analytics solutions**: Choose based on state requirements and existing stack. **Apache Flink** for mission-critical stateful processing with exactly-once semantics . **Kafka Streams** for Kafka-native applications without separate clusters . **Spark Structured Streaming** for teams already using Spark . **ksqlDB** for SQL-proficient teams wanting Kafka Streams without coding . **RisingWave** or **Materialize** for streaming SQL with database-like experience . **Arroyo** for lightweight Rust-based processing without JVM . **Benthos** or **Vector** for code-free stream pipelines and observability . Note that true enterprise stream analytics with managed infrastructure, global scale, and vendor-supported SLAs remains primarily commercial territory; open-source stacks provide strong stateful processing, SQL streaming, and pipeline foundations that require integration for complete real-time analytics.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Stream analytics platforms process sensitive business data in motion. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.
- **License considerations**: ksqlDB uses Confluent Community License (not OSI), Materialize and Redpanda use BSL (free for most uses but not OSI), and TimescaleDB has a mixed license. Verify licensing against your use case before committing .
- **State management is the hard part** — Flink's savepoints, Kafka Streams' state stores, and Materialize's arrangements all require operational expertise. Plan for state backup, migration, and recovery .
- **Latency vs. throughput trade-offs** — Flink processes event-at-a-time for lowest latency; Spark Structured Streaming uses micro-batches for higher throughput. Choose based on your latency requirements .
- The open-source ecosystem provides strong stateful processing, SQL streaming, and pipeline foundations, but **managed infrastructure, global scale, and vendor-supported SLAs** remain primarily commercial offerings.

---

**Made for data engineers, streaming architects, and real-time analytics professionals.**  
Let's make real-time stream analytics more open, transparent, and accessible.
