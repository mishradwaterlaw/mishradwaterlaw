<div align="center">

# Tezash Mishra

**Backend Engineer · CNCF Open Source Contributor · Builder**

Designing distributed systems, async pipelines, and shipping real code to production codebases.

</div>

---

## About Me

Second-year Information Technology student at JSS Science and Technology University. I build backend systems and contribute to open source production codebases. Not waiting to be senior enough to do real work.

- Merged a bug fix in **kubernetes-sigs/kueue** (CNCF) fixing a Kubernetes 1.35 API regression in the MultiKueue controller
- Opened PR which Fixes security vulnerabilities (argument injection, WebSocket hijacking) in **Headlamp**, a CNCF Sandbox project
- Built **EchoSort** — an async photo-retrieval platform with Redis Streams crash recovery, pgvector HNSW search, and a serverless ONNX ML worker


---

## Open Source

| Project | Org | What I did |
|---|---|---|
| [kueue](https://github.com/kubernetes-sigs/kueue) | CNCF / kubernetes-sigs | Merged PR #17059 — fixed Kubernetes 1.35 API regression in MultiKueue re-dispatch eviction loop |
| [Headlamp](https://github.com/headlamp-k8s/headlamp) | CNCF Sandbox | Fixed RBAC permission bug (#5908), React Hooks violations (#6769), argument injection and WebSocket hijacking vulnerabilities |
| [Layer5](https://github.com/layer5io/layer5) | CNCF Member Org | Dark mode implementation (#7761), CSS layout fixes (#7764, #7743) |

---

## Featured Projects

**[EchoSort](https://github.com/mishradwaterlaw/echosort)** — Event photo retrieval using face recognition

Attendees upload a selfie and get back every photo of them from the event. Built the entire system solo.

- Async pipeline: FastAPI enqueues jobs to Redis Streams via XADD; Modal serverless worker drains via XREADGROUP/XACK; crashed workers reclaim jobs from Pending Entries List via XAUTOCLAIM
- Face retrieval: InsightFace buffalo_l (SCRFD-10G + ArcFace ResNet50) on ONNX Runtime CPU; 512-D embeddings stored in pgvector with HNSW index, searched via cosine distance in a single Postgres RPC
- Cost: ONNX CPU over GPU cut inference cost by over 85%; pre-baked model weights in Modal container cut cold start from ~20s to under 1.5s
- Stack: Next.js, FastAPI, PostgreSQL + pgvector, Redis Streams, InsightFace ONNX, Supabase, Modal, Docker

**[K8s Copilot](https://github.com/mishradwaterlaw/k8s-copilot)** — Multi-agent Kubernetes root cause analysis

- Parallel Deploy and Log Investigator agents in LangGraph merge findings via state reducers
- Confidence-scored synthesis with conditional re-run router (up to 3 loops) and human-in-the-loop approval via LangGraph interrupts with SQLite checkpointing
- Stack: LangGraph, FastAPI, Python, SQLite

**ORCA** — Marine safety advisory platform (Smart India Hackathon)

- LangGraph multi-agent backend with Gemini-powered supervisor routing to parallel risk agents
- Rule-based risk engine: wave height + wind speed thresholds to Safe/Caution/Unsafe with highest-severity-wins roll-up
- Stack: LangGraph, FastAPI, Gemini, React, Folium

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

**Backend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logoColor=white)

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

**Databases & Messaging**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

**ML & Vector Search**

![ONNX](https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Modal](https://img.shields.io/badge/Modal-000000?style=for-the-badge&logoColor=white)

---

## Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/tezashmishra)

**tezashmishra@outlook.com**
