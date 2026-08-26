# GPT API

[Official OpenAI API model catalogue](https://developers.openai.com/api/docs/models)

> API pricing in USD. Information verified 25 August 2026.

## API access

| Requirement | Published detail |
|---|---|
| Billing | The OpenAI API is **separate** from ChatGPT Free, Go, Plus, Pro, Business, Edu, and Enterprise billing. A ChatGPT subscription does not include API credits or API rate limits. |
| Account | Create an API Platform organization/project, add API billing, then create a project API key. |
| Billing model | Pay-as-you-go token billing. The Responses API, Chat Completions API, Batch API, and Assistants API do not carry separate endpoint fees. |
| GPT-5.6 family on API Free tier | Not supported. |
| GPT-5.6 family from API Tier 1 | Available after at least **US$5** in API spend. |
| Usage tiers | API rate limits and approved monthly usage limits increase automatically with qualifying spend. They are organization/project controls—not ChatGPT-plan limits. |

## GPT-5.6 API model comparison

| API model ID | API alias | Standard input / cached input / output<br>per 1M tokens | Context / max output | Available API capabilities |
|---|---|---:|---:|---|
| `gpt-5.6-sol` | `gpt-5.6` | US$4.00 / US$0.40 / US$20.00 | 1.05M / 128K tokens | Responses, Chat Completions, Batch; streaming, function calling, structured outputs, image input; web search, file search, computer use |
| `gpt-5.6-terra` | — | US$2.00 / US$0.20 / US$12.00 | 1.05M / 128K tokens | Same API capabilities as Sol |
| `gpt-5.6-luna` | — | US$0.20 / US$0.02 / US$1.20 | 1.05M / 128K tokens | Same API capabilities as Sol |

- `gpt-5.6` is an alias for **GPT-5.6 Sol**.
- Pricing above is **Standard / short-context** pricing. For requests above 272K input tokens, long-context prices apply: 2× input and cached-input rates, and 1.5× output rates.
- Cache writes are billed separately at 1.25× the uncached input rate.
- Fast mode costs more. Batch and Flex processing use lower prices but trade off latency or availability.

## API usage tiers and spend caps

| API tier | Qualification | Approved monthly usage limit | GPT-5.6 access |
|---|---:|---:|---|
| Free | Eligible geography | US$100/month | Not supported |
| Tier 1 | US$5 paid | US$100/month | Supported |
| Tier 2 | US$50 paid | US$500/month | Supported |
| Tier 3 | US$100 paid | US$1,000/month | Supported |
| Tier 4 | US$250 paid | US$5,000/month | Supported |
| Tier 5 | US$1,000 paid | US$200,000/month | Supported |

The monthly figure is an API organization’s maximum approved spend—not free included credit. Check the API Platform **Limits** page for the current organization and project limits.

## GPT-5.6 rate limits

| API tier | Sol / Terra tokens per minute | Luna tokens per minute |
|---|---:|---:|
| Free | Not supported | Not supported |
| Tier 1 | 500,000 | 500,000 |
| Tier 2 | 1,000,000 | 2,000,000 |
| Tier 3 | 2,000,000 | 4,000,000 |
| Tier 4 | 4,000,000 | 10,000,000 |
| Tier 5 | 40,000,000 | 180,000,000 |

Rate limits are enforced at the organization and project level. The API response headers show the current request/token limits, remaining capacity, and reset time.

## Official references

- [GPT API model catalogue](https://developers.openai.com/api/docs/models)
- [GPT-5.6 model comparison](https://developers.openai.com/api/docs/models/compare)
- [API pricing](https://developers.openai.com/api/docs/pricing)
- [API rate limits and usage tiers](https://developers.openai.com/api/docs/guides/rate-limits)
- [ChatGPT and API billing are separate](https://help.openai.com/en/articles/9039756-managing-billing-settings-on-chatgpt-web-and-platform)
