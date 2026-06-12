# AI Governance Control Matrix

## Purpose

This matrix maps enterprise AI movement to required controls before production advancement.

---

| Control Area | Required Evidence | Failure Outcome |
|---|---|---|
| Ownership | Named business and technical owners | HOLD |
| Data classification | Data type, sensitivity, source, and permitted use documented | HOLD / REFUSE |
| Identity and access | Access model, roles, approval, and privileged paths defined | HOLD / REFUSE |
| Privacy | Data minimization, retention, and policy review documented | HOLD / REFUSE |
| Security | Threat model, misuse cases, monitoring, and escalation path documented | HOLD / REFUSE |
| RAG grounding | Approved source corpus and grounding evaluation present | HOLD |
| Agent/tool use | Tool inventory, action boundary, and approval model defined | REFUSE |
| Evaluation | Quality, safety, hallucination, and reliability testing documented | HOLD |
| Observability | Telemetry, logging, and incident response path defined | HOLD / REFUSE |
| Revalidation | Change triggers documented for model, prompt, data, tools, policy, and environment | HOLD |

---

## Outcome Rule

```text
ADMIT only when required evidence exists for the risk tier.
HOLD when the system is incomplete but not structurally unsafe.
REFUSE when protected movement can bind without authority, control, or observability.
REVALIDATE when prior approval no longer matches current conditions.
```
