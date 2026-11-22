<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:00ADD8,50:6E40C9,100:FF6AC1&text=Peeyush%20Mishra&fontColor=ffffff&fontSize=52&fontAlignY=40&desc=Backend%20engineer%20%C2%B7%20Go%20%C2%B7%20LLM%20systems%20%C2%B7%20Retrieval&descAlignY=62&descSize=18" width="100%" alt="Peeyush Mishra" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-peeyush--m-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/peeyush-m)
[![X](https://img.shields.io/badge/@mipeeyush-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/mipeeyush)

</div>

## About

I'm a backend engineer working on AI products at **OnDemand AI** and **SchoolHack AI**, both part of AIREV Holding. I work mostly in Go, with some Node.js, on the backend side of LLM products: media processing, retrieval, model routing and agent orchestration.

It's team work on shared codebases, so I'd rather describe what I've worked on than claim whole systems. I studied materials science at NIT Calicut, which is probably why I like measuring things before I believe them.

## Experience

| When | Where | Highlights |
|---|---|---|
| Aug 2025 to now | **OnDemand AI**, Senior Software Engineer | Contributing across the platform's Go services: LLM gateway, media pipeline, storage and agent orchestration, plus custom solutions for clients |
| Mar 2024 to Jul 2025 | **OnDemand AI**, Software Engineer | Queue-driven media processing, embeddings and search, and the services around them |
| Aug 2025 to now | **SchoolHack AI**, Senior Software Engineer | Backend for a platform with 3.4M+ active users and 165M+ queries handled |
| Jul 2023 to Jul 2025 | **SchoolHack AI**, Software Engineer | Core backend and third-party integrations while the platform scaled |

Earlier: data analyst at a healthcare analytics company, and backend and data internships in insurance software and energy.

## What I've worked on

- **Media pipelines.** Queue-driven processing for documents, audio, video and images: transcription, OCR, thumbnails and embeddings. Explicit retry rules, idempotent jobs and bounded concurrency so a bad file doesn't take the workers down.
- **Retrieval.** Vector search on top of model-generated embeddings: hybrid dense and keyword search, reranking behind feature flags, and separate hot and cold vector collections.
- **LLM gateway.** One interface over many model providers: streaming, tool calling, structured output, reasoning controls, and OCR routing with fallbacks. It's also where embeddings are generated, with request chunking, configurable dimensions and several embedding providers.
- **Agent orchestration.** Planning multi-step runs across plugins, validating parameters against JSON schemas, and streaming results back as they finish.
- **Storage access.** Signed-URL access across several cloud storage providers, with ownership checks on every write and delete.
- **Data collection.** Scraping plus LLM extraction, geo search, background jobs and push notifications for a consumer app backend.
- **Keeping it healthy.** Tracing and metrics, dependency patching, and security scans in CI.

Most of this is in private company repos, so there isn't much to show here. Happy to talk through any of it.

## A typical retrieval pipeline

```mermaid
flowchart LR
    A[Documents and media] --> B[Extract, OCR, transcribe]
    B --> C[Chunk]
    C --> D[Embed: dense and keyword]
    D --> E[(Vector store)]
    Q[Question] --> F[Hybrid search]
    E --> F
    F --> G[Rerank]
    G --> H[Prompt]
    H --> I[LLM]
    I --> J[Answer with sources]
```

When these systems give bad answers, the problem is usually on the left side of this diagram (extraction, chunking, search) and not the model.

## Tech stack

| | |
|---|---|
| **Languages** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| **Services** | ![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=flat-square&logo=grpc&logoColor=white) ![Gin](https://img.shields.io/badge/Gin-008ECF?style=flat-square&logo=gin&logoColor=white) ![Job queues](https://img.shields.io/badge/Job_queues-DC382D?style=flat-square) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) |
| **AI** | ![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white) ![Embeddings](https://img.shields.io/badge/Embeddings-0A66C2?style=flat-square) ![Hybrid search](https://img.shields.io/badge/Hybrid_search-6E40C9?style=flat-square) ![LLM APIs](https://img.shields.io/badge/LLM_APIs-FF6AC1?style=flat-square) ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white) ![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white) |
| **Infra** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) ![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white) |
| **Observability** | ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) |

## Get in touch

I'm open to collaborating, especially on Go, retrieval and agent projects. Message me on [LinkedIn](https://linkedin.com/in/peeyush-m) or [X](https://x.com/mipeeyush).
