# Agentic Systems Control Model

## Purpose

Agentic AI systems create new governance requirements because they can plan, call tools, retrieve data, trigger workflows, and influence real operational movement.

This model defines public-safe controls for enterprise agentic systems before production use.

---

## Control Surface

| Area | Required Control |
|---|---|
| Tool access | Every callable tool must have an owner, purpose, scope, and approval boundary. |
| Action authority | Agents must not bind protected action without authority resolution. |
| Human approval | High-impact actions require human approval or explicit delegated authority. |
| Data retrieval | Retrieval scope must be constrained to approved sources. |
| Memory | Persistent memory must be scoped, reviewable, and revocable. |
| Escalation | Ambiguous or high-risk conditions must escalate instead of executing. |
| Logging | Tool calls, refusals, escalations, and approvals must be observable. |
| Revalidation | Changes to tools, permissions, data, model, or scope trigger revalidation. |

---

## Agent Movement Flow

```text
User / system request
        ↓
Intent classification
        ↓
Tool/action eligibility check
        ↓
Data scope check
        ↓
Authority boundary check
        ↓
Risk and impact classification
        ↓
Approve / escalate / refuse / revalidate
        ↓
Tool call only if admitted
        ↓
Telemetry and post-action review
```

---

## Refusal Conditions

An agentic workflow should refuse or halt when:

- tool scope is undefined
- action can create protected effect without approval
- user authority is unresolved
- data source is untrusted or out of scope
- system cannot explain required action path
- persistent memory is unbounded
- telemetry is absent
- high-impact action lacks review

---

## Operating Principle

Agentic systems are not governed by prompt instructions alone.

They are governed by the architecture of allowed movement: what tools exist, what authority applies, what data can be touched, what actions can bind, what must escalate, and what cannot proceed.
