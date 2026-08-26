# Codex

[Official Codex product page](https://openai.com/codex/)

> Prices in USD. Information verified 25 August 2026.

## Plan comparison

| Plan | Price | Codex models | Included usage | After the included allowance |
|---|---:|---|---|---|
| Free | US$0 | GPT-5.6 Terra | Plan-specific 5-hour and weekly windows. OpenAI does **not** publish a fixed task, token, or credit quota. | Wait for the reset shown in **Usage**. |
| Go | Varies by country | GPT-5.6 Terra | Plan-specific 5-hour and weekly windows. No public fixed quota. | Wait for the reset shown in **Usage**. |
| Plus | US$20/month | GPT-5.6 Sol, Terra, Luna | Baseline paid individual allowance; it is shared with ChatGPT Work and ChatGPT for Excel. No public fixed quota. | Buy pay-as-you-go credits; Auto top-up is available. |
| Pro — US$100 | US$100/month | GPT-5.6 Sol, Terra, Luna; GPT-5.3-Codex-Spark preview | **5×** the Plus usage allowance. The allowance is shared with ChatGPT Work and ChatGPT for Excel. | Buy pay-as-you-go credits; Auto top-up is available. |
| Pro — US$200 | US$200/month | GPT-5.6 Sol, Terra, Luna; GPT-5.3-Codex-Spark preview | **20×** the Plus usage allowance. The allowance is shared with ChatGPT Work and ChatGPT for Excel. | Buy pay-as-you-go credits; Auto top-up is available. |
| Business — Standard | US$25/user/month, or US$20/user/month annually | GPT-5.6 Sol, Terra, Luna | Included baseline business allowance; no public fixed quota. Minimum two seats. | Workspace credit pool can extend use when enabled by an owner. |
| Business — Premium | US$125/user/month, or US$100/user/month annually | GPT-5.6 Sol, Terra, Luna | **5×** Standard-seat usage; **no 5-hour usage limit**. Minimum two seats. | Workspace credit pool can extend use when enabled by an owner. |
| Edu / Enterprise | Contract pricing | GPT-5.6 Sol, Terra, Luna | Contract and workspace-specific allowance. | Credit-based billing is available for eligible workspaces. |

## How personal-plan limits work

- Codex maintains separate **5-hour** and **weekly** usage windows. The exact remaining allowance and reset time are shown in **Codex Settings → Usage**; in an active CLI session, run `/status`.
- There is no public conversion from “100% of the weekly allowance” to a fixed number of tokens, tasks, or credits. Consumption changes with the model, task length, token mix, concurrency, and Fast mode.
- If a task reaches a limit while it is running, it may finish that active turn. Subsequent work must wait for reset, use a banked reset where offered, upgrade, or use credits when eligible.

## Pay-as-you-go Codex credits

Plus and Pro use included allowance first. After that, purchased credits can cover Codex use. Credits are shared with supported ChatGPT Work and ChatGPT for Excel use.

| Model | Input | Cached input | Output |
|---|---:|---:|---:|
| GPT-5.6 Sol | 100 credits / 1M tokens | 10 credits / 1M tokens | 500 credits / 1M tokens |
| GPT-5.6 Terra | 50 credits / 1M tokens | 5 credits / 1M tokens | 300 credits / 1M tokens |
| GPT-5.6 Luna | 5 credits / 1M tokens | 0.5 credits / 1M tokens | 30 credits / 1M tokens |

- A typical GPT-5.6 Sol Codex task uses approximately **5–30 credits**.
- Cache writes do not consume credits.
- Fast mode costs more where supported.
- Purchased credits expire 12 months after purchase; they are non-refundable and non-transferable.

## Official references

- [Codex product page](https://openai.com/codex/)
- [ChatGPT plan access and Codex limits](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan)
- [ChatGPT rate card](https://help.openai.com/en/articles/11481834-chatgpt-rate-card-business-enterpriseedu)
- [ChatGPT Pro tiers](https://help.openai.com/en/articles/9793128-about-chatgpt-pro-tiers)
- [ChatGPT Business seats](https://help.openai.com/en/articles/8792828-what-is-chatgpt-business)
