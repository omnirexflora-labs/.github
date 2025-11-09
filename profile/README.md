# OmniRexflora Labs

> **Building the infrastructure layer for autonomous AI systems**

[![GitHub](https://img.shields.io/badge/GitHub-Organization-black?style=flat-square&logo=github)](https://github.com/omnirexflora-labs/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![Open Source](https://img.shields.io/badge/Open%20Source-Yes-green?style=flat-square)](https://opensource.org)
[![Production](https://img.shields.io/badge/Production-Ready-success?style=flat-square)](https://www.linkedin.com/company/santry/)
[![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)](https://www.python.org/)

---

## ✨ Key Highlights

- 🚀 **Production-Ready** — OmniCore Agent v0.2.10 already powering [Santry Technology](https://www.linkedin.com/company/santry/) in production
- 🔌 **Framework-Agnostic** — Works with any AI framework (OmniCore Agent, LangGraph, CrewAI, AutoGen, or plain Python)
- ⚡ **Event-Driven** — Transform AI agents into reactive, scalable systems that respond to business events
- 📈 **Horizontal Scaling** — Scale from 1 instance to 100+ with zero configuration changes
- 🛠️ **Developer-Friendly** — Register agents with a few lines of code, SDK handles the complexity
- 💾 **Production Memory** — Multi-tier memory with Redis, PostgreSQL, MongoDB, and vector DB support
- 🔄 **Real-Time Streaming** — Built-in streaming responses for modern, interactive UX
- 🌐 **Universal Models** — Support for OpenAI, Claude, Gemini, Ollama, and any LLM via LiteLLM

---

## 🌍 The Vision

**Making AI agent development as modular and composable as today's cloud systems.**

Modern AI systems need more than chat interfaces—they require multi-agent coordination, autonomous event responses, persistent memory, and cloud-scale orchestration. The Omni Stack delivers this using **event-driven architecture**, the same pattern powering Netflix, Uber, and Stripe, now reimagined for AI systems.

We build **open-source AI infrastructure** that empowers developers to deploy and scale autonomous AI agents with the simplicity of modern cloud platforms. **Already powering production systems** and trusted by companies building the future of intelligent automation.

---

## 🎯 The Problem We Solve

Today's AI landscape is fragmented:

- **Frameworks** provide intelligence but lack production runtime
- **Chatbots** are reactive, not autonomous
- **Multi-agent systems** are complex to orchestrate
- **Event-driven AI** is missing from most platforms
- **Production deployment** requires custom infrastructure

**The Omni Stack bridges this gap** by providing a complete, modular ecosystem for building AI agents as **distributed systems**, not chatbots. We connect reasoning, memory, and automation through event-driven architecture.

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

### 🚧 In Development

#### **OmniDaemon**
**Universal Event-Driven Runtime Engine for AI Agents** — Transform AI agents into event-driven, scalable, autonomous systems.

OmniDaemon is a production-grade runtime engine that provides the infrastructure layer enabling AI agents to listen, react, and process tasks asynchronously across distributed environments. Think of it as the operating system for AI agents—handling orchestration, persistence, messaging, and coordination so your agents can focus on intelligence, not infrastructure.

**Key Features:**

- **🔌 Framework-Agnostic Architecture** — Works with any AI agent framework: OmniCore Agent, Google ADK, LangGraph, CrewAI, AutoGen, or even plain Python functions. Your agent code remains unchanged; OmniDaemon provides the event-driven runtime that powers it.

- **📡 Redis Streams Event Bus** — Built on Redis Streams for reliable, durable messaging with consumer groups, automatic load balancing, and message replay capabilities. Enterprise-grade reliability with minimal operational overhead.

- **⚖️ Intelligent Consumer Groups** — Each agent registers with its own consumer group, enabling automatic load distribution across multiple instances. Run one agent or a hundred—Redis coordinates work distribution and ensures every message gets handled exactly once.

- **📊 Built-in Observability** — Comprehensive monitoring through CLI commands, REST API, and real-time metrics. Track task processing, monitor agent health, inspect message streams, view dead letter queues—everything you need for production operations.

- **🗄️ Pluggable Storage Backend** — Currently supports Redis and JSON storage, with extensible architecture for PostgreSQL, MongoDB, or any database. Automatic TTL management makes data retention effortless.

**The Benefits:**
- **Event-Driven by Design** — Agents respond to business events (CRM updates, file uploads, scheduled triggers, webhook notifications) without polling or constant API requests
- **Horizontal Scaling Made Simple** — Just start another agent runner instance. No load balancers, no complex orchestration—just run more processes
- **Developer Experience** — Register your agent with a few lines of code. The SDK handles event bus connections, message parsing, error handling, retries, and metrics
- **Production Reliability** — Automatic message reclaiming, dead letter queues, graceful shutdown handling, and connection recovery

**Perfect for:** Enterprise AI automation, multi-agent systems, event-driven architectures, microservices with AI, background AI processing, intelligent workflow automation.

**→ [Learn More](https://github.com/omnirexflora-labs/OmniDaemon)**

#### **OmniCloud**
**Scalable deployment and control layer** for distributed AI workloads.

- **Deploys OmniCore Agent** and **OmniDaemon** to cloud infrastructure
- Multi-cloud deployment (AWS, Azure, GCP)
- Auto-scaling and resource management
- Infrastructure as code
- Cost optimization and monitoring
- High availability and disaster recovery

**→ Coming Soon**

#### **OmniMemory**
**Persistent, context-aware memory backend** for OmniCore Agent.

- Plugs into OmniCore Agent as its memory system
- Cross-session memory persistence
- Semantic search and retrieval
- Context compression and optimization
- Multi-tenant memory isolation
- Vector database integration (Qdrant, ChromaDB, MongoDB Atlas)
- Multiple backends: Redis, PostgreSQL, MongoDB, SQLite, in-memory

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

---

## 📊 Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                    OmniRexflora Labs Stack                   │
├─────────────────────────────────────────────────────────────┤
│                                                               │
│                    ┌──────────────────┐                      │
│                    │   OmniCloud      │                      │
│                    │  (Deployment)    │                      │
│                    └────────┬─────────┘                      │
│                             │                                 │
│                    ┌────────▼─────────┐                      │
│                    │   OmniDaemon     │                      │
│                    │  (Event Runtime)  │                      │
│                    └────────┬─────────┘                      │
│                             │                                 │
│                    ┌────────▼─────────┐                      │
│                    │ OmniCore Agent   │                      │
│                    │  (Intelligence)   │                      │
│                    └────────┬─────────┘                      │
│                             │                                 │
│                    ┌────────▼─────────┐                      │
│                    │  OmniMemory       │                      │
│                    │  (Memory Backend) │                      │
│                    └───────────────────┘                      │
│                                                               │
│  Flow: OmniMemory → OmniCore Agent → OmniDaemon → OmniCloud │
│  Event-Driven Architecture • Distributed Systems • AI Agents │
└─────────────────────────────────────────────────────────────┘
```

**How It Works:**

1. **OmniMemory** plugs into **OmniCore Agent** as its memory backend (Redis, PostgreSQL, MongoDB, or in-memory)
2. **OmniCore Agent** plugs into **OmniDaemon** as an agent that runs on the event-driven runtime
3. **OmniCore Agent** can be deployed using **OmniCloud** (deployment layer)
4. **OmniDaemon** can also be deployed using **OmniCloud** (deployment layer)

**In Practice:**
- Your OmniCore Agent uses OmniMemory for persistent context
- Your OmniCore Agent registers with OmniDaemon to process events
- Both OmniCore Agent and OmniDaemon can be deployed via OmniCloud

---

## 🎓 Getting Started

### **Start with OmniCore Agent**

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

**Key Features You Get:**
- Universal model support (switch models without code changes)
- Intelligent routing to specialized sub-agents
- Native MCP tool integration
- Production-grade memory with multiple backends
- Real-time streaming responses
- Background agent scheduling

**→ [Full Documentation](https://github.com/omnirexflora-labs/omnicoreagent)**

### **Add Event-Driven Runtime**

Transform your OmniCore Agent into an event-driven system with OmniDaemon:

```bash
# Install
uv add omnidaemon

# Your OmniCore Agent callback
from omnicoreagent import OmniAgent
from omnidaemon import OmniDaemonSDK, AgentConfig

# Initialize your OmniCore Agent
agent = OmniAgent(...)

# Register with OmniDaemon - just a few lines!
sdk = OmniDaemonSDK()
sdk.register_agent(
    AgentConfig(name="file_agent", topic="file.tasks"),
    callback=lambda msg: agent.run(msg["content"])  # OmniCore Agent runs here
)

# Start runtime - OmniCore Agent now processes events!
sdk.start()
```

**What You Get:**
- Automatic load balancing across instances
- Redis Streams event bus with guaranteed delivery
- Built-in observability and monitoring
- Dead letter queues for failed messages
- Horizontal scaling with zero configuration

**→ [Full Documentation](https://github.com/omnirexflora-labs/OmniDaemon)**

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

### **Current Status (November 2025)**
- ✅ OmniCore Agent v0.2.10 (Production - Used by [Santry Technology](https://www.linkedin.com/company/santry/))
- 📋 OmniDaemon v0.0.1 (Beta - Coming Soon)
- 📋 OmniMemory v0.1 (Alpha - December 2025)

### **2026**
- 🚧 OmniCore Agent improvements and stability
- 🚧 OmniDaemon v0.x development and enhancements
- 🚧 OmniMemory v0.x improvements and feature additions
- 📋 OmniCloud v0.1 (Alpha - Development begins)
- 📋 Enhanced multi-agent orchestration
- 📋 Advanced memory compression
- 📋 Enterprise features

---

## 👨‍💻 About the Creator

**Abiola Adeshina** — A developer from Lagos, Nigeria, building open-source AI infrastructure.

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

