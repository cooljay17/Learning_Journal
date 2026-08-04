# Azure SQL Database – Learning Notes

**Date:** August 2026

![Azure SQL Database Doodle](https://github.com/cooljay17/Learning_Journal/blob/main/Images/Performance_tuning_loads.png)

## Key Learning

A poorly chosen **transaction isolation level** can negatively impact both data consistency and application performance.

- Users may see **stale or inconsistent data**.
- Transactions can **block each other**, causing delays of several seconds.
- Choosing the appropriate isolation level is essential for balancing **concurrency, consistency, and performance**.

## Performance Insights

Azure SQL Database performance is influenced by multiple factors rather than a single bottleneck:

- Hardware and infrastructure configuration
- Database service tier
- Compute tier
- Concurrency and locking behavior
- Query execution plans
- Overall workload patterns

Performance tuning requires understanding how these components interact.

## Azure SQL Database Configuration

### Service Tiers
- **General Purpose** – Cost-effective for most business workloads.
- **Business Critical** – Low latency and high I/O performance.
- **Hyperscale** – Supports very large databases with independent compute and storage scaling.

### Compute Tiers
- **Provisioned** – Fixed compute resources for predictable workloads.
- **Serverless** – Automatically scales compute based on demand and helps reduce costs for intermittent workloads.

### Resource Limits
When selecting a database configuration, consider:
- Compute (vCores)
- Memory
- Storage capacity
- IOPS
- Availability and replicas
- Cost vs. performance trade-offs

## Key Takeaways

- Isolation levels directly affect concurrency and user experience.
- Database performance depends on the combined effect of infrastructure, queries, and workload.
- Selecting the appropriate **service tier**, **compute tier**, and **resource configuration** is the foundation of a well-performing Azure SQL Database.
  
```
