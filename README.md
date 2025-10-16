# AssureAI — Brand Protection Intelligence

AssureAI is a lightweight OSINT tool that detects impersonating social media accounts and fake/phishing websites that target a brand.  
This repository contains the Replit/Gradio MVP used to demonstrate brand protection value to insurers and corporate security teams.

## What it does
- Create brand "ground-truth" profiles (official social links, domains, phones)
- Search public search results (DuckDuckGo) for social media profiles and websites
- Score and flag suspicious matches (typosquatting, handle mismatch, keywords)
- Export executive intelligence packs (CSV, JSON, DOCX)
- UI built with Gradio (clean modern theme)

> NOTE: AssureAI uses only public metadata and DDG queries. It does NOT scrape behind logins or use private APIs (Meta ToS compliant).

## Quick start (run locally / Replit)
```bash
# Setup
git clone <repo-url>
cd assureai
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# Run
python app.py
# Open: http://localhost:5000
Folder structure

app.py — Gradio web UI

core/ — search, scoring, reporting logic

ui/ — reusable UI components and CSS

config/ — example brand profiles

data/exports/ — generated reports (ignored from git)

Contributing

Raise issues, submit PRs.

See CONTRIBUTING.md for guidelines.

License

MIT License — see LICENSE file.

Changelog
2025-10-16

MVP: Gradio UI with brand profile + impersonation scanner using DuckDuckGo (DDGS)

Export: CSV, JSON, DOCX takedown template

Focus change: limited search to social platforms + phishing-like websites

UI redesign: corporate-clean theme (Inter font, blue accent)
