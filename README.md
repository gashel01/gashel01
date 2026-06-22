# Hi, I'm Gaël Gaussens 👋

**Full-stack engineer — 8 years across the stack, now building AI systems.** I own features end to end: architecture → API → UI → deploy. Most recently I built **MCP AI Suite**, a governed AI-agent orchestration platform — engine, product, and site, front to back.

📍 Ibiza, Spain · fully remote · **open to senior frontend / full-stack / AI engineering roles**
🔗 [mcpaisuite.com](https://mcpaisuite.com) · [LinkedIn](https://www.linkedin.com/in/gaelgaussens/) · 📫 contact@mcpaisuite.com

---

## 💼 Background

[42](https://42.fr) alum (started at the Silicon Valley campus). 8 years shipping production web apps end to end — from co-founding a software studio (ride-hailing app, transport ERP, booking platform) to enterprise fintech.

→ Full work history on **[LinkedIn](https://www.linkedin.com/in/gaelgaussens/)**.

---

## 🧩 MCP AI Suite — my deep-dive into production AI

A **governed orchestration suite for AI agents** + a **full-stack control hub**, built solo, front to back. The thesis: agent frameworks are easy to demo and hard to run safely and cheaply — so the engine is built around a single **governed chokepoint** (budget, RBAC, DLP secret-redaction, audit) and a **compile-once planner (LTP)** that makes multi-step runs deterministic and token-cheap — with a real product wrapped around it, not just a library.

**The engine (Python · AI)**
- **Governed kernel** — every tool call passes one enforcement point: per-task/namespace budgets, RBAC, DLP secret redaction/blocking, full audit. Deterministic, not asked of the model.
- **LTP (compile-once planning)** — compiles a goal into a verifiable plan in one LLM call; **provable plans** statically reject unsafe steps *before* execution. Benchmark-driven vs LangGraph & CrewAI — reproducible, honest numbers, including where it loses.
- **10 libraries, 4 surfaces each** (Python lib · CLI · MCP server · FastAPI), on PyPI under Apache-2.0: orchestrator, planner, RAG (rerank / SPLADE / ColPali), tiered memory, eval (native RAG metrics), polyglot sandbox, scheduler, web search, workspace.

**The product (TypeScript · React/Next · full-stack)**
- **Control Hub** — a Next.js + FastAPI app: live execution **observability**, **time-travel replay**, a **visual graph builder** (ReactFlow) that actually runs, **plan-diff**, A/B-tested constitutions, deploy-an-agent-as-an-API, and a conversational "chat-to-build" team designer.
- **Marketing/docs site** ([mcpaisuite.com](https://mcpaisuite.com)) — Astro, with benchmarks wired from real result receipts.

**Ops** — Prometheus `/metrics` + OpenTelemetry, Docker, Kubernetes/Helm.

```bash
pip install mcpaisuite-kernelmcp     # the governed orchestrator (+ the rest of the suite)
```

→ Architecture, benchmarks, live demos: **[mcpaisuite.com](https://mcpaisuite.com)**

---

## 🛠 Tech

**Frontend:** TypeScript · React · Next.js · Tailwind · ReactFlow · D3.js · Cytoscape.js · Redux · data-viz / dashboards
**Backend / AI:** Python · FastAPI · MCP protocol · litellm · async · LLM orchestration · RAG / vector search
**Data / Infra:** PostgreSQL · Neo4j · Redis · Docker · Kubernetes / Helm · Azure · Prometheus · OpenTelemetry

I like working across the stack — designing an API and the UI that consumes it in the same afternoon — with AI systems as the throughline.

---

<sub>Open to senior frontend / full-stack / AI engineering roles — fully remote. The MCP AI Suite libraries are open source (Apache-2.0) on PyPI; ping me for a walkthrough.</sub>

<!-- profile -->
