# Awesome AI Agent Landscape

A focused, vendor-first map of the fast-moving AI agent ecosystem.

> **The question this project answers:** *What exists, what layer does it belong to, and when should I use it?*

[![Curated by HighScore](https://img.shields.io/badge/curated%20by-HighScore.ai-111827?style=flat-square)](https://highscore.ai)
[![Last review](https://img.shields.io/badge/last%20reviewed-2026--08--25-2563eb?style=flat-square)](#update-policy)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-16a34a?style=flat-square)](CONTRIBUTING.md)

<p align="left">
  <img src="https://raw.githubusercontent.com/highscore-ai/awesome-free-ai-learning-courses/main/assets/high-score-banner.png" alt="HighScore" width="260">
</p>

Unlike broad “AI tools” directories, this repository concentrates on the products and open-source projects that define **how agents are built, run, connected, evaluated, and deployed**. It is designed to help builders and technical decision-makers separate the core platforms from the surrounding noise.

The catalogue is maintained in [data/landscape.yml](data/landscape.yml). The README is the human-friendly view.

## Start here

| If you want to… | Begin with |
|---|---|
| Build a production agent around a frontier model | [Agent platforms](#1-agent-platforms) |
| Delegate coding tasks to an autonomous tool | [Coding agents & harnesses](#2-coding-agents--harnesses) |
| Orchestrate workflows, state, or multi-agent systems | [Frameworks](#3-frameworks--orchestration) |
| Give agents safe tools, browsers, or isolated execution | [Runtimes & tool execution](#4-runtimes--tool-execution) |
| Connect agents to tools or to other agents | [Protocols & interoperability](#5-protocols--interoperability) |
| Trace, test, and improve agent behavior | [Evaluation & observability](#6-evaluation--observability) |
| Ship an internal workflow without building everything from scratch | [Visual & low-code builders](#7-visual--low-code-builders) |

## The landscape at a glance

~~~mermaid
flowchart TD
  P["Model / Agent platform"] --> F["Framework & orchestration"]
  F --> R["Runtime & tools"]
  R --> U["User or business workflow"]
  F -.observe and evaluate.-> E["Evaluation & observability"]
  R <-.connect.-> I["Protocols & interoperability"]
~~~

A product can appear in more than one place, but its **primary layer** determines where it is listed. This avoids treating every project that calls an LLM as a separate “agent platform.”

## Contents

- [1. Agent platforms](#1-agent-platforms)
- [2. Coding agents & harnesses](#2-coding-agents--harnesses)
- [3. Frameworks & orchestration](#3-frameworks--orchestration)
- [4. Runtimes & tool execution](#4-runtimes--tool-execution)
- [5. Protocols & interoperability](#5-protocols--interoperability)
- [6. Evaluation & observability](#6-evaluation--observability)
- [7. Visual & low-code builders](#7-visual--low-code-builders)
- [8. Benchmarks & research environments](#8-benchmarks--research-environments)
- [How to read the catalogue](#how-to-read-the-catalogue)
- [Update policy](#update-policy)
- [Contributing](#contributing)

---

## 1. Agent platforms

Managed or model-native foundations for building and operating agents. These are the most useful starting points when you are aligned to a specific model provider or enterprise cloud.

| Platform | Primary fit | Open source | Notes |
|---|---|:---:|---|
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | Tool-using agents, handoffs, traces | Yes | Provider-native SDK; pairs with the Responses API. |
| [Anthropic Claude Agent SDK](https://docs.anthropic.com/en/docs/claude-code/sdk) | Claude-powered coding and task agents | Partial | Agent capabilities built around Claude Code’s agent loop. |
| [Google Agent Development Kit (ADK)](https://github.com/google/adk-python) | Multi-agent applications on Gemini / Google Cloud | Yes | Code-first framework with Google Cloud deployment paths. |
| [Microsoft Azure AI Foundry Agent Service](https://learn.microsoft.com/azure/ai-foundry/agents/) | Governed enterprise agents on Azure | No | Managed service with identity, tools, and enterprise integrations. |
| [Amazon Bedrock Agents](https://aws.amazon.com/bedrock/agents/) | AWS-native task automation | No | Managed agents integrated with AWS services and knowledge bases. |
| [NVIDIA NeMo Agent Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) | Enterprise agent systems and optimization | Yes | Modular toolkit with strong NVIDIA ecosystem integration. |
| [IBM watsonx Orchestrate](https://www.ibm.com/products/watsonx-orchestrate) | Enterprise work automation | No | Business process and enterprise application focus. |

[Back to top](#awesome-ai-agent-landscape)

---

## 2. Coding agents & harnesses

Agentic developer tools that plan, edit, execute, and verify work inside a codebase. A **harness** is the environment and control loop around the model—not just the model itself.

| Project | Surface | Best for | Open source |
|---|---|---|:---:|
| [Codex CLI](https://github.com/openai/codex) | Terminal / agent harness | OpenAI-native coding workflows | Yes |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) | Terminal / IDE | Deep repository work with Claude | No |
| [Gemini CLI](https://github.com/google-gemini/gemini-cli) | Terminal | Gemini-native command-line coding | Yes |
| [OpenCode](https://github.com/anomalyco/opencode) | Terminal / desktop | Model-flexible open coding agent | Yes |
| [Cline](https://github.com/cline/cline) | VS Code | Tool-rich, user-steered IDE agent | Yes |
| [Aider](https://github.com/Aider-AI/aider) | Terminal | Git-aware pair programming with many models | Yes |
| [Continue](https://github.com/continuedev/continue) | IDE | Open-source coding assistant platform | Yes |
| [SWE-agent](https://github.com/SWE-agent/SWE-agent) | Python framework | Software-engineering issue resolution research | Yes |

[Back to top](#awesome-ai-agent-landscape)

---

## 3. Frameworks & orchestration

Frameworks for defining agent state, tool use, retrieval, routing, and multi-agent workflows. Choose the smallest abstraction that gives you the reliability you need.

| Framework | Core idea | Strong fit | Language |
|---|---|---|---|
| [LangGraph](https://github.com/langchain-ai/langgraph) | Stateful graph workflows | Durable, controllable agent loops | Python / JS |
| [LangChain](https://github.com/langchain-ai/langchain) | Application and integration framework | Broad model/tool ecosystem | Python / JS |
| [LlamaIndex](https://github.com/run-llama/llama_index) | Data and knowledge agents | RAG, data connectors, knowledge work | Python / TS |
| [PydanticAI](https://github.com/pydantic/pydantic-ai) | Type-safe agent applications | Python teams that value schemas and validation | Python |
| [CrewAI](https://github.com/crewAIInc/crewAI) | Role-based multi-agent flows | Clear task delegation patterns | Python |
| [Microsoft AutoGen](https://github.com/microsoft/autogen) | Conversational multi-agent systems | Research and enterprise prototypes | Python / .NET |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | AI orchestration SDK | Microsoft-stack applications | C# / Python / Java |
| [Agno](https://github.com/agno-agi/agno) | Lightweight agent runtime | Fast code-first agent delivery | Python |
| [Mastra](https://github.com/mastra-ai/mastra) | TypeScript agent framework | Full-stack JavaScript teams | TypeScript |
| [Hugging Face smolagents](https://github.com/huggingface/smolagents) | Minimal, code-first agents | Compact experimental agents | Python |
| [Haystack](https://github.com/deepset-ai/haystack) | Production NLP / RAG pipelines | Search and retrieval-heavy applications | Python |

[Back to top](#awesome-ai-agent-landscape)

---

## 4. Runtimes & tool execution

Agents become useful only when they can safely act. This layer provides browser control, sandboxes, computer use, credentials boundaries, and execution environments.

| Project | Provides | Typical use |
|---|---|---|
| [Browser Use](https://github.com/browser-use/browser-use) | Browser automation for agents | Website research and browser task execution |
| [Playwright](https://github.com/microsoft/playwright) | Browser automation primitives | Reliable browser tools inside a custom agent |
| [E2B](https://github.com/e2b-dev/E2B) | Isolated cloud sandboxes | Secure code execution and data work |
| [Daytona](https://github.com/daytonaio/daytona) | Development environments and sandboxes | Long-lived agent workspaces |
| [Modal Sandboxes](https://modal.com/docs/guide/sandbox) | Managed compute sandboxes | Programmatic execution at scale |
| [Docker](https://www.docker.com/) | Local container isolation | Self-hosted execution boundaries |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | Software-agent runtime | Open, end-to-end coding-agent workflows |

[Back to top](#awesome-ai-agent-landscape)

---

## 5. Protocols & interoperability

Standards and open interfaces that make agents portable, connectable, and less dependent on one vendor’s tool format.

| Protocol / project | Connects | Why it matters |
|---|---|---|
| [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) | AI applications ↔ tools, data, and prompts | The emerging standard interface for exposing agent tools and context. |
| [Agent2Agent (A2A)](https://github.com/google/A2A) | Agent ↔ agent | Lets independently built agents communicate and delegate work. |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) | Agent backends ↔ interactive frontends | Standardizes real-time, agentic user interfaces. |
| [OpenAPI](https://www.openapis.org/) | Software ↔ software | Widely used API contract often adapted into agent tools. |
| [JSON Schema](https://json-schema.org/) | Models ↔ structured tool inputs / outputs | A foundational contract for reliable structured actions. |

[Back to top](#awesome-ai-agent-landscape)

---

## 6. Evaluation & observability

An agent is not production-ready because it completes one demo. This layer makes behavior inspectable, testable, comparable, and improvable.

| Project | Primary capability | Deployment |
|---|---|---|
| [LangSmith](https://www.langchain.com/langsmith) | Tracing, evaluation, prompt and dataset management | Hosted |
| [Langfuse](https://github.com/langfuse/langfuse) | Open-source observability and evaluation | Self-hosted / cloud |
| [Arize Phoenix](https://github.com/Arize-ai/phoenix) | Open-source tracing and LLM evaluation | Self-hosted |
| [Braintrust](https://www.braintrust.dev/) | Evals, logging, and scoring | Hosted |
| [Weights & Biases Weave](https://github.com/wandb/weave) | Traces, evaluations, and experiment tracking | Open source / cloud |
| [MLflow](https://github.com/mlflow/mlflow) | Experiment tracking and AI lifecycle | Open source |
| [Ragas](https://github.com/explodinggradients/ragas) | RAG and agent evaluation metrics | Open source |
| [DeepEval](https://github.com/confident-ai/deepeval) | LLM and agent test framework | Open source |
| [Promptfoo](https://github.com/promptfoo/promptfoo) | Test, red-team, and compare LLM applications | Open source |

[Back to top](#awesome-ai-agent-landscape)

---

## 7. Visual & low-code builders

These products remove much of the boilerplate for teams that need to assemble, test, and ship agentic workflows quickly.

| Project | Primary fit | Open source |
|---|---|:---:|
| [n8n](https://github.com/n8n-io/n8n) | Automation workflows with AI steps | Source available |
| [Dify](https://github.com/langgenius/dify) | Production AI apps and workflow agents | Yes |
| [Flowise](https://github.com/FlowiseAI/Flowise) | Visual LLM and agent flows | Yes |
| [Langflow](https://github.com/langflow-ai/langflow) | Visual LangChain-style workflows | Yes |
| [Microsoft Copilot Studio](https://www.microsoft.com/microsoft-copilot/microsoft-copilot-studio) | Enterprise copilots and business automation | No |
| [Google Vertex AI Agent Builder](https://cloud.google.com/products/agent-builder) | Google Cloud enterprise agents | No |
| [Zapier Agents](https://zapier.com/agents) | SaaS workflow automation | No |

[Back to top](#awesome-ai-agent-landscape)

---

## 8. Benchmarks & research environments

Benchmarks help distinguish an impressive agent demo from a system that actually performs well under comparable conditions.

| Benchmark / environment | Measures |
|---|---|
| [SWE-bench](https://github.com/SWE-bench/SWE-bench) | Real-world GitHub issue resolution |
| [GAIA](https://huggingface.co/gaia-benchmark) | General assistant reasoning and tool use |
| [AgentBench](https://github.com/THUDM/AgentBench) | Agent behavior across multiple environments |
| [WebArena](https://github.com/web-arena-x/webarena) | Web-agent task completion in realistic sites |
| [OSWorld](https://github.com/xlang-ai/OSWorld) | Computer-use agents in operating-system tasks |
| [BrowseComp](https://openai.com/index/browsecomp/) | Web browsing and information-seeking ability |

[Back to top](#awesome-ai-agent-landscape)

---

## How to read the catalogue

- **Vendor-first:** official platforms come before third-party abstractions. Start with the platform you already use, then add a framework only when it solves a real control or portability problem.
- **Layered, not ranked:** this is a map, not a “top 100.” A tool may be excellent and still be the wrong layer for your problem.
- **Open source is specific:** “open source,” “source available,” and “hosted only” are deliberately distinct. Always verify the project’s current license and terms.
- **Links point to primary sources:** project repositories and official documentation are preferred over listicles or affiliate pages.

## Update policy

This ecosystem changes weekly. Entries are reviewed when one of these changes:

- a major platform or project launches, is renamed, archived, or materially changes direction;
- a project gains a production agent capability, protocol support, or an open-source release;
- a benchmark, evaluation result, or license change alters how the project should be understood.

Each entry should have a stable primary link and a clear reason for appearing here. We avoid duplicate entries, funding announcements, prompt packs, and short-lived “wrapper” products.

## Contributing

Additions and corrections are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md), then open an issue using the submission template. A good submission explains **which layer** the project belongs to and **why it is durable enough to map**.

## Related HighScore projects

- [Awesome Free HighScore AI Learning Resources](https://github.com/highscore-ai/awesome-free-ai-learning-courses) — free learning resources for the skills behind the landscape.
- [HighScore.ai](https://highscore.ai) — choose a role, map capabilities, discover learning resources, follow a path, and apply them to work.

## License

The original curation and repository content are released under the [AGPL-3.0 License](LICENSE). Linked third-party projects remain subject to their own licenses and terms.
