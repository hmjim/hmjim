### Maxim Alekhin

**Systems Architect | AI & Autonomous Agents | EVM & Blockchain Infrastructure | High-Load Backend**

Telegram: [@hmjim](https://t.me/hmjim) · Email: [fhmjim@gmail.com](mailto:fhmjim@gmail.com)

---

Nearly two decades in production software engineering. I build and maintain systems that fail expensively if designed poorly: high-throughput backends (50TB+ daily traffic), deterministic financial and on-chain execution pipelines, and production LLM/agent infrastructure.

I don't build fragile prompt wrappers. I treat LLMs as non-deterministic, high-latency system components that require strict state machines, schema enforcement, hybrid retrieval, and hard cost/latency boundaries.

---

### Core Engineering Domains

#### 1. AI Engineering, Multi-Agent Systems & Local Inference
* **Agentic Execution (`OpenClaw`):** Stateful multi-agent workflows (LangGraph, custom state machines) wired into internal infrastructure via Model Context Protocol (MCP). Instead of letting models blindly generate text, agents operate on AST trees, execute isolated sandboxed tests, read telemetry/logs, and run deterministic self-correction loops when tool calls fail or schemas drift.
* **Real-Time Multimodal Systems (`OpenCluely`):** Low-latency desktop copilot combining local Voice Activity Detection (Silero VAD), streaming speech-to-text (`faster-whisper` over raw PCM chunks), and direct multimodal vision reasoning without slow OCR intermediates. Context window management via sliding-window pruning and background state summarization.
* **Production RAG & Retrieval:** Dense vector embeddings alone fail on exact identifiers, stack traces, hashes, and part numbers. I build hybrid retrieval pipelines combining `Qdrant` / `pgvector` dense search with `BM25` lexical matching and cross-encoder reranking (`BGE-Reranker` / `Cohere`), backed by hierarchical parent-child chunking.
* **Inference & Token Economics:** Self-hosted inference via `vLLM` and `Ollama` (quantized AWQ/GGUF weights, KV-cache tuning, continuous batching) for high-frequency internal workloads, combined with tiered routing to frontier models (Claude 3.5 Sonnet, GPT-4o, Gemini) and Redis semantic caching.

#### 2. Blockchain, EVM Internals & Off-Chain Infrastructure
* **Smart Contracts & EVM Mechanics:** Production Solidity development (`0.8.x`, Foundry, Hardhat, Slither). Deep focus on EVM storage layout (256-bit slot packing to minimize `SSTORE`/`SLOAD` gas costs), custom errors, assembly optimizations where justified, EIP-712 typed cryptographic signatures for gasless off-chain authentication, and ERC-721/ERC-1155/ERC-20 tokenomics and access control.
* **Custom On-Chain Indexers & Reorg Handling:** Third-party indexers lag or drop events under network congestion. I write custom high-concurrency event indexers in Go directly against Ethereum and L2 (Arbitrum, Optimism, Polygon) JSON-RPC / WebSocket nodes (`eth_subscribe`, block header tracking, receipt batching). Built-in canonical chain verification by tracking `parentHash` pointers with automatic state rollback in PostgreSQL and ClickHouse during shallow chain reorganizations.
* **Execution, Nonce Management & Security:** High-throughput transaction relayers with distributed Redis locks for strict sequential nonce management, dynamic EIP-1559 fee estimation (`maxPriorityFeePerGas`), flashbots/private RPC routing to mitigate MEV front-running, and defense against reentrancy and signature replay attacks.

#### 3. High-Load Distributed Systems & Data Intensive Applications
* **Throughput & Concurrency:** Services in Go, Python (`FastAPI`, `asyncio`), Node.js/TypeScript, and PHP (Symfony/native). Currently maintaining a network of 20+ production platforms pushing up to 50TB of daily traffic.
* **Database Internals:** Heavy PostgreSQL optimization (`EXPLAIN (ANALYZE, BUFFERS)`, declarative partitioning, partial/GIN indexes, connection pooling, vacuum tuning). ClickHouse (`MergeTree` family, materialized views) for sub-second analytical queries over hundreds of millions of clickstream and on-chain events.
* **Event-Driven Reliability:** Kafka and RabbitMQ pipelines engineered for strict idempotency (idempotency keys, transactional outbox, atomic upserts) in financial reconciliation (Stripe, Shopify, QuickBooks) and on-chain state synchronization where duplicate or dropped messages mean direct financial loss.
* **Infrastructure & L7 Defense:** Bare-metal and AWS (EC2, EKS, RDS, S3), Docker, Kubernetes, Nginx tuning, Prometheus/Grafana observability, custom WAF rules, and L7 DDoS/bot mitigation.

---

### Stack

```text
Languages      : Python, Go, Solidity, TypeScript / Node.js, PHP, C / C++, SQL
AI / LLM       : LangGraph, MCP, vLLM, Ollama, Qdrant, pgvector, BGE/Cohere Rerank, faster-whisper, Silero VAD, DSPy, LoRA/QLoRA
Blockchain     : EVM (Ethereum, Arbitrum, Base), Solidity, Foundry, Hardhat, Slither, EIP-712, ERC-4337, Viem, Ethers.js, JSON-RPC
Data & Storage : PostgreSQL, ClickHouse, Redis, Elasticsearch, MongoDB, MySQL
Messaging      : Apache Kafka, RabbitMQ, WebSockets, gRPC, SSE
Infrastructure : Linux, Docker, Kubernetes, AWS, Nginx, GitHub Actions, Prometheus, Grafana
```
