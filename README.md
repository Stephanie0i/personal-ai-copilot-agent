# 🤖 Technical Critique AI Agent (Production-Ready)

> **An autonomous, non-conversational AI Agent built on n8n and Anthropic Claude 5 Sonnet.**  
> It serves as a direct "Second Brain" and Senior Technical Partner that delivers objective architectural critiques, live open-source resource retrieval, real-world community insights, and visual asset suggestions—completely free of conversational fluff or pleasantries.

---


## 🚀 Key Modules & Functional Pillars

- **Analytical Strategic Critique Engine:** Powered by **Claude 3.5 Sonnet** to rigorously evaluate proposed system architectures, identify performance bottlenecks, critique technical trade-offs, and suggest concrete edge-case remedies.
- **Live GitHub Repository Fetcher:** Connects directly to the **GitHub REST API** to automatically search, filter, and extract active, relevant open-source frameworks, libraries, and tools matching the user's technical stack.
- **Developer Discussion Aggregator:** Queries the **Hacker News (Algolia) API** in real-time to surface real-world community sentiment, production post-mortems, and developer warnings.
- **Visual Asset Search Engine:** Integrates with the **Unsplash REST API** to bypass AI image generation in favor of real-world high-resolution photography, system architecture visual references, desktop wallpapers, and media editing assets.
- **Token-Efficient Data Pipeline:** Features custom JavaScript mapping and parsing expressions in n8n nodes to sanitize raw JSON responses before prompting the LLM, ensuring minimal latency and optimal context utilization.

---

## 🏗️ System Architecture & Workflow Pipeline

The n8n workflow executes a sequential multi-stage pipeline:

```text
┌────────────────────────┐     ┌────────────────────────┐     ┌────────────────────────┐
│   Chat Input Trigger   │ ──► │ Extract Keywords Node  │ ──► │  GitHub REST API Node  │
└────────────────────────┘     └────────────────────────┘     └────────────────────────┘
                                                                          │
┌────────────────────────┐     ┌────────────────────────┐                 ▼
│  AI Agent (Claude 5)   │ ◄── │   Unsplash API Node    │ ◄── ┌────────────────────────┐
│   [Critique Output]    │     └────────────────────────┘     │ Hacker News API Node   │
└────────────────────────┘                                    └────────────────────────┘

```


## 📋 Prerequisites & Credentials

Before deploying this workflow, ensure you have active API keys for the following services:

1. **n8n Instance:** Self-hosted (Docker/npm) or n8n Cloud (v1.0+).
2. **Anthropic API Key:** Access to `Claude 5 Sonnet` (`claude-sonnet-5`).
3. **GitHub Personal Access Token (PAT):** For authenticated repository queries.
4. **Unsplash API Access Key:** Free developer tier access key.

---


# 🚀 How to Import & Deploy in n8n
Download the Technical Critique AI Agent.json workflow file from this repository.

1. Open your n8n dashboard.

2. Click on Workflows → Import from File.

3. Upload the .json file and assign your Anthropic API Credentials or use the built-in Gateway Credits.

4. Activate the workflow and test it via the Chat Trigger canvas!

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
