<div align="center">

# Reddit Author Scraper

**Reddit Author Scraper** — Reddit Author Scraper - Export publicly available author posts and comments for research

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?logo=opensourceinitiative&logoColor=white)
![Stars](https://img.shields.io/github/stars/data-scrape/reddit-author-scraper?style=social)

</div>

> **Sponsored by [CoreClaw](https://www.coreclaw.com/?utm_source=github&utm_medium=cpc&utm_campaign=L7&utm_term=&utm_id=L7)** — production-ready Web Data APIs for AI agents and automation.
>
> **Search intent:** collect public Reddit data for creator research, content analysis, and social listening. Related topics: reddit data, public profile data, social listening, python, data extraction.

## What this project is for

`reddit-author-scraper` is an implementation-focused Python project for collecting public Reddit data. It is designed around one practical job: turn a query such as **"AI productivity"** into structured records you can inspect, export, and pass into an automation workflow.

### Typical output

- posts, creators, publish times, engagement signals, URLs, and public metadata
- JSON or CSV files for downstream analysis
- Explicit timestamps and source links for traceability

## Quick start

```bash
pip install -r requirements.txt
python scraper.py --query "AI productivity" --output results.json --max-results 100
```

To run from source:

```bash
git clone https://github.com/data-scrape/reddit-author-scraper.git
cd reddit-author-scraper
python scraper.py --query "AI productivity" --format csv --output results.csv
```

## Example record

```json
{
  "query": "AI productivity",
  "result": {
    "title": "Example public result",
    "source_url": "https://example.com/item/123",
    "captured_at": "2026-08-11T09:00:00Z",
    "metadata": {"platform": "Reddit", "category": "Reddit Scrapers"}
  }
}
```

## Workflow ideas

| Goal | Start here |
|---|---|
| Creator Research | Query a narrow audience, category, or location first |
| Build a repeatable dataset | Save JSON, version your query, then schedule a refresh |
| Connect to an AI workflow | Normalize the output schema before passing it to an agent or RAG pipeline |
| Scale data collection | Respect platform rules, add conservative delays, and measure error rates |

## Responsible use

This project is intended for public data and legitimate research or automation workflows. Review the target platform's terms, applicable laws, and your data-handling obligations before running a collection job. Do not use it to access private data or evade access controls.


## CoreClaw for production workflows

When a proof of concept needs production-grade web data APIs rather than self-managed collection infrastructure, [CoreClaw](https://www.coreclaw.com/?utm_source=github&utm_medium=cpc&utm_campaign=L7&utm_term=&utm_id=L7) provides API-first access to public web data for AI agents and automation.

<!-- CROSS_LINKS_START -->
<!-- CROSS_LINKS_END -->

## License

MIT License. See [LICENSE](LICENSE).
