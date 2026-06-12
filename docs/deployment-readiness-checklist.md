# Deployment Readiness Checklist

## Purpose

This checklist defines what must be resolved before an enterprise AI use case advances from idea, pilot, or prototype into a production-facing environment.

---

## Ownership

- [ ] Business owner assigned
- [ ] Technical owner assigned
- [ ] Security reviewer assigned
- [ ] Data/privacy reviewer assigned where required
- [ ] Production support owner assigned

---

## Data Scope

- [ ] Data sources identified
- [ ] Data classification documented
- [ ] Sensitive data status confirmed
- [ ] Retrieval scope defined
- [ ] Data retention expectations documented
- [ ] Data minimization reviewed
- [ ] Access policy mapped

---

## Identity and Authority

- [ ] User roles defined
- [ ] Service identities documented
- [ ] Privileged access reviewed
- [ ] Approval authority mapped
- [ ] Agent/tool authority bounded
- [ ] Override path documented

---

## Model / RAG / Agent Controls

- [ ] Model or AI service identified
- [ ] Prompt or system behavior documented at a public-safe level
- [ ] RAG source authority verified
- [ ] Grounding evaluation completed
- [ ] Agent tools inventoried
- [ ] Tool-call boundaries defined
- [ ] Human approval requirements defined
- [ ] Refusal and escalation conditions documented

---

## Responsible AI and Security

- [ ] Threat model completed
- [ ] Privacy review completed where required
- [ ] Safety testing completed
- [ ] Hallucination / groundedness review completed
- [ ] Abuse or misuse cases reviewed
- [ ] Auditability requirements documented
- [ ] Incident path defined

---

## Observability

- [ ] Logs defined
- [ ] Metrics defined
- [ ] Alerts defined
- [ ] Review cadence defined
- [ ] Drift or change detection defined
- [ ] Evidence retention defined

---

## Revalidation

Revalidation is required when any of the following changes:

- model
- prompt
- data source
- retrieval corpus
- agent tool
- workflow permission
- production environment
- business owner
- security or privacy policy
- regulatory requirement
- customer-facing scope

---

## Final Decision

```text
ADMIT      Required controls and evidence are present.
HOLD       Missing evidence or control coverage must be completed.
REFUSE     Critical boundary is missing; movement cannot advance.
REVALIDATE Prior approval no longer matches current conditions.
```
