# Marketing Ops AI-OS

**A working system for running Marketing Operations with AI agents and automation — not a slide deck about it.**

Built and operated by [Sharath Chandra Chaganti](https://www.linkedin.com/) — Marketing Operations Manager, 15+ years in MarTech / Lead Ops / RevOps (Marketo, HubSpot, Salesforce, SFMC, MS Dynamics 365, Power BI) — now applying AI agents (Claude, MCP, n8n, Make) to the operational layer of B2B marketing.

This repo is the evidence behind that claim: real automations, real prompts, real architecture, documented as case studies.

---

## Why this exists

Most "AI in MarTech" portfolios are either (a) a resume line, or (b) a ChatGPT screenshot. This is neither.

Every project here started as a real operational problem inside a Marketing Ops function — lead enrichment latency, content production bottlenecks, cross-tool context loss, manual reporting — and was solved by building an actual agent, workflow, or integration. The repo documents the problem, the architecture, the build, and the measurable outcome for each one.

If you're evaluating me for a Head of Marketing Operations / Director of Marketing Operations / AI Marketing Transformation role, this is meant to answer the question **"can this person actually build the AI-driven MarOps function they're describing, or just talk about it?"**

---

## Repo Map

```
marketing-ops-ai-os/
│
├── README.md                          ← you are here
├── CLAUDE.md                          ← how I use Claude Code / MCP to run this repo and my daily MOps work
│
├── case-studies/                      # each project: problem → architecture → build → impact
│   ├── thought-orchestrator/
│   ├── n8n-content-automation-engine/
│   ├── claude-hubspot-lead-enrichment/
│   └── mcp-server-integration/
│
├── automations/                       # exported, sanitized workflow definitions
│   ├── n8n-workflows/                 #   .json exports + setup notes
│   └── make-scenarios/                #   scenario blueprints + setup notes
│
├── prompts/                           # production prompts used inside these systems
│
├── playbooks/                         # reusable MOps frameworks (not tool-specific)
│   ├── ai-governance-checklist.md
│   ├── lead-lifecycle-automation-framework.md
│   └── campaign-ops-runbook.md
│
├── architecture/                      # system diagrams for each case study
│
├── docs/                              # leadership narrative — impact summary, AI adoption roadmap
│
└── assets/screenshots/                # visual proof (dashboards, workflow canvases, output samples)
```

---

## Case Studies

| Project | Problem | Stack | Status |
|---|---|---|---|
| [Thought Orchestrator](case-studies/thought-orchestrator/) | *(fill in one-line problem statement)* | Claude, n8n | *(draft / live)* |
| [n8n Content Automation Engine](case-studies/n8n-content-automation-engine/) | *(fill in)* | n8n, Claude API | *(draft / live)* |
| [Claude + HubSpot Lead Enrichment](case-studies/claude-hubspot-lead-enrichment/) | *(fill in)* | Claude API, HubSpot API | *(draft / live)* |
| [MCP Server Integration](case-studies/mcp-server-integration/) | *(fill in)* | MCP, Claude, CRM/MAP tools | *(draft / live)* |

---

## Who I am / what I bring

- 15+ years in MarTech, Lead Operations, and Revenue Operations
- Core stack: Marketo, HubSpot, Salesforce, SFMC, MS Dynamics 365, Power BI, Make, n8n
- Salesforce certified (incl. AI Associate)
- Manage a team spanning US, EMEA, and APJ stakeholders at Hitachi Vantara
- Currently building this system as both a working internal capability and a public portfolio asset

---

## How to read this repo

- **Skimming for fit?** Read this README + `docs/impact-summary.md`.
- **Technical interviewer?** Open any `case-studies/*/README.md` — each follows Problem → Architecture → Build → Impact → What I'd do differently.
- **Want to see the actual automations?** `automations/` has sanitized, importable n8n/Make exports.
- **Curious how I use AI to run this repo itself?** See `CLAUDE.md`.

---

*This is a living repo — updated as new automations ship and existing ones evolve.*
