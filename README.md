# Aegis Research SDK

Python SDK for the [Aegis Research API](https://aegisagent.ai/research) - AI-powered web research as a service.

## Installation

```bash
pip install aegis-research
```

## Quick Start

```python
from aegis_research import AegisResearch

# Initialize client
client = AegisResearch(api_key="res_your_api_key")

# Execute research
result = client.research("Best practices for API rate limiting in 2025")

print(result.summary)
for finding in result.key_findings:
    print(f"- {finding}")
```

## Features

- **AI-Powered Research**: Get synthesized research results, not just search links
- **Multiple Depth Levels**: Choose shallow (1 credit), medium (3 credits), or deep (10 credits) research
- **Caching**: Results cached for 24 hours to save credits
- **Source Citations**: Every claim backed by sources

## Pricing

| Tier | Price | Credits/Month | Rate Limit |
|------|-------|---------------|------------|
| Free | $0 | 500 | 10/min |
| Starter | $9/mo | 2,000 | 20/min |
| Pro | $49/mo | 10,000 | 60/min |

Get your API key at [aegisagent.ai/research](https://aegisagent.ai/research)

## License

MIT
