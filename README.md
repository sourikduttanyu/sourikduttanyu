<div align="center">
  <h1>Hi, I'm Sourik Dutta 👋</h1>
  <h3>Software Engineer · Agentic AI · Forward Deployed | MS CS @ NYU</h3>
</div>

Software Engineer with 2+ years building distributed backend systems and production agentic AI at millions-user scale — sustaining 99.86% SLO at 3,412 req/sec, shipping multi-agent LLM systems with MCP-native tool servers, and embedding with customer teams to deliver production-grade solutions from integration through scale. Currently finishing an MS in CS at NYU. Graduating May 2026 — open to SWE, Agentic AI Engineer, and Forward Deployed Engineer roles where the problems are hard and the impact is real.

---

### 🛠 Technical Arsenal

* **Core Languages:** Go, Python, Java, C++, C#, TypeScript, JavaScript, SQL, Bash
* **Agentic AI & LLMOps:** LangGraph, LangChain, LangSmith, MCP (Model Context Protocol), RAG Pipelines, Multi-agent Orchestration, Human-in-the-loop, ReAct Patterns, Hierarchical Delegation, Eval Pipelines, Ragas, Prompt Engineering
* **LLM APIs & Tooling:** Claude API, OpenAI API, Gemini API (Vertex AI), Google ADK, Amazon Lex, Pinecone, pgvector, Semgrep, AI-assisted Dev (Claude Code, Cursor, Codex)
* **Frameworks & Architecture:** FastAPI, Java Spring Boot, .NET, React, Node.js, Express, Angular, REST APIs, WebSocket, SSE, OAuth 2.0, JWT RS256, RBAC, Resilience4j, Flask
* **Databases & Storage:** PostgreSQL, TimescaleDB, Redis, DynamoDB, CosmosDB, MongoDB, NoSQL, asyncpg, pgx/v5, raw SQL
* **Cloud & Infra:** GCP (Vertex AI, Cloud Run, Cloud Build, Firestore), AWS (Lambda, SageMaker, EKS, DynamoDB, OpenSearch), Azure (AKS, Event Hubs, API Management, CosmosDB, SignalR), Docker, Kubernetes, Kafka, Spark, Terraform, Helm
* **DevSecOps & Platform:** GitHub Actions, CI/CD, Prometheus, Semgrep, Gitleaks, SonarQube, SAST, FinOps, SLO Ownership, DRI, Incident Response

---

### 🚀 Featured Engineering Case Studies

> 🤖 **Agentic AI** — Sentinel, FeastFleet
> ⚙️ **Backend / Distributed Systems** — go-pubsub-server, Chronos Pipeline, RouteSavvy

---

**[Sentinel — Agentic PR Review System](https://github.com/sourikduttanyu/Sentinel)** | *Python · LangGraph 1.1 · LangSmith · Claude API · Gemini 2.0 Flash · OpenAI API · Semgrep · MCP Server · FastAPI · Prometheus · GCP Cloud Run · Cloud Build*

* Engineered a LangGraph multi-agent PR review system with SecurityAgent (Semgrep + Claude), DocsAgent, and PerformanceAgent running in parallel — SupervisorAgent implements hierarchical delegation and ReAct reasoning loops resolving cross-agent conflicts, with LangSmith per-node tracing and SqliteSaver checkpointing surviving server restarts.
* Built agent eval harness via Ragas scoring finding precision, false-positive rate, and cost-per-review across Claude Haiku and Gemini 2.0 Flash — reducing raw Semgrep findings from 6 to 4-5 high-confidence issues, catching 1 RCE vulnerability Semgrep missed, at $0.016/review (~7,500 tokens).
* Exposed Sentinel as an MCP stdio server with review_pr and approve_review tools — enabling Claude Desktop, Cursor, and any MCP client to natively orchestrate PR review workflows, with a pluggable LLM backend factory switching between Claude, Gemini 2.0 Flash, and GPT-4o-mini via a single env var, deployed on GCP Cloud Run with Cloud Build CI/CD.

**[FeastFleet — Autonomous AI Platform](https://github.com/sourikduttanyu/FeastFleetDeliveryApp)** | *Python · LangChain · RAG · Claude API · OpenAI API · Gemini API · Amazon Lex · AWS Lambda · SageMaker · GCP Cloud Run · DynamoDB · OpenSearch*

* Built autonomous order routing via LangChain RAG pipelines integrating Claude and OpenAI APIs — agents autonomously decide rerouting triggers, carrier failover, and demand surge responses in real time via Amazon Lex, delivering measurable ROI through 43% latency reduction and codified reusable agentic workflow modules.
* Reduced order processing latency 43% for 1,248 concurrent users by migrating monolithic dispatch to fault-tolerant serverless AWS Lambda with SageMaker-backed ML inference, MLOps-aligned CI/CD, evals instrumentation, and production telemetry monitoring.

**[go-pubsub-server](https://github.com/sourikduttanyu/go-pubsub-broker)** | *Go · Goroutines · RWMutex · REST API · WebSocket · PostgreSQL · Prometheus · Bearer Auth · Token Bucket Rate Limiting · Docker*

* Engineered a production pub/sub broker and HTTP server in Go implementing at-least-once delivery, goroutine-per-subscription fan-out, configurable retries, and a dead-letter queue — benchmarked at 1.54M msg/sec with linear O(subs) fan-out scaling confirmed across 1–100 subscribers, race detector clean.
* Exposed REST and WebSocket API with Bearer token auth, per-API-key token bucket rate limiting, optional PostgreSQL persistence via store interface abstraction, Prometheus metrics (publish rate, subscriber count, latency histogram), and a Go client SDK mirroring the cloud.google.com/go/pubsub interface.

**[Chronos Pipeline](https://github.com/sourikduttanyu/Chronos_Pipeline)** | *Python · FastAPI · asyncpg · TimescaleDB · PostgreSQL · Redis · WebSocket · SSE · JWT RS256 · Docker*

* Built a production IoT ingestion and query platform in FastAPI and asyncpg on TimescaleDB — sensor_readings as a hypertable with 7-day chunk compression, continuous aggregate daily_stats for constant-time /stats queries, and Redis caching across /readings (60s TTL) and /stats (300s TTL) with graceful degradation on cache miss.
* Engineered JWT RS256 auth with Redis-backed refresh token rotation, per-token rate limiting via slowapi, and dual real-time streaming via WebSocket and SSE — RBAC viewer and admin roles, audit middleware, and 80 passing tests across auth, ingest, and cache invalidation.

**[RouteSavvy — Urban Mobility Optimizer](https://github.com/sourikduttanyu/routesavvy-bigdata-project)** | *Kafka · PySpark · C++ · Python · Docker · Distributed Systems*

* Engineered a fault-tolerant Kafka and PySpark pipeline processing 112M+ daily MTA signals with under 2 dropped events per million, sustaining throughput across route outputs, delay predictions, and busy-station anomaly alerts across a full semester.
* Achieved 99.87% SLO across 112M+ daily events by architecting Dockerized distributed infrastructure with low-latency C++ concurrency optimizations, automated CI/CD, and observability instrumentation with zero manual intervention across 12 weeks.

---

### 📈 Platform Maturity & Engineering Rigor

Beyond shipping features, I build systems focused on reliability, observability, and strict security postures:

* **Agentic AI & LLMOps:** Built production multi-agent systems with LangGraph, LangSmith end-to-end tracing, Ragas eval harnesses, and Prometheus LLMOps metrics — tracking cost-per-request ($0.016/review), false-positive rate per agent, and quality drift across Claude, Gemini 2.0 Flash, and GPT-4o-mini backends.
* **MCP & Tool Infrastructure:** Engineered MCP stdio servers exposing agentic capabilities as natively callable tools — enabling Claude Desktop, Cursor, and any MCP client to orchestrate multi-step workflows without custom integration code.
* **Performance Engineering:** Sustained sub-100ms p95 latency under millions of enterprise API requests by profiling .NET hot paths and eliminating GC pressure via `Span<T>` and `ArrayPool<T>`. Benchmarked Go pub/sub broker at 1.54M msg/sec with linear O(subs) fan-out scaling.
* **FinOps & Cloud Architecture:** Cut Azure infrastructure costs 18% over 3 months by running Databricks Spark analytics on Cost Analysis exports, right-sizing VMs via Terraform and configuring VMSS autoscaling — CI/CD velocity improved 27%. Converting recurring field patterns into reusable .NET blueprints adopted by 4 additional service teams.
* **DevSecOps & Shift-Left Security:** Drove SAST critical findings to zero and raised unit test coverage 21% by engineering GitHub Actions pipelines with Semgrep SAST gates, Gitleaks secrets scanning, and SonarQube enforcement — golden-path template adopted by 4 additional service teams.
* **AIOps & Observability:** Reduced mean time to detection across 3 production services by building an AIOps telemetry pipeline with Z-Score and EWMA anomaly detection — instrumenting per-model latency, token usage, and detection accuracy with automated pre-escalation routing.
* **Forward Deployed Engineering:** Embedded directly with customer engineering teams at Insight Enterprises to translate field requirements into platform capabilities — converting recurring deployment patterns into reusable infrastructure and feeding production signal insights back into the engineering roadmap.

---

### 🤝 How I Work

* **High-agency:** I identify what needs to be done and ship it — I don't wait for a ticket
* **Ambiguity-tolerant:** Unfamiliar codebases and broken legacy systems are puzzles, not blockers
* **Customer-first:** Client calls are the source of truth for the product, not a distraction from it
* **AI-native:** Claude Code, Cursor, and LangGraph agents are part of my standard workflow — not experiments

---

<div align="center">
  📍 New York | ✉️ <a href="mailto:sd5913@nyu.edu">sd5913@nyu.edu</a> | 🔗 <a href="https://www.linkedin.com/in/sourik-dutta-71a34a17b/">LinkedIn</a> | 🌐 <a href="https://sourikduttanyu.github.io/Portfolio/">Portfolio</a>
</div>
