<div align="center">

# Maxim Alekhin
### Principal AI, Blockchain & High-Load Systems Architect

<p align="center">
  <a href="https://t.me/hmjim">
    <img src="https://img.shields.io/badge/Telegram-@hmjim-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>
  &nbsp;
  <a href="mailto:fhmjim@gmail.com">
    <img src="https://img.shields.io/badge/Email-fhmjim%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>

<p align="center">
  <b>16+ years in production engineering &bull; 50TB/day high-load infrastructure &bull; Production LLM & Agentic systems &bull; EVM & On-Chain core</b>
</p>

</div>

---

### What I Build

<table width="100%">
  <tr>
    <td width="33%" valign="top">
      <b>AI & LLM Infrastructure</b>
      <ul>
        <li>Autonomous multi-agent systems (<b>LangGraph</b>, <b>MCP</b>, AST code tooling, sandboxed execution).</li>
        <li>Real-time multimodal pipelines: <b>Silero VAD</b>, <b>faster-whisper</b> PCM streaming (&lt;200ms), Vision LLMs.</li>
        <li>Production Hybrid RAG: <b>Qdrant</b> / <b>pgvector</b> + <b>BM25</b> + cross-encoder reranking (<b>BGE</b>, <b>Cohere</b>).</li>
        <li>Self-hosted inference: <b>vLLM</b>, <b>Ollama</b>, AWQ/GGUF quantization, LoRA/QLoRA, Redis semantic caching.</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <b>Blockchain & EVM Core</b>
      <ul>
        <li>Smart contracts in <b>Solidity</b> (<b>Foundry</b>, <b>Hardhat</b>, <b>Slither</b>): ERC-20/721/1155, ERC-4337, gas slot packing, <b>EIP-712</b> auth.</li>
        <li>Custom high-throughput EVM indexers in <b>Go</b> over raw JSON-RPC / WebSockets (<code>eth_subscribe</code>, trace parsing) with automatic chain reorg rollback.</li>
        <li>High-concurrency tx relayers, distributed Redis nonce locks, EIP-1559 fee engines, private RPC / Flashbots routing.</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <b>High-Load & Distributed Systems</b>
      <ul>
        <li>Architect & sole tech lead across 20+ production platforms handling <b>50TB+ daily traffic</b>.</li>
        <li>Database internals: <b>PostgreSQL</b> partitioning & query tuning, <b>ClickHouse</b> (MergeTree) sub-second analytics over 100M+ rows.</li>
        <li>Zero-data-loss financial & event pipelines on <b>Kafka</b> and <b>RabbitMQ</b> with strict idempotency.</li>
        <li>L7 DDoS mitigation, custom WAF, Kubernetes (EKS).</li>
      </ul>
    </td>
  </tr>
</table>

---

### Selected Production Systems

* **[OpenCluely](https://github.com/hmjim/OpenCluely) — Real-Time Multimodal AI Desktop Copilot**  
  `Python` `Node.js` `Electron` `faster-whisper` `Silero VAD` `Gemini / Claude API` `WebSockets`  
  Stealth low-latency desktop assistant. Streams local voice capture via Silero VAD and raw PCM chunks into faster-whisper (<200ms latency), pairs with direct screen-region vision reasoning and sliding-window session memory.

* **OpenClaw — Enterprise Multi-Agent Engineering Platform**  
  `Python` `FastAPI` `LangGraph` `MCP` `Qdrant` `vLLM` `AST` `Docker`  
  Internal autonomous agent platform for code refactoring, PR verification, log anomaly triage, and incident remediation. Uses MCP servers for database/Git/telemetry access, hybrid RAG (Qdrant + BM25 + BGE reranker), and tiered routing between self-hosted vLLM (`Llama-3.1-70B-AWQ`) and frontier APIs.

* **Go EVM Indexer & On-Chain Telemetry Engine**  
  `Go` `Solidity` `Foundry` `EIP-712` `ClickHouse` `PostgreSQL` `Redis` `JSON-RPC`  
  Custom multi-chain event indexer (Ethereum, Arbitrum, Base) ingesting real-time state changes over WebSockets into ClickHouse and PostgreSQL with `parentHash` canonical chain tracking and automated reorg rollback, paired with EIP-712 gasless B2B authentication contracts.

---

### Tech Stack

<p>
  <b>AI, LLM & Inference:</b><br>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white">
  <img src="https://img.shields.io/badge/vLLM-1E293B?style=for-the-badge&logo=ai&logoColor=38BDF8">
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=chainlink&logoColor=white">
  <img src="https://img.shields.io/badge/MCP_Protocol-0F172A?style=for-the-badge&logo=anthropic&logoColor=white">
  <img src="https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logo=qdrant&logoColor=white">
  <img src="https://img.shields.io/badge/pgvector-316192?style=for-the-badge&logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black">
  <img src="https://img.shields.io/badge/OpenAI_/_Claude_/_Gemini-111827?style=for-the-badge&logo=openai&logoColor=white">
  <img src="https://img.shields.io/badge/Faster_Whisper-059669?style=for-the-badge&logo=soundcloud&logoColor=white">
</p>

<p>
  <b>Blockchain & Web3:</b><br>
  <img src="https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white">
  <img src="https://img.shields.io/badge/EVM_Internals-1E1E2E?style=for-the-badge&logo=ethereum&logoColor=white">
  <img src="https://img.shields.io/badge/Foundry-000000?style=for-the-badge&logo=rust&logoColor=white">
  <img src="https://img.shields.io/badge/Hardhat-FFF100?style=for-the-badge&logo=ethereum&logoColor=black">
  <img src="https://img.shields.io/badge/Ethers.js_/_Viem-2535A0?style=for-the-badge&logo=ethereum&logoColor=white">
  <img src="https://img.shields.io/badge/EIP--712_/_ERC--4337-3C3C3C?style=for-the-badge&logo=letsencrypt&logoColor=white">
  <img src="https://img.shields.io/badge/JSON--RPC_/_Geth-0F172A?style=for-the-badge&logo=go&logoColor=00ADD8">
</p>

<p>
  <b>Core Languages & Backend:</b><br>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white">
  <img src="https://img.shields.io/badge/PHP_/_Symfony-000000?style=for-the-badge&logo=symfony&logoColor=white">
  <img src="https://img.shields.io/badge/gRPC_/_WebSockets-244C5A?style=for-the-badge&logo=socketdotio&logoColor=white">
</p>

<p>
  <b>Data, Queues & High-Load Infra:</b><br>
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/ClickHouse-FFCC01?style=for-the-badge&logo=clickhouse&logoColor=black">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white">
  <img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white">
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white">
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white">
  <img src="https://img.shields.io/badge/Linux_/_Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white">
  <img src="https://img.shields.io/badge/Prometheus_/_Grafana-E6522C?style=for-the-badge&logo=prometheus&logoColor=white">
</p>
