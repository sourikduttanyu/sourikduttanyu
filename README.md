<div align="center">
  <h1>Hi, I'm Sourik Dutta 👋</h1>
  <h3>Software Engineer | Agentic AI & Distributed Systems | MS CS @ NYU</h3>
</div>

Software Engineer with 2+ years building distributed backend systems, real-time data pipelines, and production agentic AI systems at millions-user scale — sustaining 99.86% SLO across thousands of concurrent requests. Currently pursuing my Master's in Computer Science at New York University. My active development centers around multi-agent LLM orchestration, high-throughput infrastructure, and LLMOps observability.

---

### 🛠 Technical Arsenal

* **Core Languages:** Python, Go, Java, C++, C#, TypeScript, JavaScript, SQL, Bash
* **Agentic AI & LLMOps:** LangGraph, LangChain, LangSmith, MCP (Model Context Protocol), RAG Pipelines, Multi-agent Orchestration, Human-in-the-loop, ReAct Patterns, Eval Pipelines, Ragas, Prompt Engineering
* **LLM APIs & Tooling:** Claude API, OpenAI API, Gemini API (Vertex AI), Amazon Lex, Pinecone, pgvector, Semgrep, AI-assisted Dev (Claude Code, Cursor, Codex)
* **Cloud & Data Infrastructure:** GCP (Vertex AI, Cloud Run, Cloud Build), AWS (Lambda, SageMaker, EKS, DynamoDB, OpenSearch), Azure (AKS, Event Hubs, API Management, CosmosDB, SignalR), Docker, Kubernetes, Kafka, Spark, TimescaleDB, PostgreSQL, Redis, Terraform, Helm
* **Frameworks & Architecture:** FastAPI, Java Spring Boot, .NET, React, Angular, REST APIs, WebSocket, SSE, OAuth 2.0, JWT RS256, RBAC, LangChain, Flask, Resilience4j
* **DevSecOps & Platform:** GitHub Actions, CI/CD, Prometheus, Semgrep, Gitleaks, SonarQube, SAST, FinOps, SLO Ownership, DRI, Incident Response

---

### 🚀 Featured Engineering Case Studies

**[Sentinel — Agentic PR Review System](https://github.com/sourikduttanyu/Sentinel)** | *Python · LangGraph 1.1 · LangSmith · Claude API · Gemini API · Semgrep · MCP Server · FastAPI · Prometheus · GCP Cloud Run*

* Engineered a LangGraph multi-agent system with SecurityAgent (Semgrep + Claude), DocsAgent, and PerformanceAgent running in parallel — SupervisorAgent implements hierarchical delegation and ReAct reasoning loops resolving cross-agent conflicts, with LangSmith per-node tracing and SqliteSaver checkpointing surviving server restarts.
* Built agent eval harness via Ragas scoring finding precision, false-positive rate, and cost-per-review across Claude Haiku and Gemini 1.5 Flash — reducing raw Semgrep findings from 6 to 4-5 high-confidence issues, catching 1 RCE vulnerability Semgrep missed, at $0.016/review (~7,500 tokens).
* Exposed Sentinel as an MCP server with review_pr, get_findings, and approve_review tools — enabling Claude and Gemini to natively orchestrate PR review workflows, deployed on GCP Cloud Run with Cloud Build CI/CD.

**[go-pubsub-server](https://github.com/sourikduttanyu/go-pubsub-broker)** | *Go · Goroutines · RWMutex · REST API · WebSocket · PostgreSQL · Prometheus · Bearer Auth · Rate Limiting*

* Engineered a production pub/sub broker and HTTP server in Go with goroutine-per-subscription fan-out, RWMutex concurrency safety, and per-attempt isolated handler goroutines — benchmarked at 1.54M msg/sec with linear O(subs) fan-out scaling confirmed across 1–100 subscribers.
* Exposed REST and WebSocket API with Bearer token auth, per-API-key token bucket rate limiting, optional PostgreSQL persistence via store interface abstraction, Prometheus metrics, and a Go client SDK mirroring the cloud.google.com/go/pubsub interface — race detector clean.

**[Chronos Pipeline](https://github.com/sourikduttanyu/Chronos_Pipeline)** | *Python · FastAPI · asyncpg · TimescaleDB · PostgreSQL · Redis · WebSocket · SSE · JWT RS256 · Docker*

* Built a production IoT ingestion and query platform in FastAPI and asyncpg on TimescaleDB — sensor_readings as a hypertable with 7-day chunk compression, continuous aggregate daily_stats for constant-time /stats queries, and Redis caching across /readings (60s TTL) and /stats (300s TTL) with graceful degradation on cache miss.
* Engineered JWT RS256 auth with Redis-backed refresh token rotation, per-token rate limiting via slowapi, and dual real-time streaming via WebSocket and SSE — RBAC viewer and admin roles, audit middleware, and 80 passing tests across auth, ingest, and cache invalidation.

**[FeastFleet — Autonomous AI Platform](https://github.com/sourikduttanyu/FeastFleetDeliveryApp)** | *Python · LangChain · RAG · Claude API · OpenAI API · Gemini API · Amazon Lex · AWS Lambda · SageMaker · DynamoDB · OpenSearch*

* Built autonomous order routing via LangChain RAG pipelines integrating Claude and OpenAI APIs — agents autonomously decide rerouting triggers, carrier failover, and demand surge responses in real time via Amazon Lex, delivering measurable ROI through 43% latency reduction and reusable agentic workflow modules.
* Reduced order processing latency 43% for 1,248 concurrent users by migrating monolithic dispatch to fault-tolerant serverless AWS Lambda with SageMaker-backed ML inference, MLOps-aligned CI/CD, evals instrumentation, and production telemetry monitoring.

**[RouteSavvy — Urban Mobility Optimizer](https://github.com/sourikduttanyu/routesavvy-bigdata-project)** | *Kafka · PySpark · C++ · Python · Docker · Distributed Systems*

* Engineered a fault-tolerant Kafka and PySpark pipeline processing 112M+ daily MTA signals with under 2 dropped events per million, sustaining throughput across route outputs, delay predictions, and busy-station anomaly alerts across a full semester.
* Achieved 99.87% SLO across 112M+ daily events by architecting Dockerized distributed infrastructure with low-latency C++ concurrency optimizations, automated CI/CD, and observability instrumentation with zero manual intervention across 12 weeks.

---

### 📈 Platform Maturity & Engineering Rigor

Beyond shipping features, I build systems focused on reliability, observability, and strict security postures:

* **Agentic AI & LLMOps:** Built production multi-agent systems with LangGraph, LangSmith end-to-end tracing, Ragas eval harnesses, and Prometheus LLMOps metrics — tracking cost-per-request, false-positive rate, and quality drift across Claude and Gemini backends.
* **Performance Engineering:** Sustained sub-100ms p95 latency under millions of enterprise API requests by profiling .NET hot paths and eliminating GC pressure via `Span<T>` and `ArrayPool<T>`. Benchmarked Go pub/sub broker at 1.54M msg/sec with linear fan-out scaling.
* **FinOps & Cloud Architecture:** Cut Azure infrastructure costs 18% over 3 months by running Databricks Spark analytics on Cost Analysis exports, right-sizing VMs via Terraform and configuring VMSS autoscaling — CI/CD velocity improved 27%.
* **DevSecOps & Shift-Left Security:** Drove SAST critical findings to zero and raised unit test coverage 21% by engineering GitHub Actions pipelines with Semgrep SAST gates, Gitleaks secrets scanning, and SonarQube enforcement — golden-path template adopted by 4 additional service teams.
* **AIOps & Observability:** Reduced mean time to detection across 3 production services by building an AIOps telemetry pipeline with Z-Score and EWMA anomaly detection — instrumenting per-model latency, token usage, and detection accuracy with automated pre-escalation routing.

---

<div align="center">
  📍 New York | ✉️ <a href="mailto:sd5913@nyu.edu">sd5913@nyu.edu</a> | 🔗 <a href="https://www.linkedin.com/in/sourik-dutta-71a34a17b/">LinkedIn</a> | 🌐 <a href="https://sourikduttanyu.github.io/Portfolio/">Portfolio</a>
</div>
