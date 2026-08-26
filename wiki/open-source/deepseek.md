# DeepSeek

[Official DeepSeek API pricing](https://api-docs.deepseek.com/quick_start/pricing/)

> API prices in USD per 1M tokens. Verified 25 August 2026.

## Access options

| Access path | Price | Published detail |
|---|---|---|
| DeepSeek-R1 weights | Open model release | Self-hosting requires your own infrastructure and inference stack. |
| DeepSeek API | Token-based | `deepseek-reasoner` provides R1-style reasoning through the API. |
| API off-peak | Lower token rate | Cache-hit / cache-miss / output: US$0.007 / US$0.22 / US$0.66. |
| API peak | 2× off-peak rate | Cache-hit / cache-miss / output: US$0.014 / US$0.44 / US$1.32. |

Current DeepSeek API pricing uses peak and off-peak periods. Model aliases and pricing can change; use the official pricing page before production deployment.

## Official references

- [DeepSeek-R1 repository](https://github.com/deepseek-ai/DeepSeek-R1)
- [DeepSeek API pricing](https://api-docs.deepseek.com/quick_start/pricing/)
- [DeepSeek-R1 API release](https://api-docs.deepseek.com/news/news250120/)
