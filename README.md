# AI-Driven-OSINT-Pipeline

Overview
An automated Open Source Intelligence (OSINT) pipeline built with n8n and Google Gemini 1.5. The system monitors geopolitical RSS feeds, aggregates key developments, and uses Generative AI to produce a concise 3-bullet point intelligence brief delivered directly to Discord.

How It Works
Ingestion: Scans RSS feeds for the latest geopolitical updates.

Filtering: Limits processing to the top 5 most recent/relevant items to reduce noise.

Aggregation: Consolidates disparate headlines into a structured data object.

Analysis: Uses the Gemini 1.5 Flash model via a LangChain Basic LLM Chain to perform sentiment and strategic risk analysis.

Delivery: Posts the final "Intelligence Brief" to a designated Discord channel.

Tech Stack
Automation: n8n

AI/LLM: Google Gemini 1.5 Flash

Integration: Discord Webhooks, RSS/XML

🚀 How to Deploy
Clone the Repository:

Bash
git clone https://github.com/kushal009-arch/GeoIntel-Sentinel.git
Import to n8n:

Open your n8n instance.

Create a new workflow.

Click the Settings menu (three dots) and select Import from File.

Choose the workflow.json from this repository.

Setup Credentials:

Google Gemini: Add your API Key to the Google Gemini Chat Model node.

Discord: Create a Webhook in your Discord Server settings and paste the URL into the Discord node.

Execute: Click "Execute Workflow" to pull the latest intelligence brief.
