# Automation Engineering Portfolio

**Role:** AI Automation Engineer | **Focus:** Process Efficiency, System Integration & Reliability

## 🚀 Overview
This repository showcases production-grade automation architectures designed to reduce manual operational load and streamline business logic. Unlike simple linear automations, these workflows feature **self-healing logic, error handling, and human-in-the-loop approval systems**.

**Core Tech Stack:**
* **Orchestration:** n8n, Webhooks, Custom JavaScript
* **AI & LLMs:** Gemini 1.5 Pro, OpenAI (DALL-E 3), Anthropic Claude
* **Integrations:** WordPress, DataForSEO, Google Workspace, Slack, Firecrawl, Pinterest, Threads

---

## 📂 Featured Projects

| Project | Business Impact | Tech Highlights |
| :--- | :--- | :--- |
| **[1. SEO Blog Content Pipeline](./projects/01-seo-blog-content-pipeline)** | Autonomous "Research-to-Publish" agent. Researches keywords, writes SEO articles, generates DALL-E 3 images, and publishes to WordPress after human approval. | DataForSEO API, Gemini 1.5 Pro, DALL-E 3, WordPress API, Advanced Prompt Engineering |
| **[2. Omni-Channel Social Agent](./projects/02-omni-channel-social-agent)** | Automates content for 7 platforms from 1 asset with human approval. | Gemini Vision, Custom API Nodes (Threads), Error Reporting |
| **[3. Finance Invoice Processor](./projects/03-finance-invoice-processor)** | Eliminates manual data entry by extracting unstructured invoice data. | OCR, Regex, Google Sheets Database |
| **[4. Cold Email Engine](./projects/04-cold-email-outreach-engine)** | Manages complex outreach sequences without expensive SaaS tools. | Custom JS Date Logic, Gmail API Threading |
| **[5. Lead Gen Pipeline](./projects/05-lead-gen-enrichment-pipeline)** | Automates scraping and enrichment of high-volume datasets. | Firecrawl, People Data Labs API, Batch Processing |
| **[6. Internal HR Tool: ATS Optimizer](./projects/06-internal-hr-tool-ats-optimizer)** | Automates candidate screening by scoring resumes against JDs. | PDF Parsing, Gemini 1.5 Pro, Structured JSON Output |

*(Click the project names to view the source code)*

---

## ⚙️ How to Run These Workflows
1.  **Import:** Download the `workflow.json` file from the specific project folder.
2.  **Load:** In your n8n instance, go to `Workflows` > `Import from File`.
3.  **Credentials:** All sensitive API keys have been stripped for security. You must configure your own credentials in n8n (OpenAI, Google, DataForSEO, etc.).

## 🛡️ Reliability Philosophy
My automations are built for the real world:
* **Error Handling:** Critical failures trigger Slack/Email alerts.
* **Idempotency:** Workflows check for existing records before creating new ones to prevent duplicates.
* **Security:** No hardcoded API keys; strictly environment variables and credential managers.

---
*Created by Sahil Shehzad*
