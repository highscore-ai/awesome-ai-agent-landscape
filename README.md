# Awesome AI Agent Landscape

A living map of how the major AI ecosystems evolve:

> **Foundation Model → AI Assistant → Developer Agent → General Work Agent**

[![Curated by HighScore](https://img.shields.io/badge/curated%20by-HighScore.ai-111827?style=flat-square)](https://highscore.ai)
[![Map updated](https://img.shields.io/badge/map%20updated-2026--08--25-2563eb?style=flat-square)](data/landscape.yml)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-16a34a?style=flat-square)](CONTRIBUTING.md)

<p align="center">
  <img src="assets/ai-agent-evolving-map.svg" alt="AI Agent Evolving: Foundation Model to General Work Agent" width="100%">
</p>

The industry is not simply releasing better chatbots. Each major ecosystem is extending the same arc: first intelligence, then conversation, then agents that can build, and finally agents that can own longer-running work.

This repository tracks that evolution in one comparable map. It is a **product-positioning landscape**, not a generic directory of agent frameworks.

## The map

| Ecosystem | Foundation Model<br><sub>The intelligence</sub> | AI Assistant<br><sub>Talk to AI</sub> | Developer Agent<br><sub>Engineer with AI</sub> | General Work Agent<br><sub>Get work done with AI</sub> |
|---|---|---|---|---|
| **OpenAI**<br><sub>Broad general intelligence & leading developer tools</sub> | [GPT](https://openai.com/) <br><sub>GPT-5.6 family</sub> | [ChatGPT](https://chatgpt.com/) <br><sub>AI assistant</sub> | [Codex](https://openai.com/codex/) <br><sub>Developer agent for software</sub> | [ChatGPT Work](https://chatgpt.com/) <br><sub>Longer tasks & deliverables</sub> |
| **Anthropic**<br><sub>AI safety pioneers & agent-harness leaders</sub> | [Claude](https://www.anthropic.com/claude) <br><sub>Claude 4 family</sub> | [Claude](https://claude.ai/) <br><sub>AI assistant</sub> | [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) <br><sub>Developer agent for codebases</sub> | [Claude Cowork](https://claude.ai/) <br><sub>General work agent for teams & projects</sub> |
| **Google**<br><sub>AI + data + cloud advantage</sub> | [Gemini](https://gemini.google.com/) <br><sub>Gemini 2.5 family</sub> | [Gemini + Search](https://gemini.google.com/) <br><sub>Assistant with real-time search</sub> | Antigravity <br><sub>Developer agent platform</sub> | Gemini Spark <br><sub>General work agent, 24/7 execution</sub> |
| **xAI**<br><sub>Built for the era of agents</sub> | [Grok](https://grok.com/) <br><sub>Grok 3 family</sub> | [Grok](https://grok.com/) <br><sub>AI assistant</sub> | Grok Build <br><sub>Developer agent for complex builds</sub> | Grok Bot <br><sub>Autonomous agent with its own computer</sub> |
| **Open Source**<br><sub>Open models, open freedom</sub> | [DeepSeek](https://github.com/deepseek-ai/DeepSeek-R1) <br><sub>DeepSeek R1 family</sub> | [Open WebUI](https://github.com/open-webui/open-webui) <br><sub>Open-source AI interface</sub> | [OpenHands](https://github.com/All-Hands-AI/OpenHands) <br><sub>Open-source developer agent</sub> | [OpenClaw](https://github.com/openclaw/openclaw) <br><sub>Open-source general work agent</sub> |

## What this repository tracks

Each cell is a maintained product record in [data/landscape.yml](data/landscape.yml), with:

- the ecosystem and stage in the evolution;
- the named product or product family;
- a primary source, when one is available;
- current status: **active**, **tracking**, **renamed**, **retired**, or **unverified**;
- a short note explaining why it occupies that position.

A blank or unverified entry is useful information: it means the market has not yet produced a clear public product for that role, or its status is still being validated. We will not fill gaps merely to make the grid look complete.

## How to read the stages

| Stage | It mainly does | Typical user relationship |
|---|---|---|
| **Foundation Model** | Provides reasoning, language, vision, code, and other raw intelligence | You or an application call the model |
| **AI Assistant** | Responds interactively and helps with individual tasks | You drive the conversation |
| **Developer Agent** | Reads codebases, uses tools, makes changes, and verifies work | You delegate engineering tasks |
| **General Work Agent** | Runs longer tasks across files, apps, research, and deliverables | You assign an outcome and supervise |

These are product roles, not strict technical boundaries. A strong assistant can use tools; a developer agent is also an assistant. The useful question is **what job the product is designed to own**.

## Update policy

We update the map when a major ecosystem makes a meaningful move across one of the four stages:

- a new model family materially changes the foundation;
- an assistant gains persistent tools, memory, or real-time grounding;
- a coding product becomes an autonomous developer agent;
- a product can carry out longer-running, cross-application work with meaningful autonomy;
- an entry is renamed, discontinued, or its public availability changes.

The aim is to capture the strategic shift, not every feature launch.

## Contributing

If you spot a change, open a [landscape update issue](../../issues/new?template=landscape-entry.md). Please include the product, ecosystem, stage, official source, and what changed.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the editorial rules.

## Related HighScore projects

- [Awesome Free HighScore AI Learning Resources](https://github.com/highscore-ai/awesome-free-ai-learning-courses) — learn the capabilities behind this landscape.
- [HighScore.ai](https://highscore.ai) — choose a role, map skills, discover resources, follow a path, and apply them to work.

## License

The original curation, data, and visual are released under the [AGPL-3.0 License](LICENSE). Linked third-party products remain subject to their own licenses and terms.
