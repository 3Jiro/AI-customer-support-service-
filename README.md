# 🤖 Enterprise AI Customer Support Representative (n8n + Verified Logic)



### 🌟 Overview

An advanced n8n-based AI Agent designed for high-accuracy customer support. This project solves the "AI Hallucination" problem by implementing a custom verification layer that cross-references LLM outputs against a Google Sheets "Source of Truth" in real-time.



### 🛠️ Technical Architecture

* **LLM Orchestration:** AI Agent node utilizing Tool-calling for real-time database lookups.

* **Metadata Injection Protocol:** A custom prompting technique that forces the LLM to output structured state data (`[VERIFY: Status=...]`) for post-processing.

* **Deterministic Validation:** A JavaScript-based "Confidence Scorer" that compares natural language responses against raw database values.

* **Stateless Webhook Integration:** Engineered to act as a backend API for web-based chat interfaces.



### 🚀 Key Challenges Overcome

* **Data Siloing:** Resolved n8n's tool-scoping limitations by bridging ephemeral tool data into the main execution timeline.

* **Output Polishing:** Implemented Regex-based string manipulation to hide technical verification tags from the end-user.


### ⚙️ Tech stack
* **Primary Engine:** n8n (self hosted) / webhooks
* **AI/LLM:** Google gemini / OpenAI
* **Data & storage:** Google sheets
* **Communication:** Slack / Webhook
