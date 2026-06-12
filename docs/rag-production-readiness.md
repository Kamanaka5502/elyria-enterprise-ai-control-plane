# RAG Production Readiness

## Purpose

Retrieval-augmented generation systems introduce risk when generated answers depend on retrieved content whose authority, freshness, completeness, and scope are not governed.

This readiness model defines what must be resolved before a RAG system moves into production.

---

## Readiness Domains

| Domain | Readiness Question |
|---|---|
| Source authority | Are retrieval sources approved and owned? |
| Data scope | Is the corpus limited to permitted data? |
| Freshness | How often is the index refreshed and validated? |
| Grounding | Does the system show source basis for important outputs? |
| Evaluation | Are answer quality, groundedness, refusal, and safety tested? |
| Access control | Does retrieval respect user permissions and data boundaries? |
| Monitoring | Are retrieval failures, low-confidence answers, and source drift observable? |
| Revalidation | What changes force re-review? |

---

## Minimum Production Evidence

- approved source list
- corpus owner
- indexing schedule
- access-control model
- groundedness evaluation
- hallucination testing
- refusal behavior testing
- user-permission enforcement
- telemetry plan
- incident response path
- revalidation triggers

---

## Refusal Conditions

A RAG system should not advance when:

- source authority is unclear
- sensitive data retrieval is uncontrolled
- grounding is not evaluated
- user permissions are not enforced
- hallucination/safety testing is absent
- production telemetry is missing
- index changes cannot trigger revalidation

---

## Operating Principle

RAG readiness is not only answer quality.

It is governed retrieval: source authority, data scope, access, evaluation, grounding, telemetry, and revalidation working together before generated output influences business consequence.
