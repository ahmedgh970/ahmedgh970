# Ahmed Ghorbel

**AI Engineer | LLM Systems · Advanced RAG · Agentic AI · Generative Models**

I build and deploy AI systems, from generative model research to production-oriented LLM applications.

My current focus is on **advanced RAG, agentic workflows, LLM evaluation, and efficient inference**, from local-first open-weight stacks to **Microsoft Foundry** on Azure, with an emphasis on measurable quality, reliability, and cost.

My background spans generative modeling, computer vision, and neural compression, combining deep learning research with practical AI engineering.

**Approach:** benchmark first, change one variable at a time, and keep complexity only when it delivers measurable gains.

---

## 🚀 Featured Projects

### [FinQA Azure — RAG & Agents on Microsoft Foundry](https://github.com/ahmedgh970/finqa-azure)

A cloud-native question-answering system over 84 financial filings (10-K, 10-Q, 8-K, earnings releases; 12,013 pages), built on Azure AI Search, Azure OpenAI and Microsoft Foundry, and evaluated on the 150 FinanceBench questions.

**Key engineering highlights:**

- **Agentic RAG with Foundry Agent Service** — GPT-5.2 agent with strict function tools (filing catalog, search, safe calculator) under per-question budgets: answers 91% of questions vs 69% for the best single-pass RAG, with 46 of 48 figures exact (McNemar p = 0.012).
- **Hybrid retrieval on Azure AI Search** — BM25 + vector search fused with RRF, then semantic reranking (+0.32 completeness, 95% CI [+0.15, +0.51]); metadata filters extracted from the question lift top-5 document hits from 49% to 92%. Layout-based parsing was benchmarked and discarded.
- **Grounded generation** — Structured outputs with numbered citations and verbatim quotes verified by code; the answer status is computed by the application, not the model.
- **LLM & agent evaluation** — Azure AI Evaluation with a judge distinct from the generator, deterministic figure checks, agent evaluators (Tool Call Accuracy 4.66/5, Intent Resolution 4.81/5), paired bootstrap and McNemar tests.
- **Production deployment** — Chatbot deployed as a Foundry hosted agent (ZIP code deployment, Responses protocol) with conversation memory, tools called only when needed, and its own Microsoft Entra agent identity with least-privilege RBAC.
- **Observability & security** — End-to-end OpenTelemetry traces (GenAI semantic conventions) in Application Insights; keyless Entra authentication, content-safety guardrails, and defense in depth against indirect prompt injection.
- **Cost & quality engineering** — Per-question cost caps (≈ $0.04 per agent answer), architecture decision records backed by measurements, 290 automated tests, mypy strict.

### [FinQA Engine — Advanced RAG & Agentic Financial QA](https://github.com/ahmedgh970/finqa-engine)

An evaluation-driven, fully local RAG system for question answering over financial documents, built with open-weight LLMs.

**Key engineering highlights:**

- **Retrieval optimization** — Dense retrieval (BGE-M3) and Cross-Encoder reranking, improving Recall@10 from 0.30 to 0.65. BM25 and hybrid RRF were benchmarked and discarded based on evaluation results.
- **Agentic RAG** — LangGraph workflow with passage relevance grading and contextual retrieval, reducing token consumption by 56% at equivalent answer quality.
- **LLM evaluation** — Benchmarking of 10 open-weight LLMs, evidence-grounded answer evaluation, and a validated LLM-as-a-Judge methodology.
- **Verified computation** — Tool-assisted financial calculations with exact decimal arithmetic and evidence verification.
- **LLM serving** — Local inference with vLLM and GPU-based deployment.
- **LLMOps** — FastAPI, Docker, CI/CD, 210 automated tests, and distributed tracing with OpenTelemetry, Phoenix, and Langfuse.

---

## 🧰 Tech Stack

**LLM & Agentic AI**  
LangGraph · LangChain · Hugging Face Transformers · Ollama · vLLM

**Azure AI**  
Microsoft Foundry (Agent Service, hosted agents) · Azure OpenAI · Azure AI Search · Azure AI Evaluation · Application Insights · Microsoft Entra ID

**RAG & Document Intelligence**  
Qdrant · BGE-M3 · Cross-Encoder Reranking · Docling · Dense, Hybrid & Semantic Retrieval

**Evaluation & Observability**  
LLM-as-a-Judge · Agent Evaluators · Retrieval Metrics · Langfuse · Arize Phoenix · OpenTelemetry

**Deep Learning & Generative AI**  
PyTorch · TensorFlow · Diffusers · Flow Matching · Transformers

**Backend & MLOps**  
Python · FastAPI · Pydantic · Docker · GitHub Actions · Pytest · Ruff · mypy · Linux

---

## 🔬 Research Background

**Generative AI**
- Diffusion and flow-matching models for image, video, and audio generation and editing.
- Generative motion forecasting and multi-agent traffic simulation.
- Efficient generative architectures combining attention and state-space models.

**Computer Vision & Model Optimization**
- Learned image and video compression outperforming VVC reference implementations on evaluated benchmarks.
- Implicit Neural Representations (INR) for neural video coding.
- Model pruning, quantization, and knowledge distillation.
- Unsupervised anomaly detection and segmentation in medical imaging.

**Selected publications:** IEEE ICIP 2023 · EUVIP 2023 · IEEE VCIP 2024 · ICLR 2026 Workshop · [Google Scholar](https://scholar.google.com/citations?user=4OX0gTwAAAAJ)

---

## 📫 Connect

- **Email:** [ghorbel.ahmd@gmail.com](mailto:ghorbel.ahmd@gmail.com)
- **LinkedIn:** [ahmed-ghorbel97](https://www.linkedin.com/in/ahmed-ghorbel97)
- **Google Scholar:** [Ahmed Ghorbel](https://scholar.google.com/citations?user=4OX0gTwAAAAJ)
