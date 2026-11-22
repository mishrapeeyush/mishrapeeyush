<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:00ADD8,50:6E40C9,100:FF6AC1&text=Peeyush%20Mishra&fontColor=ffffff&fontSize=52&fontAlignY=40&desc=Backend%20engineer%20%C2%B7%20Go%20%C2%B7%20RAG%20%C2%B7%20LLM%20systems&descAlignY=62&descSize=18" width="100%" alt="Peeyush Mishra" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-peeyush--m-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/peeyush-m)
[![X](https://img.shields.io/badge/@mipeeyush-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/mipeeyush)

</div>

## About

I'm a backend engineer working on AI products at **OnDemand AI** and **SchoolHack AI**, both part of AIREV Holding. Most of my time goes into Go and Node.js services, retrieval (RAG), and the plumbing around LLMs.

I've built 15+ microservices from scratch and led a few client projects from first call to production. Before all this I studied materials science at NIT Calicut, which is probably why I like measuring things before I believe them.

Right now I'm working on:
- RAG systems that answer from private documents
- one clean layer over several LLM providers
- streaming and event-driven backends
- keeping latency and cost down as usage grows

## Experience

| When | Where | Highlights |
|---|---|---|
| Aug 2025 to now | **OnDemand AI**, Senior Software Engineer | Architecture for an AI platform built on RAG, plus custom solutions for clients |
| Mar 2024 to Jul 2025 | **OnDemand AI**, Software Engineer | Built a media-processing service for documents, audio, video and images. Cut vector storage by 92% with cold storage. Moved key services from Node.js to Go for lower memory use and latency |
| Aug 2025 to now | **SchoolHack AI**, Senior Software Engineer | Backend for a platform with 3.4M+ active users and 165M+ queries handled |
| Jul 2023 to Jul 2025 | **SchoolHack AI**, Software Engineer | Core backend and third-party integrations while the platform scaled |

Earlier: data analyst at a healthcare analytics company, and backend and data internships in insurance software and energy.

## What I work on

- **RAG and retrieval.** Letting an LLM answer from your own documents, with sources, and saying "I don't know" when the data isn't there.
- **Agents.** LLMs that call tools and automate repetitive work, with a person approving anything important.
- **Microservices.** gRPC, pub/sub, streaming and realtime chat, mostly in Go.
- **Integrations.** Multiple model providers and third-party APIs behind one interface.
- **Data pipelines.** Turning messy web pages and files into clean, structured data.

Most of this is in private company repos, so there isn't much to show here. Happy to talk through any of it.

## A typical RAG setup

```mermaid
flowchart LR
    A[Documents] --> B[Clean and chunk]
    B --> C[Embed]
    C --> D[(Vector store)]
    Q[Question] --> E[Embed query]
    E --> F{Retrieve and rerank}
    D --> F
    F --> G[Build prompt]
    G --> H[LLM]
    H --> I[Answer with sources]
```

When these systems give bad answers, the problem is usually on the left side of this diagram (chunking, retrieval, context) and not the model.

## Tech stack

| | |
|---|---|
| **AI** | ![RAG](https://img.shields.io/badge/RAG-6E40C9?style=flat-square) ![Embeddings](https://img.shields.io/badge/Embeddings-0A66C2?style=flat-square) ![Agents](https://img.shields.io/badge/Agents-00ADD8?style=flat-square) ![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square) ![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white) ![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white) ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white) ![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white) |
| **Backend** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=flat-square&logo=grpc&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) |
| **Data** | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| **Infra** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) |
| **Also** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white) ![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white) |

## Get in touch

I'm open to collaborating, especially on Go, RAG and agent projects. Message me on [LinkedIn](https://linkedin.com/in/peeyush-m) or [X](https://x.com/mipeeyush).
