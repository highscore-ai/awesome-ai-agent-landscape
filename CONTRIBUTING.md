# Contributing to the AI Agent Evolving Map

This repository tracks a specific product evolution:

**Foundation Model → AI Assistant → Developer Agent → General Work Agent**

It is not a broad directory of agent frameworks or every new AI product.

## A contribution belongs here when it changes the map

Please submit an update when a major ecosystem:

- launches or meaningfully upgrades a foundation-model family;
- introduces an assistant with a distinct product role;
- ships a developer agent that can work across code and tools;
- ships a general work agent that can complete longer-running tasks or deliverables;
- renames, retires, or materially changes one of the products already mapped.

## What to include

Open an issue with:

1. **Ecosystem** — OpenAI, Anthropic, Google, xAI, Open Source, or a proposed new ecosystem
2. **Stage** — foundation model, AI assistant, developer agent, or general work agent
3. **Product name** and **official source**
4. **Status** — active, tracking, renamed, retired, or unverified
5. **What changed** and why it moves or fills a position on the map

Use official documentation, an official announcement, or the canonical project repository. Do not use a news summary as the only source.

## Editorial rules

- The stage describes the product’s **main job**, not every capability it has.
- One ecosystem can have one representative product per stage. If several candidates exist, explain why the position should change.
- A product without a stable primary source is marked **tracking**, not presented as confirmed.
- Do not submit generic frameworks, wrappers, prompt collections, or paid courses unless they become a representative product in the four-stage evolution.
- Keep the one-line note factual and concise.

## Data source

The source of truth is [data/landscape.yml](data/landscape.yml). Update it with the same commit as the public README and visual when you make a material change.

By contributing, you agree that your contribution may be published under the repository’s AGPL-3.0 license.
