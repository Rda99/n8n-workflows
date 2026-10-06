# n8n-workflows

Automation templates by **Rajdip Dutta** — Kolkata, India (IST).

Self-hosted n8n on Linux (VPS, Docker) running production automations daily:
lead capture, AI triage, reporting pipelines, scheduled agents. Python,
JavaScript, Java, C/C++. REST APIs, webhooks, Google Sheets, WhatsApp
Business, OpenAI/Gemini behind HTTP nodes.

## lead-capture-ai-reply.json

Web form → AI classification + drafted reply → Google Sheets log.

```
n8n import:workflow --input=lead-capture-ai-reply.json
```

Then:
1. Set your OpenAI API key in the "AI triage + draft" HTTP Request node header.
2. Connect your Google Sheets credential in "Log to Sheet" and pick your
   document + sheet.
3. Activate the workflow, open the form URL (`/form/lead-capture`) and submit
   a test lead — watch the row land with the AI classification.

Every workflow here ships the way I deliver client work: importable,
documented, testable before you pay for anything beyond the agreed scope.

More templates added weekly. For custom builds, find me on the n8n community
forum (@Rda99).
