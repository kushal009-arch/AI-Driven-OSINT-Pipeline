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
