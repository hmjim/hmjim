<p align="center">
  <img src="https://raw.githubusercontent.com/hmjim/hmjim/main/assets/hero.svg?v=4" width="100%" alt="Principal AI & Blockchain Systems Architect" />
</p>

<table width="100%">
  <tr>
    <td width="33%" valign="top">
      <b>AI Infrastructure &amp; Agentic Systems</b>
      <ul>
        <li><b>LangGraph</b> state machines &amp; <b>Temporal.io</b> durable agent execution.</li>
        <li><b>Model Context Protocol (MCP)</b> server architecture, AST code tooling &amp; sandboxed Docker runtimes.</li>
        <li>Self-hosted GPU inference: <b>vLLM</b> (PagedAttention, Chunked Prefill, AWQ/FP8, continuous batching) + Redis semantic cache.</li>
        <li>Hybrid RAG: <b>Qdrant</b> dense vectors + <b>BM25</b> lexical search + <b>BGE-Reranker</b> cross-encoders.</li>
        <li>Real-time multimodal: <b>Silero VAD</b> + <b>faster-whisper</b> raw PCM streaming (&lt;200ms) + Vision LLMs.</li>
        <li>Programmatic optimization &amp; CI evals: <b>DSPy</b>, <b>Arize Phoenix</b>.</li>
      </ul>
      <p><sub><code>Python</code> <code>PyTorch</code> <code>vLLM</code> <code>LangGraph</code> <code>MCP</code> <code>Temporal</code> <code>Qdrant</code> <code>faster-whisper</code> <code>DSPy</code> <code>Phoenix</code></sub></p>
    </td>
    <td width="33%" valign="top">
      <b>Blockchain, EVM &amp; Algo-Trading</b>
      <ul>
        <li><b>Solidity</b> &amp; <b>Yul</b> inline assembly (<b>Foundry</b>, <b>Slither</b>): transient storage (<b>EIP-1153</b>), 256-bit slot packing, <b>ERC-4337</b>, <b>EIP-712</b> gasless auth.</li>
        <li>Custom execution-layer indexers in <b>Go</b> over <b>Reth / Geth</b> JSON-RPC &amp; WebSockets (<code>eth_subscribe</code>, <code>trace_block</code>) with <code>parentHash</code> reorg state rollbacks.</li>
        <li>MEV-resistant tx relayers: distributed Redis sequential nonce locks, EIP-1559 fee engines, <b>Flashbots</b> private bundles.</li>
        <li>Crypto algorithmic trading engines: low-latency WebSocket orderbook ingestion, grid execution &amp; idempotent balance accounting.</li>
      </ul>
      <p><sub><code>Solidity</code> <code>Yul</code> <code>Foundry</code> <code>Go</code> <code>EIP-1153</code> <code>ERC-4337</code> <code>EIP-712</code> <code>Viem</code> <code>Reth/Geth</code> <code>Flashbots</code></sub></p>
    </td>
    <td width="33%" valign="top">
      <b>High-Load Core &amp; Distributed Data</b>
      <ul>
        <li>Sole tech lead across 20+ production platforms handling <b>50TB+ daily traffic</b>.</li>
        <li><b>PostgreSQL</b> declarative partitioning &amp; planner tuning (<code>EXPLAIN ANALYZE</code>); <b>ClickHouse</b> (MergeTree) sub-second analytics over 100M+ rows.</li>
        <li>Event-driven pipelines on <b>Apache Kafka (KRaft)</b> with strict idempotency (transactional outbox, atomic upserts, zero data loss).</li>
        <li>Cloud &amp; GPU orchestration: <b>Kubernetes (EKS)</b>, <b>Karpenter</b>, Docker, OpenTelemetry, L7 WAF / DDoS-Guard defense.</li>
      </ul>
      <p><sub><code>Go</code> <code>Python</code> <code>TypeScript</code> <code>PostgreSQL</code> <code>ClickHouse</code> <code>Redis</code> <code>Kafka</code> <code>K8s</code> <code>Karpenter</code> <code>AWS</code></sub></p>
    </td>
  </tr>
</table>
