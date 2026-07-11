# 👋 **Hello, I'm Leandro Cunha**

## 💡 **Senior Applied AI/ML Engineer | LLM Systems & Production Architecture**  

I am a Senior Engineer specializing in production-grade Applied AI , ML and Data engineering.  With 16+ years of engineering experience in mission-critical high-availability systems sectors like Power Grids, Pharma, and Aeronautics. I hold an M.Sc. in AI (Distinction), and I aim to build efficient solutions with modern Deep Learning that perform fast and reliably in the real world.

---

## 🚀 **Core Competencies**

- **AI & Agentic Systems**: **PyTorch**, **LLM Architectures** (RAG, Multi-Agent Systems/CrewAI), LangChain, Computer Vision (OpenCV, OpenVino), Explainable AI.
- **Production MLOps**: **Kubernetes**, **Docker**, **Infrastructure as Code (Terraform, AWS CDK)**, Pipeline Orchestration (Airflow, Dagster, Kedro).
- **Data Engineering at Scale**: **PySpark**, **Databricks**, Distributed Processing, Data Warehousing (BigQuery, Redshift).
- **Languages**: Python (FastAPI), JavaScript (React/Node.js).

---

## 📂 **Featured Projects**

---
### 1.  AI Customer Service Agent
A scenario-based, multi-tenant AI Customer Service Agent platform demonstrating stateful multi-turn customer support, dynamic SOP-adherence RAG, and an asynchronous LLM-as-a-judge compliance evaluation engine.

👉 Live Demo 🚀

Tech Stack: Python | FastAPI (Async) | LangGraph | LangChain | Groq (Llama 3) | Supabase (PostgreSQL + pgvector) | SentenceTransformers | React + Vite | Tailwind CSS | TypeScript | Pytest

🧠Key features and highlights:

Stateful LangGraph Orchestration: Models customer interactions as a structured state graph (Triage -> Retrieval -> Action -> Resolution) to cleanly manage multi-turn conversation history, state transitions, and ticket resolution logic, supporting pre-seeded demo tenants being four currently implemented: Ecommerce, Credit Card, Internet, and E-learning.

Dynamic SOP Context Retrieval (pgvector RAG): Translates customer queries into local vector embeddings on the fly using all-MiniLM-L6-v2 and matches them against tenant-specific SOP rules using a custom vector similarity RPC in Supabase.

Asynchronous Compliance Evaluator: LLM-as-a-judge intercepts agent responses using FastAPI background tasks to execute out-of-band LLM quality audits, shown in a live compliance small dashboard, (evaluating SOP adherence score, tone compliance, policy violations, and hallucination flags) without adding latency to the client response.

Robust Guardrail Protection: Identifies adversarial prompts and instruction-hijacking at the triage layer, dynamically classifying out-of-boundary queries as off-topic to prevent model manipulation. 
[Repo](https://github.com/leovcunha/cx-agent)

---

### 2. Low Latency Web Search-RAG

A resilient, async Web Search-RAG pipeline optimized for low latency Time-to-First-Token (TTFT) using live web data.

👉 [Live Demo](https://pulse-client-1tgj.onrender.com/) 🚀

Tech Stack: Python | FastAPI (Async) | React + Vite | Groq LPU | OpenRouter | Tavily | Cohere Rerank | SlowAPI | Pytest

🧠Key features and highlights:

Intent-Based Routing: Classifies user query intent (chitchat vs. search) at the gateway layer.

Query Transformation & Localization: Reformulates queries in a single pass (resolving pronouns, removing filler) and localizes/translates search terms to match the target geography (e.g., German for Germany).

Geographic Filtering & Brand Anonymization: Filters context sources by geographic region and dynamically classifies query  to either anonymize commercial brands (informational queries) or objectively output vendor details and links (transactional queries).

Reranking (Cohere) : Utilizes cross-encoder relevance models to drop noisy search results (score < 0.6) and selects the top 5 highest-scoring documents for better query match.

Server-Sent Events (SSE) Streaming: Streams real-time pipeline status, search sources, token chunks, and performance metrics to the client on a single HTTP connection using EventSourceResponse.

Client-IP Rate Limiting & Telemetry: Restricts requests using SlowAPI and logs structured JSON telemetry capturing metrics like TTFT, failover status, and the count of search results dropped by the reranker.
[Repo](https://github.com/leovcunha/pulse-rag)

---

### 3. **Movie Recommendation Engine**  
*Collaborative filtering system handling 1M+ user ratings with advanced memory optimization*
[live demo](https://movie-recom.graybeach-1591a263.centralus.azurecontainerapps.io/)
- Hybrid recommendation system (user-based + item-based collaborative filtering)  
- - **Tech**: FastAPI, React, Scipy (sparse matrices), TMDB API, Caching  
- **Key Features**:
  - Hybrid approach: 40% user-based + 60% item-based predictions
  - **Memory optimization**: Dynamic loading based on available RAM, sparse matrices, batch processing (1000-user batches)
  - Cold-start solution: TMDB API integration with intelligent fallback
  - Handles datasets with 1M+ user ratings on resource-constrained machines
  - Model caching for fast inference
- 👉 [`movie-recom` repo](https://github.com/leovcunha/movie-recom)

---

### 4. **Deepfake Detection with CNN+RNN**  
*M.Sc. thesis: Hybrid CNN-RNN architectures for deepfake video detection*

- Deep learning system for detecting forged videos using EfficientNet (CNN) and EfficientNet-GRU (Hybrid)   
- **Tech**: PyTorch, EfficientNet, GRU, Particle Swarm Optimization, Video Processing  
- **Key Features**:
  - Datasets: DFDC (deepfakes), CelebDF-v2 (deepfakes), YouTube Faces (real)
  - Hyperparameter tuning: Manual search + PSO (Particle Swarm Optimization)
  - Architecture comparison: Pure CNN vs. Hybrid CNN-RNN
  - Finetuned model weights available
  - Comprehensive experiment notebooks (data analysis → preliminary → tuning → final testing)
- 👉 [`deepfake_detection_cnn_rnn` repo](https://github.com/leovcunha/deepfake_detection_cnn_rnn)

---

## 🌐 **Let's Connect**

- **LinkedIn**: [Leandro Cunha](https://www.linkedin.com/in/leandro-vcunha/)  

