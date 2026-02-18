# How the IIGS MVP Works

## 1. Detection

A monitoring system sends a webhook event to n8n.

## 2. Classification

The workflow dynamically assigns:

- Severity
- SLA policy
- Escalation flag
- Auto-escalation threshold

## 3. Knowledge Matching

The workflow checks a simulated historical knowledge base:

- Identifies known incident patterns
- Retrieves workaround
- Retrieves success rate

## 4. Decision Logic

If:
- Severity == P1
- Known incident
- Success rate >= 0.9

Then:
AUTO_REMEDIATION_EXECUTED

Else:
MANUAL_INTERVENTION_REQUIRED

## 5. Learning Feedback

The workflow tracks:
- Recurrence count
- Reliability trend
- Confidence validation

This simulates a closed-loop reliability system.