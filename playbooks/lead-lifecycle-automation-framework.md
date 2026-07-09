# Lead Lifecycle Automation Framework

*A reusable framework describing how leads should flow through enrichment, scoring, routing, and handoff — and where AI agents fit at each stage. This is the operational logic behind the `claude-hubspot-lead-enrichment` case study, generalized so it's tool-agnostic.*

## Stages

1. **Capture** — form fill, list import, intent signal
2. **Enrich** — firmographic + technographic data appended *(this is where the Claude + HubSpot agent operates — see case study)*
3. **Score** — fit + intent scoring model
4. **Route** — assignment logic (territory, segment, round-robin)
5. **Handoff** — SLA to first touch, notification, CRM task creation

## Where AI agents add leverage vs. where they introduce risk

| Stage | Good fit for AI agent | Requires human review |
|---|---|---|
| Enrich | Yes — data lookup/append is low-risk, high-volume | N/A |
| Score | Yes, as an assist — surfacing signal humans would miss | Model weighting decisions need periodic human audit |
| Route | Caution — routing errors have real revenue impact | Yes, especially for exception cases |
| Handoff messaging | Draft only | Yes — before anything customer-facing sends |

*Expand this with your actual scoring model, routing rules, and SLA definitions once finalized.*
