# 🤖 Brace-AI  
Your AI Automation Platform for Everyday Tasks with SDK and Web Support. Built on Solana.  
*This repository is in active development. While functional, some modules are still being integrated into the mono repo.*

## What is Brace-AI?  
Brace-AI is an intelligent automation platform designed to simplify everyday tasks by integrating AI workflows seamlessly into your daily routine. From automating repetitive tasks to enabling advanced data processing, Brace-AI empowers users with SDK and web support, all built on the Solana blockchain for enhanced efficiency and scalability.  
*Join our stargazers to stay updated! ⭐*.

---
### API Key  
Get started at  [Brace-AI](https://brace-ai.xyz/) for your API key. 

---
## Features  
### Core Capabilities  
- **Automate**: Build end-to-end AI workflows for everyday tasks  
- **Crawl**: Auto-discover and process website structures for data extraction  
- **Extract**: Transform content into structured schemas for RAG, fine-tuning, and analytics  
- **Integrate**: Connect to Solana-based tools, vector DBs, LLMs, and automation platforms  

### Advanced Features  
- **Task Automation**: Chain workflows for seamless task execution  
- **Dynamic Execution**: Browser automation, retries, and JavaScript rendering  
- **Multi-Format Support**: Websites, PDFs, DOCX, and images  
- **Scalability**: Batch processing, proxies, and anti-bot handling  

---
## Quickstart Examples  
### Run a Workflow  
```bash  
curl -X POST https://api.brace-ai.dev/v1/run \  <!-- Update domain -->  
    -H 'Authorization: Bearer brace-YOUR_API_KEY' \  <!-- Update API key prefix -->  
    -d '{  
      "workflow": "crawl-extract",  
      "url": "https://docs.brace-ai.dev"  
    }'  
```  

### Extract Structured Data  
```python  
from brace_ai import BraceAI  # Updated SDK  
class ProductSchema(BaseModel):  
    features: list[str]  
    pricing: str  
data = BraceAI(api_key="brace-YOUR_KEY").extract(  
    url="https://brace-ai.dev/pricing",  
    schema=ProductSchema  
)  
```  

---
## SDK Installation  
### Python  
```bash  
pip install brace-ai  
```  

### Node.js  
```bash  
npm install @brace-ai/sdk  
```  

---
## Deployment Options  
Brace-AI is open-source (AGPL-3.0) with a managed cloud service:  
| Feature               | Self-Hosted | Cloud          |  
|-----------------------|-------------|----------------|  
| Task Automation       | ✅          | ✅ (Enhanced)  |  
| Browser Execution     | ❌          | ✅             |  
| Enterprise SLAs       | ❌          | ✅             |  
| Free Tier             | ✅          | ✅             |  

---
## Contributing  
We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md).  
**Note**: Users must respect website terms of service and robots.txt rules.  

---
## License  
- Core: AGPL-3.0  
- SDKs: MIT  

---
<p align="right">  
  <a href="#readme-top">↑ Back to Top ↑</a>  
</p>
