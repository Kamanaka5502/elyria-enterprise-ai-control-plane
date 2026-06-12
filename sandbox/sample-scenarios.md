# Sandbox Sample Scenarios

## Scenario 1: Customer Support Copilot

**Stage:** Pilot  
**System type:** RAG-assisted internal copilot  
**Data:** Internal knowledge base  
**Agentic action:** No protected external action  
**Controls:** Ownership, identity, data controls, grounding evaluation, approval, observability

Expected outcome:

```text
ADMIT
```

Why:

```text
The system has ownership, bounded data scope, identity controls, grounding evaluation, human review, and observability.
```

---

## Scenario 2: Agentic Workflow With External Tool Action

**Stage:** Production candidate  
**System type:** Agentic workflow automation  
**Data:** Confidential account data  
**Agentic action:** Operational workflow update  
**Controls missing:** Data controls, grounding evaluation, action boundary, human approval

Expected outcome:

```text
REFUSE
```

Why:

```text
The workflow can bind protected action while sensitive data controls and action boundaries are missing.
```

---

## Scenario 3: RAG Knowledge Assistant With Missing Evaluation

**Stage:** Pilot  
**System type:** RAG assistant  
**Data:** Internal documentation  
**Controls missing:** Grounding evaluation

Expected outcome:

```text
HOLD
```

Why:

```text
The system is not structurally refused, but it lacks evidence that generated answers are grounded in approved sources.
```

---

## Scenario 4: Previously Approved Copilot With Changed Data Scope

**Stage:** Production  
**System type:** Copilot extension  
**Change:** New confidential data source added  
**Controls missing:** Updated review

Expected outcome:

```text
REVALIDATE
```

Why:

```text
Prior approval cannot be relied on when data scope changes.
```

---

## Demo Close

Each scenario demonstrates a different governance posture:

```text
ADMIT      Ready to advance.
HOLD       Not ready yet.
REFUSE     Blocked due to missing critical boundary.
REVALIDATE Changed conditions invalidate prior approval.
```
