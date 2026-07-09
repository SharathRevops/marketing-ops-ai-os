# CLAUDE.md — Operating Instructions for This Repo

This file is read by Claude Code (or any Claude-based agent) when working inside this repository. It exists partly as functional context, and partly as a demonstration: this is what "context engineering" looks like when a Marketing Ops leader — not an engineer — sets it up.

---

## What this repo is

`marketing-ops-ai-os` is Sharath Chandra Chaganti's personal Marketing Operations AI system and portfolio. It documents real automations built to solve real MOps problems (lead enrichment, content production, cross-tool orchestration, reporting) using n8n, Make, Claude, and MCP.

## Who's using this file

Either:
1. **Sharath**, running `claude` in this repo to draft a new case study, update a workflow doc, or refresh the impact summary.
2. **A reviewer / interviewer**, running `claude` and typing something like `explain the lead enrichment case study` or `summarize the impact of this repo` to get a guided walkthrough instead of reading raw files.

## How to help each

### If asked to help draft or update a case study
1. Open `case-studies/<project>/README.md` — it follows a fixed template (Problem → Architecture → Build → Impact → What I'd do differently). Preserve that structure.
2. Pull supporting detail from `automations/` (workflow exports) and `prompts/` (the actual prompts used) rather than inventing detail.
3. Keep language operator-first, not engineer-first: lead with the business problem and the metric that moved, then go technical.
4. Never fabricate metrics. If a number isn't in the file, flag it as `[NEEDS DATA]` rather than guessing.

### If asked to explain the repo to a reviewer
1. Start with `README.md` for the one-paragraph pitch.
2. Route deeper questions to the matching `case-studies/*/README.md`.
3. For "why should I hire this person" style questions, pull from `docs/impact-summary.md`.

### If asked to add a new automation
1. Create a new folder under `case-studies/` using the existing template (`playbooks/case-study-template.md`).
2. Export the underlying n8n workflow JSON or Make scenario blueprint into `automations/`, with credentials and account-specific IDs stripped.
3. Save any reusable prompt into `prompts/` with a short header comment describing what it's for and which case study uses it.
4. Update the table in the root `README.md`.

## Ground rules

- **Sanitize before committing.** No real customer data, no live API keys, no internal account IDs. Use placeholders (`{{HUBSPOT_PORTAL_ID}}`, etc.) and note what they represent.
- **Every case study needs a metric**, even a directional one (time saved, error rate reduced, volume handled). If there isn't one yet, mark it `[NEEDS DATA]` instead of writing filler.
- **Prefer showing the artifact over describing it.** A workflow screenshot or a real exported JSON beats a paragraph of prose every time.
