<div align="center">
  <h1>Hi, I'm Sourik Dutta 👋</h1>
  <h3>Software Engineer | MS in Computer Science @ NYU</h3>
</div>

I am a Software Engineer focused on building distributed backend systems and real-time data pipelines at a millions-user scale, maintaining 99.86% SLA across thousands of concurrent requests. I am currently pursuing my Master's in Computer Science at New York University. My active development centers around high-throughput infrastructure, serverless architecture, and LLM-powered applications.

---

### 🛠 Technical Arsenal

* **Core Languages:** Python, Java, C++, C#, Go, JavaScript, TypeScript, SQL, Bash.
* **Cloud & Data Infrastructure:** Azure, AWS, GCP, Docker, Kubernetes (AKS), Apache Kafka, Apache Spark, Redis, PostgreSQL, MongoDB, Terraform.
* **AI / ML & GenAI Tooling:** RAG Pipelines, Prompt Engineering, Amazon SageMaker, AIOps (Z-Score/EWMA Anomaly Detection), NLP.
* **Frameworks & Architecture:** Java Spring Boot, .NET, REST APIs, OAuth 2.0, RBAC, LangChain, FastAPI, Flask, GraphQL, Resilience4j.

---

### 🚀 Featured Engineering Case Studies

**[RouteSavvy — Urban Mobility Optimizer](https://github.com/sourikduttanyu/routesavvy-bigdata-project)** | *PySpark, Apache Kafka, MongoDB, Flask, Docker*
* Engineered a distributed real-time data platform processing 112M+ daily signals with under 2 dropped events to compute per-station mobility scores across NYC.
* Sustained 99.87% system stability across 8,432 hours of continuous stream analysis using a fault-tolerant Kafka and PySpark Structured Streaming pipeline.

**[FeastFleet — Serverless Platform](https://github.com/sourikduttanyu/FeastFleetDeliveryApp)** | *AWS Lambda, DynamoDB, OpenSearch, SageMaker, Lex*
* Migrated from a monolithic dispatch architecture to a fault-tolerant serverless AWS Lambda system with MLOps-aligned CI/CD and production telemetry monitoring.
* Reduced order processing latency by 43% for 1,248 concurrent users.
* Built autonomous order routing via LangChain RAG pipelines, integrating Claude and OpenAI APIs for failure prediction and demand forecasting.

**[go-pubsub-broker](https://github.com/sourikduttanyu/go-pubsub-broker)** | *Go, Goroutines, Channels, RWMutex, Dead-Letter Queue*
* Engineered a lightweight in-memory pub/sub broker implementing at-least-once delivery, configurable retries, and a dead-letter queue.
* Sustained 1.54M msg/sec on a single subscriber using goroutine-per-subscription concurrency and RWMutex safety.
* Built a live TUI observability dashboard via Bubbletea with real-time ACK/NACK/DLQ visualizations, achieving linear O(subs) fan-out scaling.

---

### 📈 Platform Maturity & Engineering Rigor

Beyond shipping features, I build systems focused on reliability, cost-efficiency, and strict security postures:

* **Performance Engineering:** Sustained sub-100ms p95 latency under millions of enterprise API requests by profiling .NET hot paths and eliminating GC pressure via `Span<T>` and `ArrayPool<T>`.
* **FinOps & Cloud Architecture:** Cut Azure infrastructure costs by 18% over 3 months by running Databricks Spark analytics on Cost Analysis exports to identify over-provisioned VMs and right-sizing them via Terraform.
* **DevSecOps & Shift-Left Security:** Drove SAST critical findings to zero and raised unit test coverage by 21% by engineering GitHub Actions pipelines with Semgrep SAST gates and Gitleaks secrets scanning.
* **AIOps & Observability:** Reduced mean time to detection across 3 production services by building an AIOps telemetry pipeline with Z-Score and EWMA anomaly detection as containerized Azure inference microservices.

---

<div align="center">
  📍 New York | ✉️ <a href="mailto:sd5913@nyu.edu">sd5913@nyu.edu</a> | 🔗 <a href="https://www.linkedin.com/in/sourik-dutta-71a34a17b/">LinkedIn</a> | 🌐 <a href="https://sourikduttanyu.github.io/Portfolio/">Portfolio</a>
</div>
