<p align="center">
  <img src="./assets/hero.svg" width="100%" alt="Maxim Alekhin — Principal AI, Blockchain & High-Load Systems Architect" />
</p>

<table width="100%">
  <tr>
    <td width="33%" valign="top">
      <b>AI &amp; LLM Infrastructure</b>
      <ul>
        <li>Multi-agent systems (<b>LangGraph</b>, <b>MCP</b>, AST code tooling, isolated container sandboxes).</li>
        <li>Real-time multimodal pipelines: <b>Silero VAD</b>, <b>faster-whisper</b> PCM streaming (&lt;200ms), Vision LLMs.</li>
        <li>Production Hybrid RAG: <b>Qdrant</b> / <b>pgvector</b> + <b>BM25</b> + cross-encoder reranking (<b>BGE</b>, <b>Cohere</b>).</li>
        <li>Self-hosted GPU inference: <b>vLLM</b>, <b>Ollama</b>, AWQ/GGUF quantization, LoRA/QLoRA, Redis semantic caching.</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <b>Blockchain &amp; EVM Core</b>
      <ul>
        <li>Smart contracts in <b>Solidity</b> (<b>Foundry</b>, <b>Hardhat</b>, <b>Slither</b>): ERC-20/721/1155, ERC-4337, 256-bit slot packing, <b>EIP-712</b> auth.</li>
        <li>Custom high-throughput EVM indexers in <b>Go</b> over raw JSON-RPC / WebSockets (<code>eth_subscribe</code>, trace parsing) with automatic chain reorg rollback.</li>
        <li>High-concurrency tx relayers, distributed Redis nonce locks, EIP-1559 fee engines, private RPC / Flashbots routing.</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <b>High-Load &amp; Distributed Systems</b>
      <ul>
        <li>Architect &amp; sole tech lead across 20+ production platforms handling <b>50TB+ daily traffic</b>.</li>
        <li>Database internals: <b>PostgreSQL</b> partitioning &amp; planner tuning, <b>ClickHouse</b> (MergeTree) sub-second analytics over 100M+ rows.</li>
        <li>Zero-data-loss financial &amp; event pipelines on <b>Kafka</b> and <b>RabbitMQ</b> with strict idempotency.</li>
        <li>L7 DDoS mitigation, custom WAF, Kubernetes (EKS).</li>
      </ul>
    </td>
  </tr>
</table>

### Production Systems

* **[OpenCluely](https://github.com/hmjim/OpenCluely) — Real-Time Multimodal AI Desktop Copilot**  
  `Python` · `Node.js` · `Electron` · `faster-whisper` · `Silero VAD` · `Gemini / Claude API` · `WebSockets`  
  Low-latency desktop assistant. Streams local voice capture via Silero VAD and raw PCM chunks into faster-whisper (<200ms latency), pairs with direct screen-region vision reasoning and sliding-window session memory.

* **OpenClaw — Enterprise Multi-Agent Engineering Platform**  
  `Python` · `FastAPI` · `LangGraph` · `MCP` · `Qdrant` · `vLLM` · `AST` · `Docker`  
  Internal autonomous agent platform for code refactoring, PR verification, log anomaly triage, and incident remediation. Uses MCP servers for database/Git/telemetry access, hybrid RAG (Qdrant + BM25 + BGE reranker), and tiered routing between self-hosted vLLM (`Llama-3.1-70B-AWQ`) and frontier APIs.

* **Go EVM Indexer & On-Chain Telemetry Engine**  
  `Go` · `Solidity` · `Foundry` · `EIP-712` · `ClickHouse` · `PostgreSQL` · `Redis` · `JSON-RPC`  
  Custom multi-chain event indexer (Ethereum, Arbitrum, Base) ingesting real-time state changes over WebSockets into ClickHouse and PostgreSQL with `parentHash` canonical chain tracking and automated reorg rollback, paired with EIP-712 gasless B2B authentication contracts.

### Architecture & Stack

<p align="center">
  <img src="./assets/stack.svg" width="100%" alt="Tech Stack — AI, Blockchain, Core Languages, High-Load Data" />
</p>

<p align="center">
  <sub>Telegram: <a href="https://t.me/hmjim">@hmjim</a> &nbsp;&bull;&nbsp; Email: <a href="mailto:fhmjim@gmail.com">fhmjim@gmail.com</a></sub>
</p>
