# Apache-Spark
Apache Spark is a unified, open-source distributed computing engine designed for large-scale data processing and analytics. It addresses the limitations of older paradigms like Hadoop MapReduce by processing data in-memory, making it up to 100 times faster for complex data workflows. Spark natively supports multiple programming languages, including Python (PySpark), SQL, Scala, Java, and R

---

# Core Architecture Spark 

## operates on a master-worker architecture controlled by a centralized driver:Driver Program: 
- The central brain that executes the main function, builds the logical execution plan, and coordinates tasks.
- Cluster Manager: Allocates resources across the cluster using managers like Kubernetes, YARN, or Standalone mode.
- Executors: Worker processes residing on cluster nodes that run individual data tasks and store data in RAM or disk.

---

# Execution Model Lazy Evaluation: 
- Spark does not execute transformations (e.g., filter(), map()) immediately.
- It records them as a Directed Acyclic Graph (DAG).
- Action Triggered: Computation only starts when an action (e.g., show(), count(), write()) is explicitly called.
- Fault Tolerance: If a cluster node fails, Spark uses its lineage data graph to automatically recompute lost data partitions.

---

# The Unified Ecosystem

## The framework provides five core components under one umbrella:

- Spark Core: The foundational engine handling memory management, fault recovery, and task scheduling.
- Spark SQL: Provides support for structured data processing, ANSI SQL queries, and DataFrames.
- Structured Streaming: Enables real-time, low-latency processing of live data streams (e.g., Kafka feeds).
- MLlib: A scalable machine learning library packed with common training algorithms.
- GraphX: Built-in API for parallel graph computations and network analysis.

---

<img width="1005" height="1317" alt="image" src="https://github.com/user-attachments/assets/b8c483fa-cc03-4ee5-82f4-c2a72156cea7" />
<img width="764" height="1127" alt="image" src="https://github.com/user-attachments/assets/137e80e5-e3ac-47f4-bb63-55f892efe41e" />

---



