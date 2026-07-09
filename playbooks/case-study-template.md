# Case Study Template

Copy this into any `case-studies/<project-name>/README.md` and fill it in. Delete instructions in *italics* once written.

---

# [Project Name]

*One sentence: what does this system do, for whom, in what tool stack?*

## The Problem

*What was broken or manual before this existed? Who felt the pain (you, your team, sales, the exec who saw the report)? Be specific — a number, a delay, a recurring manual task.*

*Example shape: "Marketing-qualified leads sat in HubSpot for 24–48 hours before enrichment, because enrichment was a manual weekly batch job run by one analyst. SDRs were calling stale/incorrect data."*

## The Approach

*Why this architecture and not another? What did you consider and reject? This section is where leadership judgment shows — not just "I used n8n," but "I chose event-triggered over batch because X."*

## Architecture

*Diagram or ASCII flow. See `/architecture` for a rendered version if you built one.*

```
[Trigger] → [Step] → [Step] → [Output]
```

## The Build

*What actually got built. Link to the real artifacts:*
- Workflow: `automations/n8n-workflows/<file>.json`
- Prompts used: `prompts/<file>.md`
- Key config/decisions worth calling out

*Keep this section honest about scope — a working v1 with known gaps is more credible than a claimed "complete platform."*

## Impact

*Quantify wherever possible. If you don't have a hard number, use a directional one and label it as an estimate.*

| Metric | Before | After |
|---|---|---|
| *(e.g. enrichment latency)* | *(e.g. 24-48 hrs)* | *(e.g. <5 min)* |

## What I'd Do Differently

*Shows judgment and growth, not just execution. One or two honest notes — a scaling limit you hit, a tool you'd swap, a governance gap you'd close next.*

## Try It

*If genuinely reusable: link the exported workflow and any setup steps. If it's tightly coupled to your internal systems, say so plainly instead of implying it's plug-and-play.*
