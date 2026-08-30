# Hi, I'm Aryan

Software engineer building AI infrastructure, distributed systems, and GPU-accelerated ML. I'd rather find out why something is slow than paper over it — the retrieval layer that's fine until it isn't, the scheduler nobody thinks about until it starves a process, the CUDA kernel that's the real reason training got 3x faster.

**85%** query latency reduced (RAG platform, 100+ enterprise clients) · **340x** CUDA kernel speedup · **74%** top-3 root-cause accuracy on a black-box LLM-serving diagnosis pipeline

## Currently

- Finishing an M.S. in Computer Science at NC State (GPA 3.85/4.0) — advanced distributed systems, GenAI for computer systems, parallel systems, performance modeling
- Contributing to [SGLang](https://github.com/sgl-project/sglang) — starting with Prometheus observability for KV-cache usage
- On F-1 OPT, authorized to work in the US now

## Featured Projects

**[vLLM RCA — Root-Cause Localization for p99 TTFT](https://github.com/aryansharma2k2/vllm-blackbox-rca)**
When p99 time-to-first-token spikes on a vLLM server, which subsystem caused it? KV-cache pressure, prefix-cache collapse, and batch scheduling all look alike and cause each other. This pipeline names the actual cause from Prometheus metrics alone — no profiler, no tracing. 74% top-3 accuracy across 38 labeled GPU runs, silent on all 8 clean ones, benchmarked against threshold alerting, correlation ranking, and Claude Opus 5 given identical evidence. [Full writeup](https://aryansharma2k2.github.io/vllm-blackbox-rca/)

**[CUDA-Optimized LSTM Sentiment Analyzer](https://github.com/aryansharma2k2/CUDA-optimized-Movie-Classifier)**
PyTorch's LSTM was the bottleneck, so I rewrote it. Four hand-written CUDA kernels — embedding lookup, LSTM cell, tiled matmul, fused loss — took embedding lookup from 20.4ms to 0.06ms and training from 24s to 8s per epoch.

**[NeuroCache: LLM-Driven Cache Policy Discovery](https://github.com/aryansharma2k2/NeuroCache-LLM-Driven-Policies)**
A FunSearch-style loop where an LLM generates a cache replacement policy, compiles it, simulates it in ChampSim, and evolves it against LRU and DRRIP.

**[XINU OS: Kernel Internals Reimplementation](https://github.com/aryansharma2k2/XINU-OS)**
Textbook priority scheduling starves low-priority processes, so I wrote two replacements from scratch, plus demand paging, a syscall tracer, and a disk defragmenter — all inside a Unix-like kernel on QEMU.

**[Expertiza — Open Source Contributions](https://github.com/expertiza)**
Rebuilt the participant-management page of an NSF-supported peer-review platform (used across NC State and partner universities) in React/TypeScript against a live Rails backend — real CRUD, real permissions.

More at [my portfolio](https://aryansharma2k2.github.io/).

## Tech Stack

**Languages:** Python, Java, C, C++, JavaScript, TypeScript, SQL, Ruby
**Frameworks:** TensorFlow, PyTorch, Flask, Spring, Spring Boot, Ruby on Rails, Django, React, LangChain, LlamaIndex, Spark
**GPU / Performance:** CUDA (custom kernels, shared-memory tiling, warp-level reductions, kernel fusion), NVIDIA Nsight, PyTorch C++ bindings
**Cloud / Infra:** AWS (EC2, S3, OpenSearch Serverless, Bedrock), Docker, Kubernetes, Prometheus, Grafana, Chaos Mesh, Helm
**Databases:** PostgreSQL, MySQL, MongoDB, Redis, OpenSearch, ChromaDB, Qdrant, FAISS
**Tools:** Git, Jenkins, Wireshark, Jupyter Notebooks
**AI & ML:** Machine Learning, Deep Learning, NLP, Generative AI, RAG pipelines, Data Engineering, Image Processing

## Let's Connect

[LinkedIn](https://linkedin.com/in/aryansharma2k2) · [inguvaaryan22@gmail.com](mailto:inguvaaryan22@gmail.com) · [Portfolio](https://aryansharma2k2.github.io/)

<!--
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=aryansharma2k2&show_icons=true&count_private=true&hide_title=true)
-->
