Open-source infrastructure for production-ready, event-driven autonomous AI systems.

We build the foundational runtime, memory, and orchestration layers required to run AI agents as reliable, distributed systems — not demos or chatbots.

Our focus is on:
- Event-driven execution
- Multi-agent coordination
- Persistent memory
- Horizontal scalability
- Production reliability

All components are modular, framework-agnostic, and designed to operate independently or as a unified stack.

---

## Projects

### OmniCore Agent
Autonomous AI agent framework for reasoning, tool use, routing, and workflow orchestration.

- Model-agnostic (via LiteLLM)
- Multi-agent patterns (routing, parallel, sequential)
- MCP + local tool support
- Streaming and background execution
- Production-proven in real workloads

→ https://github.com/omnirexflora-labs/omnicoreagent

---

### OmniDaemon (Public Beta)
Event-driven runtime engine that turns agents into scalable, distributed systems.

- Framework-agnostic runtime
- Redis Streams event bus
- Consumer groups and horizontal scaling
- Retries, DLQs, and observability built-in

→ https://github.com/omnirexflora-labs/OmniDaemon

---

### OmniMemory (Alpha v0.0.1)
Persistent, framework-agnostic memory layer for AI agents.

- Cross-session memory persistence
- Hybrid retrieval (semantic + keyword + metadata)
- Multi-tenant isolation
- Redis, PostgreSQL, MongoDB, SQLite backends
- Vector DB integrations (Qdrant, ChromaDB, MongoDB Atlas)

→ https://github.com/omnirexflora-labs/omnimemory

---

## Installation

```bash
uv add omnicoreagent
uv add omnidaemon
uv add omnimemory
````

---

## Design Principles

* Event-driven by default
* Framework-agnostic
* Production-first
* Modular and composable
* Open-source, MIT licensed

---

## Architecture

See [`ARCHITECTURE.md`](./ARCHITECTURE.md) for a high-level system overview.

---

## License

MIT — free for commercial and personal use.
