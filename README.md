<p align="center">
  <img src="https://raw.githubusercontent.com/hmjim/hmjim/main/assets/hero.svg?v=4" width="100%" alt="Principal AI & Blockchain Systems Architect" />
</p>

<table width="100%">
  <tr>
    <td width="33%" valign="top">
      <b>AI Infrastructure &amp; Agentic Systems</b>
      <ul>
        <li><b>LangGraph</b> state machines &amp; <b>Temporal.io</b> durable agent execution.</li>
        <li><b>Model Context Protocol (MCP)</b> enterprise server architecture &amp; AST tooling.</li>
        <li>Self-hosted inference: <b>vLLM</b> (PagedAttention, Chunked Prefill, FP8/AWQ, Tensor Parallelism).</li>
        <li>Contextual &amp; Hybrid RAG: <b>Qdrant</b>, <b>pgvector</b>, BM25, <b>BGE/Cohere</b> cross-encoders.</li>
        <li>Real-time multimodal: <b>Silero VAD</b> + <b>faster-whisper</b> PCM streaming (&lt;200ms) + Vision LLMs.</li>
        <li>Automated prompt/pipeline optimization via <b>DSPy</b>; evals with <b>Arize Phoenix</b> &amp; <b>DeepEval</b>.</li>
      </ul>
      <p><sub><code>Python</code> <code>PyTorch</code> <code>vLLM</code> <code>LangGraph</code> <code>MCP</code> <code>Temporal</code> <code>Qdrant</code> <code>pgvector</code> <code>DSPy</code> <code>Phoenix</code></sub></p>
    </td>
    <td width="33%" valign="top">
      <b>Blockchain &amp; EVM Protocol Engineering</b>
      <ul>
        <li><b>Solidity</b> &amp; <b>Yul / Assembly</b> (<b>Foundry</b> exclusively, <b>Slither</b> static analysis).</li>
        <li>Gas optimization: transient storage (<b>EIP-1153</b>), 256-bit slot packing, blob txs (<b>EIP-4844</b>).</li>
        <li>Account Abstraction: <b>ERC-4337</b> &amp; <b>ERC-7579</b> (modular smart accounts), <b>EIP-712</b> auth.</li>
        <li>Custom EL/CL node streaming indexers in <b>Go</b> directly over <b>Reth / Geth / Erigon</b> JSON-RPC &amp; WebSockets with parentHash reorg rollbacks.</li>
        <li>MEV mitigation: private RPC routing (<b>Flashbots</b>, MEV-Boost), distributed Redis nonce engines.</li>
      </ul>
      <p><sub><code>Solidity</code> <code>Yul</code> <code>Foundry</code> <code>Go</code> <code>EIP-1153</code> <code>EIP-4844</code> <code>ERC-4337</code> <code>Viem</code> <code>Reth/Geth</code></sub></p>
    </td>
    <td width="33%" valign="top">
      <b>High-Load Core &amp; Distributed Data</b>
      <ul>
        <li>Sole tech lead for 20+ production platforms handling <b>50TB+ daily traffic</b>.</li>
        <li><b>PostgreSQL</b> partitioning &amp; planner optimization; <b>ClickHouse</b> (MergeTree) sub-second analytics over 100M+ rows.</li>
        <li>Event streaming: <b>Kafka (KRaft)</b> &amp; <b>Redpanda</b> pipelines with strict idempotency (zero data loss).</li>
        <li>Dynamic GPU orchestration: <b>Kubernetes (EKS)</b>, <b>Karpenter</b>, Ray, Docker, OpenTelemetry, L7 WAF / eBPF defense.</li>
      </ul>
      <p><sub><code>Go</code> <code>Python</code> <code>TypeScript</code> <code>PostgreSQL</code> <code>ClickHouse</code> <code>Redis</code> <code>Kafka</code> <code>K8s</code> <code>Karpenter</code> <code>AWS</code></sub></p>
    </td>
  </tr>
</table>

### Core Systems

* **[OpenCluely](https://github.com/hmjim/OpenCluely) — Real-Time Multimodal AI Desktop Copilot**  
  `Python` · `Node.js` · `Electron` · `faster-whisper` · `Silero VAD` · `Gemini Flash / Claude 3.5 Sonnet` · `WebSockets`  
  Sub-200ms voice and vision assistant. Local VAD audio stream into faster-whisper over raw PCM chunks, direct screen vision reasoning without OCR latency, and background rolling memory summarization.

* **OpenClaw — Enterprise Autonomous Multi-Agent Platform**  
  `Python` · `FastAPI` · `LangGraph` · `Temporal` · `MCP` · `Qdrant` · `vLLM` · `AST` · `Docker`  
  Autonomous engineering agent platform for AST-level code refactoring, PR verification, and telemetry triage. Decoupled MCP tool servers, hybrid retrieval (Qdrant + BM25 + BGE reranker), and continuous-batching vLLM inference (`Llama-3.3-70B`, `Qwen-2.5-Coder`) with tiered fallback to frontier models.

* **High-Throughput EVM Node Indexer & Relayer Engine**  
  `Go` · `Solidity (Foundry)` · `Yul` · `EIP-712` · `ClickHouse` · `PostgreSQL` · `Redis` · `Reth / Geth`  
  Custom Go event indexer streaming real-time EVM state changes directly from node WebSockets into ClickHouse with reorg state rollbacks, paired with EIP-712 gasless session authorization and MEV-resistant private transaction relayers.
