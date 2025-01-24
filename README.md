Here’s the updated README for **CrawlifAI** with all references to "Firecrawl" replaced and branding aligned with your project:

```markdown
<h3 align="center">
  <a name="readme-top"></a>
  <img
    src="https://raw.githubusercontent.com/your-username/crawlifai/main/img/crawlifai_logo.png"  <!-- Update logo path -->
    height="200"
  >
</h3>
```
# 🤖 CrawlifAI

Empower your AI apps with clean data from any website. Featuring advanced scraping, crawling, and data extraction capabilities.

_This repository is in development, and we’re still integrating custom modules into the mono repo. It's not fully ready for self-hosted deployment yet, but you can run it locally._

## What is CrawlifAI?

CrawlifAI is an API service that takes a URL, crawls it, and converts it into clean markdown or structured data. We crawl all accessible subpages and deliver LLM-ready content. No sitemap required.

*Join our stargazers to stay updated! ⭐*

## How to Use It?

We provide an easy-to-use API with our hosted version. You can self-host the backend or use our cloud service. Get started with these resources:

- [x] **API**: [Documentation](https://docs.crawlifai.dev/api-reference/introduction) <!-- Update links -->
- [x] **SDKs**: [Python](https://docs.crawlifai.dev/sdks/python), [Node](https://docs.crawlifai.dev/sdks/node), [Go](https://docs.crawlifai.dev/sdks/go)
- [x] **LLM Frameworks**: [Langchain](https://python.langchain.com/docs/integrations/document_loaders/crawlifai/), [Llama Index](https://docs.llamaindex.ai/en/latest/examples/data_connectors/WebPageDemo/), [CrewAI](https://docs.crewai.com/)
- [x] **Low-Code Tools**: [Langflow](https://docs.langflow.org/), [Dify](https://dify.ai/blog/integrated-with-crawlifai), [Zapier](https://zapier.com/apps/crawlifai)
- [ ] Want an SDK or Integration? [Open an issue](https://github.com/your-username/crawlifai/issues).

**To run locally**, see our [self-hosting guide](CONTRIBUTING.md).

---

### API Key
Sign up at [CrawlifAI](https://crawlifai.dev) to get your API key. <!-- Update domain -->

---

## Features

### Core Capabilities
- **Scrape**: Extract content in markdown, HTML, or structured formats
- **Crawl**: Auto-discover and process all subpages
- **Extract**: Transform content into AI-ready schemas
- **Map**: Rapid URL discovery for any domain
- **Batch Processing**: Handle thousands of URLs simultaneously

### Advanced Features
- **AI-Powered Parsing**: LLM-driven schema extraction
- **Browser Actions**: Click, scroll, input, wait
- **Dynamic Content**: Handle JavaScript-rendered pages
- **Media Support**: PDFs, DOCX, images
- **Enterprise-Grade**: Proxies, retries, anti-bot bypass

---

## Quickstart Examples

### Scrape a URL
```bash
curl -X POST https://api.crawlifai.dev/v1/scrape \  <!-- Update domain -->
    -H 'Authorization: Bearer cai-YOUR_API_KEY' \  <!-- Update API key prefix -->
    -d '{
      "url": "https://docs.crawlifai.dev",
      "formats": ["markdown"]
    }'
```

### Crawl a Website
```bash
curl -X POST https://api.crawlifai.dev/v1/crawl \
    -H 'Authorization: Bearer cai-YOUR_API_KEY' \
    -d '{
      "url": "https://docs.crawlifai.dev",
      "limit": 50
    }'
```

### Extract Structured Data
```python
from crawlifai import CrawlifAI  # Updated SDK name

class CompanySchema(BaseModel):
    mission: str
    open_source: bool

data = CrawlifAI(api_key="cai-YOUR_KEY").extract(
    url="https://crawlifai.dev",
    schema=CompanySchema
)
```

---

## SDK Installation

### Python
```bash
pip install crawlifai-py  # Updated package name
```

### Node.js
```bash
npm install @crawlifai/sdk  # Updated package name
```

---

## Self-Hosting vs Cloud

CrawlifAI is open-source (AGPL-3.0) with a managed cloud option:

| Feature               | Self-Hosted | Cloud          |
|-----------------------|-------------|----------------|
| Auto-scaling          | ❌          | ✅             |
| Browser Automation    | ❌          | ✅             | 
| Enterprise SLAs       | ❌          | ✅             |
| Free Tier             | ✅          | ✅             |

---

## Contributing
We welcome contributions! See our [contributing guide](CONTRIBUTING.md) for details. 

**Important**: Users must comply with website terms of service and robots.txt rules.

---

## License
- Core: AGPL-3.0
- SDKs: MIT

---

<p align="right">
  <a href="#readme-top">↑ Back to Top ↑</a>
</p>
```

Key changes made:
1. Replaced all "Firecrawl" references with "CrawlifAI"
2. Updated logo path (you'll need to add your actual logo)
3. Changed API endpoints to `api.crawlifai.dev`
4. Modified SDK package names and imports
5. Updated API key prefix to `cai-`
6. Simplified the feature comparison table
7. Removed redundant code examples (kept core functionality)
8. Streamlined documentation links

Would you like me to adjust any specific sections further?
