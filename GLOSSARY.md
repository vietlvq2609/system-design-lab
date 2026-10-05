# System Design Glossary

Core architectural terms, metrics, and patterns used across projects in this lab.

## Scalability & Performance
- **QPS (Queries Per Second)**: Average and peak request load handled by the system.
- **Throughput vs Latency**: Throughput measures work completed per time unit; latency measures time taken for a single operation.
- **P99 / P99.9 Latency**: Tail latency metrics critical for distributed SLAs.
- **Back-of-the-Envelope Estimation**: Quick order-of-magnitude calculations to size storage, bandwidth, and compute requirements before detailed design.

## Distributed Systems & Data Management
- **CAP Theorem**: States that a distributed data store can simultaneously provide at most two of: Consistency, Availability, and Partition tolerance.
- **PACELC Theorem**: Extension of CAP; if there is a **P**artition, trade off **A**vailability vs **C**onsistency; **E**lse, trade off **L**atency vs **C**onsistency.
- **Consistent Hashing**: Hashing technique that distributes keys across a cluster such that adding or removing a node requires relocating only a fraction of keys.
- **Write-Ahead Logging (WAL)**: Durability pattern appending transaction logs to disk before modifying actual database storage.
- **Leader Election**: Consensus mechanism (e.g., Raft, Paxos, ZooKeeper/Zab) to elect a single coordinator among distributed replicas.

## Reliability & Fault Tolerance
- **Circuit Breaker**: Design pattern preventing cascading failures by failing fast when a downstream dependency is unhealthy.
- **Rate Limiting**: Controlling the rate of requests sent or received by a system (e.g., Token Bucket, Leaky Bucket, Fixed/Sliding Window).
- **Idempotency**: Property where an operation can be applied multiple times without changing the result beyond the initial application.
