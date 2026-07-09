# Automations

Exported, sanitized workflow definitions from production systems documented in `/case-studies`.

## Before adding a file here

- Strip all real API keys, tokens, and credentials — use `{{PLACEHOLDER}}` syntax.
- Strip real account/portal/instance IDs (HubSpot portal ID, Salesforce org ID, etc.).
- Strip any real customer or prospect data from sample payloads — use synthetic examples.
- Add a short `README.md` alongside each export explaining: what it does, what it connects to, and how to import/adapt it.

## Structure

- `n8n-workflows/` — `.json` workflow exports, importable directly into n8n
- `make-scenarios/` — Make scenario blueprints + setup notes (Make blueprints export as JSON too, but note any manual reconfiguration steps since Make's import isn't always 1:1)
