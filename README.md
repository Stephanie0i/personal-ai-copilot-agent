# 🤖 Personal AI Co-Pilot / Thought Partner & Resource Finder

A specialized, non-conversational AI Agent designed as a direct "Second Brain" and technical consultant. Built with **n8n orchestration** and powered by **Anthropic Claude 3.5 Sonnet**, this agent bypasses casual chit-chat to deliver strict technical evaluations and structured resource retrieval.

---

## 🏗 System Architecture & Workflow Pipeline

```text
[User Query / Chat Trigger]
         │
         ▼
[System Prompt Enforcer (Zero-Fluff Rules)]
         │
         ▼
[AI Agent Node (Claude 3.5 Sonnet)]
         │
         ▼
[Structured 4-Section Output Engine]
```
# 🎯 Key Functional Capabilities
- Direct Technical Critique: Evaluates proposed architecture, logic flaws, debouncing issues, and bottlenecks immediately without conversational fluff.

- Open-Source Repository Fetching: Recommends active GitHub frameworks and libraries suited for the specified architecture.

- Community Discussions: Curates high-value technical threads and video tutorials from YouTube, r/selfhosted, r/programming, and r/LocalLLaMA.

- Visual Asset Mapping: Provides structural blueprints (Sequence Diagrams, Architecture Models, and State Machines) for system design execution.

---

# 🚀 How to Import & Deploy in n8n
Download the Technical Critique AI Agent.json workflow file from this repository.

1. Open your n8n dashboard.

2. Click on Workflows → Import from File.

3. Upload the .json file and assign your Anthropic API Credentials or use the built-in Gateway Credits.

4. Activate the workflow and test it via the Chat Trigger canvas!
