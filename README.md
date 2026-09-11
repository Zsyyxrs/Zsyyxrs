## Hi, I'm Shangyi Zhu 👋

**AI Algorithm Engineer** based in Shanghai, focused on **LLM applications & Agent systems**.

7 years of engineering experience — 5 years building large-scale data infrastructure at NIO (autonomous driving data) and SAIC-GM (intelligent connected vehicles), and 2+ years transitioning into LLM application development. Currently building a multi-agent Q&A platform for the banking domain.

I work at the intersection of **data engineering and LLMs** — turning messy enterprise data into reliable AI products.

---

### 🔭 What I'm working on

- **ChatBI Agent** — Conversational BI for banking: one question → SQL → chart → automated root-cause
  attribution. Three paths (precise retrieval / multi-step analysis / RCA), a YAML semantic layer with
  render-time row-level access control, and a reproducible eval harness benchmarked against BIRD.
- **Bank Intelligent Q&A Platform** — Multi-agent architecture with NL2SQL, RAG, and tool-calling routing. Built on LangGraph with BGE-M3 hybrid retrieval and Qwen-series models.
- **Medical RAG System** — Tri-modal hybrid retrieval (dense + sparse + ColBERT) over Milvus/HNSW, with LangGraph orchestration and RAGAS evaluation. ChatGLM3-6B fine-tuned with LoRA/QLoRA.
- **Exploring** — Multimodal agents, agent evaluation frameworks, and production deployment patterns (vLLM, quantization).

---

### 🛠️ Tech Stack

**LLM & Agents**
`LangGraph` · `LangChain` · `RAG` · `NL2SQL` · `vLLM` · `LoRA/QLoRA` · `RAGAS`

**Models & Frameworks**
`Qwen` · `ChatGLM` · `BGE-M3` · `PyTorch` · `Transformers` · `PEFT`

**Data & Infra**
`Milvus` · `Doris` · `ClickHouse` · `Hive` · `Iceberg` · `Spark` · `Flink` · `PostgreSQL`

**Observability & Protocols**
`Langfuse` · `MCP` · `sqlglot` · `Streamlit`

**Languages & Tools**
`Python` · `SQL` · `Java` · `Docker` · `Git` · `Linux`

---

### 📌 Selected Projects

| Project | Stack | Highlights |
|---|---|---|
| **ChatBI Agent** | Python, Qwen3.7-Max, PostgreSQL, sqlglot, Langfuse, Streamlit, MCP | Conversational BI for banking with three paths — precise NL2SQL retrieval, multi-step analysis, and RCA attribution; YAML semantic layer of 21 governed metrics with an embedding prefilter router (precision 1.000 / recall 0.75 on a 34-question ruler) emitting deterministic template SQL; render-time row-level access control that is fail-closed and never reaches the LLM prompt; reproducible eval harness (P1 0.977 / P2 0.626 / P3 0.900, event-hit 7/7) with zero-LLM offline rescoring for scorer changes; BIRD-financial dev subset (n=106) as external benchmark — dialect parameterization took syntax errors 27 → 0 and closed 38% of the gap to a BIRD-specific baseline; MCP server exposing the retrieval path to Claude Desktop under a server-side identity lock |
| **Medical RAG System** | FastAPI, LangChain, Milvus, Qwen, ChromaDB | Retrieval-first multi-turn clarification dialogue for medical education & clinical support, SufficiencyJudgement state machine for dynamic query refinement, medical knowledge base chunking with hybrid BM25+dense retrieval, support for clinical decision-making queries with cited evidence, end-to-end integration tests with state transition coverage |
| **Smart Crib Guard** | PyTorch, Qwen2.5-VL-7B, PEFT (LoRA), Transformers, OpenCV | 9-class baby behavior recognition via Qwen2.5-VL-7B LoRA fine-tuning (Loss: 0.0175), automated video frame extraction + multi-strategy augmentation (brightness/rotation/crop/flip), JSON-standardized annotation pipeline, real-time inference with confusion matrix generation, edge-cloud integrated monitoring |
| **Legal RAG System** | FastAPI, ChromaDB, bge-zh, Qwen3 | Statute-aware article-level chunking, hybrid BM25+dense retrieval, query rewriting, cited answers with confidence scoring |
| **Positive Chinese Chatbot** | PyTorch, ChatGLM3-6B, LoRA, Gradio | LoRA fine-tuning on Douban "夸夸" corpus for encouraging replies, Trie-based dirty-word filter with variant/homophone detection, multi-strategy decoding with BLEU/ROUGE/diversity evaluation |
| **Chinese Sentiment Classifier** | PyTorch, BERT-base-Chinese, Transformers, ChnSentiCorp | Selective last-N layer unfreezing on BERT with weighted sampling and jieba synonym augmentation, AMP + warmup-linear LR + early stopping, MC-dropout uncertainty and attention-based explainability, 94.5% Acc / AUC 0.983 |



---

### 📫 Get in touch

Open to opportunities in **LLM / Agent engineering** — particularly roles involving data agents, RAG systems, or multimodal applications.

Feel free to reach out via GitHub.
