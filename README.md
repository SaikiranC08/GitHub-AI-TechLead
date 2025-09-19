# AI Tech Lead GitHub App

## Overview
An installable GitHub App that automates code review and unit testing using AI agents (Gemini/OpenAI), CrewAI, and Python.

## Features
- Automated code reviews (PEP8, bugs, documentation)
- AI-generated unit tests (pytest)
- Markdown reports posted to PRs
- Free-tier friendly for students

## Tech Stack
- Python 3.10+
- CrewAI
- Flask
- PyGithub
- google-generativeai
- pytest
- Docker

## Setup Instructions

1. **Clone and prepare your environment**
   ```bash
   git clone https://github.com/SaikiranC08/GitHub-AI-TechLead.git
   cd GitHub-AI-TechLead
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

2. **Configure secrets**
   - Copy `.env.example` to `.env` and fill in your API keys when ready.

3. **Run locally**
   ```bash
   python src/ai_tech_lead/watcher_server.py
   ```

4. **Build/run with Docker**
   ```bash
   docker build -t ai-tech-lead .
   docker run --env-file .env -p 5000:5000 ai-tech-lead
   ```

## Full build guide
See [ai_tech_lead_guide.md](ai_tech_lead_guide.md).
