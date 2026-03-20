# Global Context Loader

This file defines the minimum context that every Deliveri Operations Team agent must load before performing meaningful work.

Its purpose is to ensure consistent reasoning, reduce duplicated mistakes, preserve departmental knowledge, and ground all work in Deliveri-specific context.

This loader is mandatory for all agents unless a task is explicitly trivial.

---

## Purpose

Before doing work, agents must load the right context in the right order.

This prevents agents from:
- answering without institutional knowledge
- repeating mistakes
- ignoring recent learnings
- drifting away from Deliveri-specific realities
- inventing workflows that conflict with existing practice

---

## Required Load Order

Before beginning meaningful work, every agent must load context in this order:

1. the orchestrator
2. the department memory
3. the department learnings
4. the relevant Deliveri company knowledge
5. any task-specific directives, workflows, or tools
6. any relevant cross-department memory if needed

---

## Step 1 — Load the Orchestrator

Read:

- `deliveri/orchestrator.md`

Purpose:
- understand routing rules
- understand department ownership
- understand memory and learnings expectations
- understand when to use other agents or deterministic tools

---

## Step 2 — Load Department Memory

Read:

- `deliveri/<department>/memory.md`

Purpose:
- understand the department’s reusable knowledge
- reuse prior frameworks, templates, decisions, and proven approaches
- avoid solving known problems from scratch

---

## Step 3 — Load Department Learnings

Read:

- `deliveri/<department>/learnings.md`

Minimum required sections:

1. **Most Recent Learnings**
2. **Current Best Practices**

Read deeper sections only if needed:
- Known Constraints
- Common Mistakes to Avoid
- Historical Learnings Archive

Purpose:
- absorb the newest insights quickly
- align with current departmental best practices
- avoid repeating known mistakes

---

## Step 4 — Load Deliveri Company Knowledge

Read only the files relevant to the task under:

- `deliveri/knowledge/company/`

Examples:
- `overview.md`
- `business_model.md`
- `customers.md`
- `value_proposition.md`
- `brand.md`
- `operations.md`
- `tools_systems.md`
- `learnings.md`

Purpose:
- ground work in Deliveri’s actual business
- align outputs with Deliveri’s customers, positioning, tools, and constraints
- avoid generic or company-agnostic answers

---

## Step 5 — Load Task-Specific Directives, Workflows, and Tools

Read any relevant:
- directives
- SOPs
- execution tools
- scripts
- workflows
- templates

Purpose:
- ensure the task follows the current system
- prefer existing processes over improvisation
- use deterministic tools when available

---

## Step 6 — Load Cross-Department Context Only When Necessary

If the task is cross-functional, read the relevant memory and learnings from other departments.

Examples:
- Sales may read Marketing
- Operations may read Finance
- Support may read Product
- Integrations may read Operations

Rules:
1. always load your own department first
2. only load other departments when the task requires it
3. avoid unnecessary context loading

---

## Trivial Task Exception

This loader may be partially skipped only for trivial tasks such as:
- formatting changes
- simple rewrites
- obvious file moves
- direct user formatting requests

If the task involves:
- strategy
- recommendations
- decisions
- planning
- customer guidance
- process design
- department knowledge
- company-specific reasoning

then the full loader must be used.

---

## Post-Work Requirement

After meaningful work is completed, the responsible agent must evaluate whether the task produced:

1. reusable departmental knowledge
2. new departmental learnings
3. updated Deliveri company knowledge

If yes, the agent must update the correct file(s).

---

## Enforcement Rule

No agent should begin meaningful work without loading:

- `deliveri/orchestrator.md`
- `deliveri/<department>/memory.md`
- `deliveri/<department>/learnings.md`
- relevant files under `deliveri/knowledge/company/`

This loader is mandatory for all Deliveri Operations Team agents.

---

## Summary

Every meaningful task should follow this context chain:

orchestrator  
→ department memory  
→ department learnings  
→ Deliveri company knowledge  
→ task-specific directives and tools  
→ optional cross-department context

This ensures every agent works with:
- the latest departmental context
- the latest company context
- the right operating rules
- the best available institutional knowledge

The goal is not just correctness in the current task.

The goal is cumulative intelligence over time.
