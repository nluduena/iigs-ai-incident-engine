# IIGS – AI-Assisted Incident Engine (MVP)

IIGS (Incident Intelligence & Governance System) is a lightweight AI-assisted workflow automation model built using n8n.

This MVP demonstrates how critical production incidents can be:

- Automatically classified
- Enriched with contextual intelligence
- Evaluated against historical knowledge
- Assessed using confidence thresholds
- Automatically mitigated when conditions are met
- Logged with structured learning feedback

---

## Problem

In many production environments, incident management relies heavily on:

- Manual coordination
- Tribal knowledge
- Repetitive decision-making
- Delayed escalation

This increases MTTR and creates operational dependency on individuals rather than systems.

---

## Solution

This workflow implements:

1. Webhook-based incident ingestion
2. Dynamic severity classification (P1/P2)
3. SLA and escalation policy assignment
4. Historical knowledge matching
5. Confidence-based remediation eligibility
6. Automated mitigation decision
7. Learning feedback loop with recurrence tracking

---

## Example Input

{
  "service": "payments-api",
  "error_code": "DB_TIMEOUT",
  "impact": "high"
}

---

## Example Output (Simplified)

{
  "severity": "P1",
  "eligible_for_auto_remediation": true,
  "decision": "AUTO_REMEDIATION_EXECUTED",
  "status": "MITIGATED"
}

---

## Architecture

See architecture.png for the executive-level workflow diagram.

---

## Author

Nicolás Ludueña  
Reliability & AI Workflow Automation