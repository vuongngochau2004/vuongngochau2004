<h1 align="center">Hi, I'm Hau 👋</h1>

<p align="center">
  <b>Backend & AI Engineer (fresher)</b> · Da Nang, Vietnam · <b>Open to remote roles</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/vuongngochau2004/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:YOUR_EMAIL@example.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## What I do

I'm a backend engineer who builds the systems behind LLM applications: **retrieval pipelines, streaming APIs, document ingestion, and the auth and data layers around them**. I care about retrieval quality, measurable results, and code that other people can run and maintain.

- **Backend:** Python, FastAPI, PostgreSQL, Redis, Celery, Docker
- **AI / LLM:** RAG, hybrid search (dense + BM25), embeddings, OCR ingestion, tool-calling, MCP
- **Working style:** async-friendly, documentation-first, comfortable working in a team and reviewing PRs

---

## Selected work

### 🔎 [KIRA](https://github.com/vuongngochau2004/kira): RAG assistant for Vietnamese documents

**Problem.** Pure vector search often misses exact-term queries (names, article numbers, codes), and scanned PDFs break ingestion.

**What it does.** Upload documents, then chat with them and get answers with citations, streamed in real time. Each user gets isolated documents and indexes.

**Key engineering decisions**
- **Hybrid retrieval:** dense search (Qdrant, `BAAI/bge-m3`) combined with BM25 via Reciprocal Rank Fusion, so both semantic and exact-match queries work.
- **Robust ingestion:** asynchronous OCR (PaddleOCR) with low-quality-text detection to fall back to OCR for scanned PDFs.
- **Layered architecture:** serving, agent/tools, retrieval, and ingestion are separated, with a semantic routing layer on top.
- **Security:** JWT auth, migrated from localStorage tokens to **httpOnly cookies**.
- **Quality:** unit and integration tests, Alembic migrations, Docker Compose, architecture docs.

**Results.** <!-- TODO: fill in real numbers, e.g. "Hybrid retrieval raised hit-rate@5 from X% to Y% on N hand-labeled Vietnamese questions" -->

**My part.** <!-- TODO: state exactly what you built, since the repo has other contributors -->

`Python` `FastAPI` `Qdrant` `LangChain` `PostgreSQL` `Docker`

---

### 💬 [Zalo MCP Server](https://github.com/vuongngochau2004/claude-desktop-mcp-zalo): giving Claude access to Zalo

An MCP (Model Context Protocol) server in TypeScript that exposes 20+ tools so Claude Desktop can read contacts and groups, fetch chat history, and send messages through a logged-in Zalo session. Built to explore how LLM agents can work with the messaging apps people actually use in Vietnam.

*Experimental project for personal use; it relies on an unofficial Zalo client library.*

`TypeScript` `Node.js` `MCP`

---

## Team projects

I've also worked on several team projects that live in private repositories (full-stack apps with FastAPI, PostgreSQL, Redis/Celery and Docker). I'm happy to walk through the architecture and my contributions in an interview.

---

## Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Let's connect

I'm looking for a **remote Backend / AI Engineer** role where I can keep learning from experienced engineers and ship real features. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/vuongngochau2004/) or email.
