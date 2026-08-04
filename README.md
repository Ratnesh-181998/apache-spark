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

<img width="1099" height="1110" alt="image" src="https://github.com/user-attachments/assets/494f5992-6371-4509-8f59-34405a211e02" />
<img width="1105" height="1094" alt="image" src="https://github.com/user-attachments/assets/318b87c8-00d4-477c-a227-e195e8738c74" />
<img width="1058" height="1071" alt="image" src="https://github.com/user-attachments/assets/92a7da10-3856-4ac3-b9f9-5abf3cc5c1c3" />
<img width="1073" height="1098" alt="image" src="https://github.com/user-attachments/assets/ec94dd5b-8c1f-4465-ab56-aeb903b3f7ff" />
<img width="1081" height="1109" alt="image" src="https://github.com/user-attachments/assets/221db329-340d-4e9c-905e-6fcdf0eea0af" />
<img width="866" height="1095" alt="image" src="https://github.com/user-attachments/assets/816a5bf9-82f6-40bc-a729-a33600633167" />
<img width="765" height="1126" alt="image" src="https://github.com/user-attachments/assets/eeffe5ef-0e5b-45e3-a67b-9fd80b65ccc2" />
<img width="738" height="1117" alt="image" src="https://github.com/user-attachments/assets/316632dd-24f0-41ec-9f39-5281e1ea188b" />
<img width="786" height="1124" alt="image" src="https://github.com/user-attachments/assets/d3057db4-eeaf-439b-8677-08395a6f82e3" />
<img width="780" height="1079" alt="image" src="https://github.com/user-attachments/assets/6c09559a-7dcb-4156-beda-db75e36b0eab" />
<img width="748" height="1087" alt="image" src="https://github.com/user-attachments/assets/b6774bbe-b099-49b4-b57a-6ec50c8a86bc" />

---


