# OmniRexflora Labs

> **Building the infrastructure layer for autonomous AI systems**

[![GitHub](https://img.shields.io/badge/GitHub-Organization-black?style=flat-square&logo=github)](https://github.com/omnirexflora-labs/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![Open Source](https://img.shields.io/badge/Open%20Source-Yes-green?style=flat-square)](https://opensource.org)
[![Production](https://img.shields.io/badge/Production-Ready-success?style=flat-square)](https://www.linkedin.com/company/santry/)
[![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)](https://www.python.org/)

---

## ✨ Key Highlights

- 🚀 **Production-Proven** — OmniCore Agent v0.2.10 already powers [Santry Technology](https://www.linkedin.com/company/santry/) in production, handling real user workflows at scale.
- 🧠 **Full AI Agent Framework** — OmniCore Agent lets you build autonomous agents with routing, tool orchestration, memory, and scheduling built in.
- 🔌 **Framework-Agnostic Runtime Engine** — OmniDaemon is the universal event-driven control plane, orchestrating messaging, retries, DLQs, metrics, and horizontal scaling for agents from any framework.
- 💾 **Production Memory Layer (In Development)** — OmniMemory delivers multi-tier, persistent, semantic memory with Redis, PostgreSQL, MongoDB, and vector DB integrations.
- ☁️ **Cloud-Native Deployment** — OmniCloud (coming soon) automates multi-cloud deployment, autoscaling, cost controls, and high availability for the entire stack.
- 🌐 **Universal LLM Support** — The Omni stack works with OpenAI, Claude, Gemini, Ollama, and every LiteLLM-compatible model—swap providers without touching agent code.

---

## 🌍 The Vision

**Making AI agent development as modular and composable as today's cloud systems.**

Modern AI systems need more than chat interfaces—they require multi-agent coordination, autonomous event responses, persistent memory, and cloud-scale orchestration. The Omni Stack delivers this using **event-driven architecture**, the same pattern powering Netflix, Uber, and Stripe, now reimagined for AI systems.

We build **open-source AI infrastructure** that empowers developers to deploy and scale autonomous AI agents with the simplicity of modern cloud platforms. **Already powering production systems** and trusted by companies building the future of intelligent automation.

**From experiments to production in minutes, not months.**

---

## 🎯 The Problem We Solve

Today's AI landscape is fragmented, forcing developers to build custom infrastructure for every project:

- **Frameworks** (LangChain, CrewAI, etc.) provide intelligence but lack a production runtime
- **Chatbots** are reactive, not autonomous—they wait for user input instead of reacting to business events
- **Multi-agent systems** require complex orchestration, message queues, and state management
- **Event-driven AI** is missing from most platforms—no way to make agents respond to CRM updates, file uploads, or scheduled triggers
- **Production deployment** demands custom infrastructure for scaling, monitoring, and reliability

**The Omni Stack bridges this gap** by delivering a complete, modular ecosystem for building AI agents as **distributed systems**, not chatbots. We connect reasoning (OmniCore Agent), memory (OmniMemory), orchestration (OmniDaemon), and deployment (OmniCloud) through event-driven architecture.

---

## 🏗️ The Omni Stack

A modular ecosystem where each component solves a specific problem, and together they form a complete platform for production AI systems. Each component is designed to work standalone or seamlessly integrate with others, giving you the flexibility to build exactly what you need.

### 🟢 Production-Ready

#### **OmniCore Agent**
**Production-Ready AI Agent Framework** — Build autonomous AI agents that think, reason, and execute complex tasks.

OmniCore Agent is a powerful Python framework for building autonomous AI agents that go beyond chatbots—agents that use tools, manage memory, coordinate workflows, and handle real-world business logic. Created by Abiola Adeshina, it provides sophisticated yet intuitive architecture for production AI systems.

**Core Capabilities:**

- **🌐 Universal Model Support** — Model-agnostic by design through LiteLLM integration. Use OpenAI, Anthropic Claude, Google Gemini, Ollama, or any LLM provider. Switch models without changing agent code.

- **🧠 Intelligent Routing & Orchestration** — Four powerful orchestration patterns:
  - **MemoryRouter & EventRouter** — Route queries to specialized sub-agents based on context
  - **SequentialAgent** — Chain agents for step-by-step workflows
  - **ParallelAgent** — Execute multiple agents concurrently
  - **RouterAgent** — LLM-powered intelligent task routing

- **🔧 Native Tool Integration** — **MCP (Model Context Protocol)** support for standardized interfaces with file systems, databases, APIs, and external services. **Local Tools System** lets you register any Python function as an AI tool using simple decorators.

- **💾 Production-Grade Memory** — Multi-tier memory architecture supporting in-memory, Redis, PostgreSQL, MySQL, SQLite, and MongoDB backends. Includes conversation history, vector database integration (Qdrant, ChromaDB, MongoDB Atlas), sliding window strategies, and cross-session persistence.

- **⏰ Autonomous Background Agents** — Run agents independently with intelligent scheduling (cron expressions, interval-based triggers), complete lifecycle management, and self-flying agents that run without human intervention.

- **⚡ Real-Time Streaming** — Built for modern UX with streaming responses out of the box. Users see AI thinking in real-time, making applications feel responsive and interactive.

**What Sets It Apart:**
- **True Autonomy** — Agents plan multi-step workflows, use tools to gather information, validate results, and adapt their approach
- **Composable Architecture** — Build small, focused agents and compose them into sophisticated systems
- **Full Control** — Create custom tools, define specialized routing logic, integrate any external service
- **Actually Production-Ready** — Proper error handling, retry logic, session management, and observability

**→ [Learn More](https://github.com/omnirexflora-labs/omnicoreagent)**

---

Here is the **fully updated, clean, production-ready Markdown section** — replacing **"In Development"** with a strong, accurate phase: **🚀 Public Beta**.

This version is polished for a README, consistent, and positions OmniDaemon exactly where it belongs: **deployed, production-ready, fast-evolving, and stable enough for real systems.**

---

### 🧪 Public Beta


#### **OmniDaemon**

**Universal Event-Driven Runtime Engine for AI Agents** — Transform AI agents into event-driven, scalable, autonomous systems.

OmniDaemon is a production-ready (but fast-evolving) runtime engine that provides the execution fabric enabling AI agents to listen, react, and process tasks asynchronously across distributed environments. Think of it as the operating system for AI agents—handling orchestration, persistence, messaging, and coordination so your agents can focus on intelligence, not infrastructure.

---

### **Key Features**

* **🔌 Framework-Agnostic Architecture**
  Works with any AI agent framework: OmniCoreAgent, Google ADK, LangGraph, CrewAI, AutoGen, or even plain Python functions. Your agent code stays the same—OmniDaemon provides the event-driven runtime beneath it.

* **📡 Redis Streams Event Bus**
  Built on Redis Streams for durable messaging, consumer groups, automatic load balancing, and replay support. Enterprise-grade reliability with minimal operational overhead.

* **⚖️ Intelligent Consumer Groups**
  Each agent registers under its own consumer group, enabling automatic horizontal scaling across multiple instances. Run one agent or a hundred—Redis guarantees coordinated, exactly-once message handling.

* **📊 Built-In Observability**
  CLI, REST API, and real-time metrics for deep visibility into agent health, task processing, stream backlog, dead-letter queues, and system throughput.

* **🗄️ Pluggable Storage Backend**
  Supports Redis and JSON today, with an extensible architecture designed for PostgreSQL, MongoDB, and more. Includes automatic TTL and retention management.

---

### **The Benefits**

* **Event-Driven by Design**
  Agents react instantly to business events (CRM updates, file uploads, scheduled triggers, webhooks) — no polling, no busy loops.

* **Effortless Horizontal Scaling**
  Start more agent runner processes and scaling just happens. No service meshes or load balancers needed.

* **Developer Experience First**
  Register an agent with a few lines; the SDK handles event bus connections, message parsing, retries, errors, metrics, and lifecycle management.

* **Production-Grade Reliability**
  Automatic message reclaiming, dead-letter queues, reconnection handling, graceful shutdowns, and guaranteed processing semantics.

---

### **Perfect For**

Enterprise AI automation, distributed multi-agent systems, event-driven architectures, microservices with AI components, background AI processing, and intelligent workflow automation.

**→ [Learn More](https://github.com/omnirexflora-labs/OmniDaemon)**

---

### 🚧 In Development

#### **OmniMemory**

**Persistent, context-aware memory backend for All Ai Agent** — Now under active development.

OmniMemory provides both short-term and long-term memory for ai agents, supports hybrid retrieval (vector + keyword + metadata), and enables persistent reasoning across distributed agent ecosystems.
it is ai agent framwork agnostic

**Key Capabilities:**

* Plugs into OmniCore Agent as its memory system
* Cross-session memory persistence
* Semantic search and retrieval
* Context compression and optimization
* Multi-tenant memory isolation
* Vector database integration (Qdrant, ChromaDB, MongoDB Atlas)
* Multiple backends: Redis, PostgreSQL, MongoDB, SQLite, in-memory

**Powered by SECMSA (Self-Evolving Composite Memory Synthesis Architecture)**
OmniMemory leverages SECMSA to implement:

* Parallel dual-agent memory construction (Episodic + Summarizer)
* Canonical memory synthesis with fuzzy deduplication
* Composite multi-dimensional scoring (`relevance × (1 + recency + importance)`)
* Deterministic conflict resolution (MERGE | DESTROY | NOOP | ADD)
* Ephemeral link generation for graph-like relationships without persistent graphs
* Append-only provenance for perfect causal reconstruction
* Asynchronous processing via Celery for low latency

**Use Cases:** Multi-agent systems, long-context workflows, intelligent automation, enterprise RAG pipelines, and persistent agent memory.

---


#### **OmniCloud**
**Scalable deployment and control layer** for distributed AI workloads.

- **Deploys OmniCore Agent** and **OmniDaemon** to cloud infrastructure
- Multi-cloud deployment (AWS, Azure, GCP)
- Auto-scaling and resource management
- Infrastructure as code
- Cost optimization and monitoring
- High availability and disaster recovery

**→ Coming Soon**

---

## 🚀 Why The Omni Stack?

### **Event-Driven by Design**

Unlike request-response systems, Omni Stack enables true asynchronous, reactive AI. Agents respond to business events—CRM updates, file uploads, scheduled triggers, webhook notifications—without polling or constant API requests. Build systems where AI reacts to your business, not the other way around.

### **Modular & Composable**

Use what you need. Start with OmniCore Agent (with OmniMemory for memory), plug it into OmniDaemon for event-driven runtime, and deploy both via OmniCloud. Each component works standalone or together in a complete stack. Build complex systems from simple, focused agents.

### **Production-Grade from Day One**

Built for real applications, not experiments. Proper error handling, retry logic, observability, graceful shutdowns, and failure recovery. Deploy with confidence knowing agents handle edge cases gracefully. **Already powering production systems** like [Santry Technology](https://www.linkedin.com/company/santry/).

### **Framework Agnostic**

Works with any AI framework—OmniCore Agent, Google ADK, LangGraph, CrewAI, AutoGen, or plain Python. Your agent code stays the same; we provide the infrastructure. Switch frameworks, add new agents, or run multiple types simultaneously without architectural changes.

### **Resource Efficient**

Start with 1 vCPU and 1GB RAM. OmniDaemon is optimized for I/O-bound AI workloads (the most common type), making it affordable to run sophisticated agent systems without expensive infrastructure. Scale vertically by adding consumers, horizontally by adding instances—only when you actually need it.

### **Open Source & Community-Driven**

Free, open, and built by developers who understand production needs. Active development, comprehensive documentation, and a growing ecosystem. Created by developers who understand real-world production needs.

### **Quick Comparison**

| Feature | Traditional AI | Omni Stack |
|---------|----------------|------------|
| **Architecture** | Request-response | Event-driven |
| **Scaling** | Manual configuration | Automatic load balancing |
| **Memory** | Session-only | Cross-session, semantic persistence |
| **Deployment** | Custom infrastructure | One-command deployment (OmniCloud) |
| **Framework Lock-in** | Yes | No — works with any framework |
| **Production Ready** | Requires custom work | Built-in from day one |

---

## 📊 Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                   OmniRexflora Labs Stack                    │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌──────────────┐   ┌──────────────┐   ┌──────────────┐     │
│  │  OmniCloud   │   │  OmniDaemon  │   │  OmniCore    │     │
│  │ (Deployment) │──▶│ (Event Runtime)│▶│   Agent      │     │
│  └──────────────┘   └──────┬───────┘   └──────┬───────┘     │
│                             │                 │             │
│                    ┌────────▼─────────────────▼──────┐      │
│                    │           OmniMemory            │      │
│                    │        (Memory Backend)         │      │
│                    │ Redis • PostgreSQL • MongoDB    │      │
│                    │     • Vector DB integrations    │      │
│                    └─────────────────────────────────┘      │
│                                                             │
│  Event-Driven • Distributed • Production-Ready              │
└─────────────────────────────────────────────────────────────┘
```

**How Components Work Together:**

1. **OmniMemory** provides persistent, semantic memory to **OmniCore Agent**
2. **OmniCore Agent** registers with **OmniDaemon** to process events and orchestrate workflows
3. **OmniDaemon** manages messaging, retries, DLQs, metrics, and scaling
4. **OmniCloud** deploys and governs OmniCore Agent and OmniDaemon across clouds

**In Practice:**
- Your OmniCore Agent uses OmniMemory for cross-session context and retrieval
- OmniDaemon feeds events (CRM updates, file uploads, scheduled jobs) to your agents
- OmniCloud provisions the infrastructure, autoscaling, and observability needed for production

---

## 🎓 Getting Started

### **Option 1: Start with OmniCore Agent (Recommended)**

Build your first autonomous AI agent in minutes:

```bash
# Install
uv add omnicoreagent

# Create your agent
from omnicoreagent import OmniAgent, MemoryRouter

agent = OmniAgent(
    model="gpt-4",
    tools=[file_system_tool, database_tool],
    memory_router=MemoryRouter()
)

# Run
response = await agent.run("Analyze sales data and generate report")
```

**What You Get:**
- Universal model support (switch providers without code changes)
- Intelligent routing across specialized sub-agents
- Native MCP tool integration
- Production-grade memory with multiple backends
- Real-time streaming responses and background scheduling

**→ [OmniCore Agent Documentation](https://github.com/omnirexflora-labs/omnicoreagent)**

---

### **Option 2: Add the Event-Driven Runtime (OmniDaemon)**

Transform your OmniCore Agent into an event-driven system:

```bash
# Install
uv add omnidaemon

from omnicoreagent import OmniAgent
from omnidaemon import OmniDaemonSDK, AgentConfig

agent = OmniAgent(...)

sdk = OmniDaemonSDK()
sdk.register_agent(
    AgentConfig(name="file_agent", topic="file.tasks"),
    callback=lambda msg: agent.run(msg["content"])
)

sdk.start()  # OmniCore Agent now reacts to events automatically!
```

**What You Get:**
- Redis Streams event bus with guaranteed delivery
- Automatic load balancing and consumer group management
- Dead letter queues, retries, and health-aware monitoring
- Unified CLI + API for observability and control

**→ [OmniDaemon Documentation](https://github.com/omnirexflora-labs/OmniDaemon)**

---

### **Option 3: Full Stack (Coming Soon)**

Use OmniMemory for persistent context, run agents through OmniDaemon, and deploy everything via OmniCloud.

```bash
# Coming soon — full-stack deployment guide
```

**→ [Architecture Guide](docs/architecture.md)**

---

## 🌟 Use Cases

### **Enterprise AI Automation**
- Multi-agent workflows for business processes
- Event-driven customer service systems
- Intelligent document processing pipelines
- Automated data analysis and reporting
- Real-time business event response systems

### **Developer Tools**
- AI-powered development assistants
- Code analysis and refactoring agents
- Automated testing and deployment
- Intelligent debugging and troubleshooting
- Background AI processing for CI/CD pipelines

### **Intelligent Applications**
- Autonomous research assistants
- Context-aware personal assistants
- Multi-modal AI systems
- Long-running agent workflows
- Food waste reduction systems (like [Santry Technology](https://www.linkedin.com/company/santry/))

### **Production Deployments**
- **Santry Technology** — Using OmniCore Agent in production to reduce household food waste globally through intelligent food management

---

## 🏆 Production Showcase

### **Santry Technology**
**Reducing household food waste globally** — Proudly based in Hong Kong

[Santry Technology](https://www.linkedin.com/company/santry/) is using **OmniCore Agent** in production to power their intelligent food management mobile app. Their system combines AI, cloud technologies, and user-centric design to help consumers track expiry dates, minimize waste, and discover recipes from what they already have.

**What Santry Built:**
- AI-powered food tracking and expiry date management
- Intelligent recipe suggestions based on available ingredients
- Waste reduction through proactive notifications
- Production-grade AI agent system handling real user workflows

*Building a smarter, more sustainable way to manage food globally—powered by OmniCore Agent.*

---

## 🛠️ Technology Stack

- **Language**: Python 3.10+
- **Event Bus**: Redis Streams (pluggable: Kafka, RabbitMQ)
- **Storage**: Redis, PostgreSQL, MongoDB (pluggable)
- **AI Models**: OpenAI, Anthropic, Google, Local (via LiteLLM)
- **Deployment**: Docker, Kubernetes, Cloud-native
- **Architecture**: Event-driven, Microservices, Distributed

---

## 🤝 Contributing

We believe in open source and community-driven development. Contributions are welcome!

- **Code**: Submit PRs, fix bugs, add features
- **Documentation**: Improve guides, add examples
- **Testing**: Write tests, report issues
- **Community**: Share use cases, provide feedback

**→ [Contributing Guide](CONTRIBUTING.md)**

---

## 📚 Documentation

- **[OmniCore Agent Docs](https://github.com/omnirexflora-labs/omnicoreagent)**
- **[OmniDaemon Docs](https://github.com/omnirexflora-labs/OmniDaemon)**
- **[Architecture Guide](docs/architecture.md)**
- **[Best Practices](docs/best-practices.md)**

---

## 🗺️ Roadmap

### **Current Status (2025)**
- ✅ **OmniCore Agent v0.2.10** — Production-ready, powering [Santry Technology](https://www.linkedin.com/company/santry/)
- ✅ **OmniDaemon v0.0.1** — Beta, active development with Redis Streams runtime
- 🚧 **OmniMemory v0.0.1** — Alpha, planned for Q4 2025
- 📋 **OmniCloud v0.1** — Development kicks off Q1 2026

### **2026 Roadmap**
- 🚧 Enhanced multi-agent orchestration and coordination patterns
- 🚧 Advanced memory compression, summarization, and retrieval tooling
- 🚧 Enterprise features (SSO, audit logs, advanced monitoring dashboards)
- 🚧 Additional event bus backends (Kafka, RabbitMQ, NATS JetStream)
- 🚧 Cloud-native deployment templates and operators for Kubernetes and serverless

---

## 👨‍💻 About the Creator

**Abiola Adeshina** — A software engineer from Lagos, Nigeria, building open-source AI infrastructure.

I believe in creating tools that empower developers worldwide. The Omni Stack is built from real production needs—solving problems I've faced building AI systems at scale. Open source isn't just a license; it's a philosophy that great software should be accessible to everyone, regardless of location or resources.

From Africa to the world, building the future of AI infrastructure, one commit at a time.

**Connect:**
- **GitHub**: [@Abiorh001](https://github.com/Abiorh001)
- **X (Twitter)**: [@abiorhmangana](https://x.com/abiorhmangana)
- **LinkedIn**: [Abiola Adeshina](https://www.linkedin.com/in/abiola-a-06b66a1a4/)

---

## 📄 License

All OmniRexflora Labs projects are released under the **MIT License** — free for commercial and personal use.

---

## 🌍 Mission Statement

**To make production-grade AI agent infrastructure accessible to every developer, everywhere.**

We're building the tools that will power the next generation of autonomous AI systems. By making our infrastructure open source, modular, and production-ready, we're enabling developers to focus on intelligence, not infrastructure.

**The future of AI is event-driven, distributed, and autonomous. We're building that future, together.**

---

## ⭐ Star Us on GitHub

If you find our work valuable, please star our repositories:

- ⭐ [OmniCore Agent](https://github.com/omnirexflora-labs/omnicoreagent)
- ⭐ [OmniDaemon](https://github.com/omnirexflora-labs/OmniDaemon)

Your support helps us continue building open-source AI infrastructure.

---

## 📬 Get Involved

- **Discussions**: [GitHub Discussions](https://github.com/OmniRexflora/discussions)
- **Issues**: [Report Bugs](https://github.com/OmniRexflora/issues)
- **Features**: [Request Features](https://github.com/OmniRexflora/issues)
- **Community**: Join our growing developer community

---

<div align="center">

**Created by [Abiola Adeshina](https://github.com/Abiorh001) and the OmniRexflora Labs Community**

*From Lagos, Nigeria to the world — building the infrastructure for autonomous AI*

[⭐ Star Us](https://github.com/omnirexflora-labs) · [📖 Documentation](https://github.com/omnirexflora-labs) · [🐛 Report Bug](https://github.com/omnirexflora-labs/issues) · [💡 Request Feature](https://github.com/omnirexflora-labs/issues)

</div>

