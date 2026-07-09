# AI Governance Checklist for Marketing Operations

A practical checklist for standing up AI agents/automation inside a MarOps function without creating compliance, data, or brand risk. Written from hands-on experience building the automations in this repo — not a theoretical framework.

## Before you connect an AI agent to a production system

- [ ] **Data scope is explicit.** What data can the agent read/write? Is PII involved? Is there a data retention policy for anything the model sees?
- [ ] **Least-privilege access.** Agent/API credentials scoped to only the objects and fields required — not full admin access to CRM/MAP.
- [ ] **Human-in-the-loop for anything customer-facing.** Draft/suggest, don't auto-send, until the workflow has a proven track record.
- [ ] **Audit trail exists.** Every automated write (lead score change, enrichment update, record creation) is logged and attributable.
- [ ] **Failure mode is defined.** What happens when the API times out, the model returns malformed output, or a workflow runs twice? Silent failure is the highest-risk outcome.
- [ ] **Sanitization before any external LLM call.** No raw customer PII sent to a third-party model unless contractually covered by your data processing agreement with that vendor.

## Before you roll out to the team

- [ ] Documented in plain language what the automation does, so it's not a "black box" the team distrusts.
- [ ] Rollback plan — can you disable the automation and revert to manual process in under a day?
- [ ] Owner assigned (not just "IT" or "the person who built it") for ongoing monitoring.

## Before you scale it

- [ ] Cost model understood (API calls, token usage, workflow platform tier).
- [ ] Metric baseline captured *before* rollout, so impact is measurable, not anecdotal.
- [ ] Cross-functional sign-off if the automation touches data owned by Sales, RevOps, or Legal.

---

*This checklist is applied, not aspirational — see individual case studies in `/case-studies` for how it was used in practice.*
