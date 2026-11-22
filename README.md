<div align="center">

<img src="assets/hero.svg" width="100%" alt="Terminal: Peeyush Mishra, backend engineer. Go, gRPC, job queues, hybrid search, LLM gateways." />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-peeyush--m-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/peeyush-m)
[![X](https://img.shields.io/badge/@mipeeyush-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/mipeeyush)
![Open to collaborating](https://img.shields.io/badge/Open_to-collaborating-2EA043?style=for-the-badge)

</div>

<br/>

I'm a backend engineer on AI products at **OnDemand AI** and **SchoolHack AI** (part of AIREV Holding). I work mostly in Go, with some Node.js, on the parts of LLM products that sit behind the chat box: media processing, retrieval, model routing and agent orchestration.

It's team work on shared codebases, so I describe what I've worked on rather than claim whole systems. I studied materials science at NIT Calicut, which is probably why I like measuring things before I believe them.

<table>
<tr>
<td width="33%" valign="top">

**Focus**<br/>
LLM gateways, retrieval, media pipelines, agent orchestration

</td>
<td width="33%" valign="top">

**Daily drivers**<br/>
Go · gRPC · Redis queues · MongoDB · Qdrant

</td>
<td width="33%" valign="top">

**Scale**<br/>
A platform with 3.4M+ active users and 165M+ queries handled

</td>
</tr>
</table>

## What I've worked on

<table>
<tr>
<td width="50%" valign="top">

### Media pipelines
Queue-driven processing for documents, audio, video and images: transcription, OCR, thumbnails and embeddings. Explicit retry rules, idempotent jobs and bounded concurrency, so one bad file can't take the workers down.

</td>
<td width="50%" valign="top">

### Retrieval
Vector search on top of model-generated embeddings: hybrid dense and keyword search, reranking behind feature flags, and separate hot and cold vector collections.

</td>
</tr>
<tr>
<td valign="top">

### LLM gateway
One interface over many model providers: streaming, tool calling, structured output, reasoning controls and OCR routing with fallbacks. Also where embeddings are generated, with request chunking, configurable dimensions and several providers.

</td>
<td valign="top">

### Agent orchestration
Planning multi-step runs across plugins, validating parameters against JSON schemas, and streaming results back as each step finishes.

</td>
</tr>
<tr>
<td valign="top">

### Storage access
Signed-URL access across several cloud storage providers, with ownership checks on every write and delete.

</td>
<td valign="top">

### Data collection
Scraping plus LLM extraction, geo search, background jobs and push notifications for a consumer app backend.

</td>
</tr>
</table>

Most of this is in private company repos, so there isn't much to show here. Happy to talk through any of it.

## How a retrieval pipeline flows

<div align="center">
<img src="assets/pipeline.svg" width="100%" alt="Pipeline: ingest, extract, embed, index, search, rerank, LLM, answer with sources." />
</div>

## Experience

<details open>
<summary><b>OnDemand AI</b> · Senior Software Engineer · Aug 2025 to now</summary>
<br/>

Contributing across the platform's Go services: LLM gateway, media pipeline, storage and agent orchestration, plus custom solutions for clients.

Before that, **Software Engineer** (Mar 2024 to Jul 2025): queue-driven media processing, embeddings and search, and the services around them.

</details>

<details open>
<summary><b>SchoolHack AI</b> · Senior Software Engineer · Aug 2025 to now</summary>
<br/>

Backend for an AI education platform with 3.4M+ active users and 165M+ queries handled.

Before that, **Software Engineer** (Jul 2023 to Jul 2025): core backend and third-party integrations while the platform scaled.

</details>

<details>
<summary><b>Earlier</b></summary>
<br/>

Data analyst at a healthcare analytics company, plus backend and data internships in insurance software and energy.

</details>

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
