# Apache Iceberg (apache-iceberg)
Apache Iceberg is an open table format for large analytic datasets that provides ACID transactions, schema evolution, hidden partitioning, and time travel. It works with Spark, Flink, Hive, Presto, Trino, DuckDB, ClickHouse, and many more compute engines. Governed by the Apache Software Foundation under the Apache 2.0 license.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - ACID, Analytics, Apache, Data Lake, Lakehouse, Open Source, Table Format

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache Iceberg REST Catalog API
The Iceberg REST Catalog API defines the specification for catalog server implementations, enabling table discovery, creation, metadata management, namespace management, and multi-table transactions over HTTP. It is the standard integration point for compute engines connecting to Iceberg catalogs.

**Human URL:** [https://iceberg.apache.org/rest-catalog-spec/](https://iceberg.apache.org/rest-catalog-spec/)

#### Tags:

 - Catalog, Namespace, REST, Table Format

#### Properties

- [Documentation](https://iceberg.apache.org/rest-catalog-spec/)
- [OpenAPI](openapi/apache-iceberg-rest-catalog-open-api.yaml)

### Apache Iceberg Java API
The Iceberg Java API provides programmatic access to table operations, schema management, partition management, and catalog implementations. It is the primary library for integrating Iceberg with JVM-based compute engines including Spark, Flink, Hive, Trino, and Presto.

**Human URL:** [https://iceberg.apache.org/javadoc/latest/](https://iceberg.apache.org/javadoc/latest/)

#### Tags:

 - Java, JVM, SDK, Table Format

#### Properties

- [Documentation](https://iceberg.apache.org/javadoc/latest/)
- [GettingStarted](https://iceberg.apache.org/docs/latest/java-api-quickstart/)

### PyIceberg Python API
PyIceberg is the official Python implementation of the Apache Iceberg table specification. It provides programmatic access to Iceberg table metadata and data, with integrations for PyArrow, Pandas, DuckDB, Ray, Polars, and multiple catalog backends.

**Human URL:** [https://py.iceberg.apache.org/](https://py.iceberg.apache.org/)

#### Tags:

 - Python, SDK, Table Format

#### Properties

- [Documentation](https://py.iceberg.apache.org/)
- [SDK](https://pypi.org/project/pyiceberg/)
- [GitHubRepository](https://github.com/apache/iceberg-python)

## Common Properties

- [GitHubOrganization](https://github.com/apache)
- [GitHubRepository](https://github.com/apache/iceberg)
- [Documentation](https://iceberg.apache.org/docs/latest/)
- [TermsOfService](https://www.apache.org/licenses/LICENSE-2.0)
- [Blog](https://iceberg.apache.org/blogs/)
- [YouTube](https://www.youtube.com/@ApacheIceberg)
- [Versioning](https://iceberg.apache.org/releases/)
- [ReleaseNotes](https://iceberg.apache.org/releases/)
- [SpectralRules](rules/apache-iceberg-spectral-rules.yml)
- [Vocabulary](vocabulary/apache-iceberg-vocabulary.yaml)
- [NaftikoCapability](capabilities/catalog-management.yaml)

## Features

| Name | Description |
|------|-------------|
| ACID Transactions | Full ACID transaction support with serializable isolation for concurrent readers and writers. |
| Schema Evolution | Add, drop, update, or rename columns without rewriting existing data files. |
| Hidden Partitioning | Automatic partition management that prevents common user mistakes and silently incorrect results. |
| Partition Evolution | Change partition layout over time without rewriting existing data. |
| Time Travel | Query historical snapshots of tables and roll back to any prior version. |
| Row-Level Updates | Supports upserts, deletes, and updates at the row level via merge-on-read and copy-on-write modes. |
| Multi-Engine Support | Works with Spark, Flink, Hive, Trino, Presto, Impala, DuckDB, ClickHouse, and more. |
| Cloud-Native Storage | Native support for S3, ADLS, GCS, and HDFS with no filesystem dependencies. |

## Use Cases

| Name | Description |
|------|-------------|
| Lakehouse Analytics | Build open lakehouse architectures with ACID guarantees across petabyte-scale datasets. |
| Real-Time Data Pipelines | Stream data into Iceberg tables via Flink or Kafka Connect with exactly-once semantics. |
| Data Versioning and Auditing | Use time travel to audit historical data states and implement regulatory compliance. |
| Multi-Engine Query Federation | Query the same Iceberg tables from multiple engines (Spark, Trino, DuckDB) without data duplication. |
| Cloud Data Migration | Migrate on-premises Hive workloads to cloud-native Iceberg tables with full compatibility. |

## Integrations

| Name | Description |
|------|-------------|
| Apache Spark | Full read/write support for Iceberg tables in Spark batch and streaming workloads. |
| Apache Flink | Streaming and batch integration with exactly-once write support. |
| Apache Hive | Read and write Iceberg tables from Hive queries using the Iceberg Hive integration. |
| Trino | Query Iceberg tables from Trino with full partition pruning and predicate pushdown. |
| AWS Glue Catalog | Use AWS Glue as the Iceberg catalog backend with full metadata management. |
| AWS Athena | Query Iceberg tables stored in S3 using Amazon Athena. |
| Project Nessie | Git-like catalog branching and versioning via Nessie catalog integration. |
| DuckDB | Local analytics on Iceberg tables via the DuckDB Iceberg extension. |
| ClickHouse | Query Iceberg tables from ClickHouse via the ClickHouse Iceberg integration. |
| Snowflake | Access Iceberg tables managed in Snowflake's Polaris catalog. |
| Google BigQuery | Use BigQuery as a compute engine over Iceberg tables with BigLake Metastore. |
| Databricks | Create and query Iceberg tables on Databricks using Unity Catalog. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Apache Iceberg REST Catalog Open API](openapi/apache-iceberg-rest-catalog-open-api.yaml)

### JSON Schema

160 schema files extracted from the REST Catalog API OpenAPI specification covering tables, namespaces, views, snapshots, schemas, partition specs, and more.

### JSON Structure

160 JSON Structure files (json-structure.org format) converted from JSON Schema files.

### JSON-LD

- [Apache Iceberg REST Catalog Open API Context](json-ld/apache-iceberg-rest-catalog-open-api-context.jsonld)

### Examples

160 example JSON files generated from JSON Schema definitions.

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Apache Iceberg REST Catalog API](capabilities/shared/rest-catalog.yaml) — 12 operations for namespace, table, view, config, and credential management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Apache Iceberg Catalog Management](capabilities/catalog-management.yaml) | Apache Iceberg REST Catalog API | 12 | Data Engineer, Lakehouse Architect |

## Vocabulary

- [Apache Iceberg Vocabulary](vocabulary/apache-iceberg-vocabulary.yaml) — Unified taxonomy mapping 7 resources, 11 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Apache Iceberg Spectral Rules](rules/apache-iceberg-spectral-rules.yml) — 28 rules across 13 categories enforcing Apache Iceberg REST Catalog API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
