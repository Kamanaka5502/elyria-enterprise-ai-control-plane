# Demo Script

## Purpose

This script supports a 10-minute executive or hiring-panel walkthrough of the Elyria Enterprise AI Control Plane.

---

## Opening

```text
This repository shows how I approach enterprise AI governance as architecture, not as policy language alone.

The problem is that AI systems now move through organizations as copilots, RAG assistants, agents, automations, model integrations, and AI-assisted development. The enterprise needs a repeatable way to decide what can advance, what must pause, what must stop, and what must be revalidated before production consequence occurs.
```

---

## Step 1: Show the Control Plane

Point to the README and explain:

```text
The core model is ADMIT / HOLD / REFUSE / REVALIDATE.

That gives business, technical, security, privacy, data, and AI teams a shared decision language.
```

---

## Step 2: Show the Enterprise Architecture

Open:

```text
docs/reference-architecture.md
```

Explain:

```text
This is the target-state architecture path: use-case intake, classification, data scope, authority, model/RAG/agent controls, evaluation, readiness, deployment, telemetry, and revalidation.
```

---

## Step 3: Show Agentic Governance

Open:

```text
docs/agentic-systems-control-model.md
```

Explain:

```text
Agents are not governed by prompt instructions alone. They require tool boundaries, approval paths, authority checks, logging, escalation, and revalidation.
```

---

## Step 4: Show RAG Readiness

Open:

```text
docs/rag-production-readiness.md
```

Explain:

```text
RAG readiness is not just answer quality. It is source authority, data scope, access control, grounding, evaluation, telemetry, and revalidation.
```

---

## Step 5: Show the Sandbox

Open:

```text
sandbox/deployment-playground.md
sandbox/sample-scenarios.md
```

Explain:

```text
The sandbox demonstrates how an enterprise can evaluate AI movement before production advancement and convert the result into a pilot-corridor backlog.
```

---

## Step 6: Close with Enterprise Value

```text
The value is faster AI adoption with stronger control. This gives enterprises a reusable architecture pattern for responsible AI, Azure alignment, agentic systems, data governance, production readiness, and executive decision-making.
```
