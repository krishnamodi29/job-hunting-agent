# Job Hunting Agent 🔥

An AI agent that automatically fetches, scores, and delivers cybersecurity & IT job listings daily.

## What it does
- Runs every morning at 8am automatically
- Searches Adzuna API for cybersecurity, IT helpdesk, and IT support jobs in New Jersey, USA
- Scores each job 1-10 against a target candidate profile using Groq LLaMA 3.3 70b
- Sends top 5 jobs (score 6+) via email digest
- Saves results to a Notion database for tracking

## Tech Stack
- n8n (workflow automation)
- Adzuna Jobs API
- Groq LLaMA 3.3 70b (AI scoring)
- Notion API (job tracker)
- Gmail (daily digest)

## Architecture
Schedule Trigger → Adzuna API (3 searches) → Merge → AI Scoring → Notion + Gmail
