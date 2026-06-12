# Control Plane Test Logic

## Purpose

This file documents the expected public-safe decision logic for the Elyria Enterprise AI Control Plane.

---

## Test Case 1: Customer Support Copilot

Input file:

```text
examples/customer-support-copilot.json
```

Expected outcome:

```text
ADMIT
```

Reason:

```text
The use case has assigned ownership, identity controls, data controls, RAG grounding evaluation, approval boundary, observability, and no revalidation requirement.
```

---

## Test Case 2: Agentic Workflow Risk

Input file:

```text
examples/agentic-workflow-risk.json
```

Expected outcome:

```text
REFUSE
```

Reason:

```text
The use case includes sensitive data without data controls and agentic tool use without an action boundary or required approval.
```

---

## Test Case 3: Missing Ownership

Expected outcome:

```text
HOLD
```

Reason:

```text
A production AI initiative cannot advance without business and technical ownership.
```

---

## Test Case 4: Changed Conditions

Expected outcome:

```text
REVALIDATE
```

Reason:

```text
Prior approval cannot be relied on when model, data, prompt, tool permissions, policy, owner, or production environment changes.
```
