# Department Memory Protocol

This protocol defines how all Deliveri Operations Team agents must read from and write to departmental memory.

Its purpose is to ensure that departmental knowledge becomes cumulative, reusable, and progressively stronger over time.

All agents must follow this protocol when working inside any department.

---

## Purpose

Department memory exists so agents do not repeatedly solve the same problems from scratch.

Department learnings exist so agents can quickly absorb the newest insights, avoid repeated mistakes, and apply the current best practices of their department.

Together, these files create a durable departmental intelligence layer.

---

## Required Department Files

Each department must maintain these files:

- `deliveri/<department>/memory.md`
- `deliveri/<department>/learnings.md`

Optional supporting files may be added later, but these two are the minimum required files for every department.

---

## Required Read Order Before Work

Before performing any meaningful task, the responsible agent must read these files in this order:

1. `deliveri/<department>/memory.md`
2. `deliveri/<department>/learnings.md`
   - first read **Most Recent Learnings**
   - then read **Current Best Practices**
3. relevant files in `deliveri/knowledge/company/` if company context is needed
4. any relevant directive, workflow, or execution tool instructions

Agents may read other departmental memory or learnings files if the task requires cross-functional context, but they must begin with their own department.

---

## When Memory Must Be Updated

After completing work, agents must update `memory.md` when the output creates reusable departmental value.

Examples of reusable value:

- new frameworks
- improved workflows
- reusable messaging
- templates
- checklists
- research summaries
- playbooks
- proven strategies
- important examples of strong work
- key decisions worth preserving

Do not add every minor task to memory. Only add content that improves future work.

---

## When Learnings Must Be Updated

After completing work, agents must update `learnings.md` whenever they discover something that future agents should know.

Examples:

- newly discovered constraint
- improved approach
- common failure mode
- updated preference
- pattern that consistently works
- strategy that should be avoided
- operational or tooling limitation
- new best practice

If the work produced no meaningful new insight, do not add noise. Learnings should stay useful and concise.

---

## How to Write to memory.md

When updating memory:

1. place information into the correct section
2. write clearly and concisely
3. prefer durable knowledge over temporary notes
4. summarize long outputs instead of dumping raw text
5. include references to related files when helpful
6. preserve readability for future agents

Memory should act as a department handbook, not a transcript log.

---

## How to Write to learnings.md

When updating learnings:

1. add the newest learning to the top of **Most Recent Learnings**
2. include:
   - date
   - agent name or role
   - what was learned
   - why it matters
3. update **Current Best Practices** if the new learning changes how the department should operate
4. move older learnings into **Historical Learnings Archive** over time
5. avoid duplicating content already stored in memory unless the insight is time-sensitive or newly discovered

Learnings should optimize for fast reading and progressive disclosure.

---

## Progressive Disclosure Rule

All departmental learnings files must support quick loading.

Each `learnings.md` file must contain these sections:

1. **Most Recent Learnings**
2. **Current Best Practices**
3. **Known Constraints**
4. **Common Mistakes to Avoid**
5. **Historical Learnings Archive**

Agents must read the first two sections before starting work.
They should read deeper sections only when the task requires more context.

---

## Cross-Department Access Rule

Agents may consult other departments when needed.

Examples:

- Sales may consult Marketing for positioning context
- Operations may consult Finance for refund policy context
- Support may consult Product for feature behavior context

When doing cross-department work:

1. read your own department first
2. read only the relevant sections of the other department
3. store final reusable output in the lead department's memory
4. update supporting departments only if the work changes their best practices too

---

## Deliveri Company Knowledge Rule

If the task depends on Deliveri business context, agents must also read the relevant files under:

- `deliveri/knowledge/company/`

Examples:

- `overview.md`
- `business_model.md`
- `customers.md`
- `value_proposition.md`
- `brand.md`
- `operations.md`
- `tools_systems.md`

Department memory does not replace company knowledge. Both may be required.

---

## Quality Standard

Memory and learnings updates must be:

- concise
- useful
- reusable
- department-specific
- easy for future agents to scan quickly

Do not write vague summaries.
Do not write redundant notes.
Do not store low-value noise.

---

## Enforcement Rule

No agent should begin meaningful work without first consulting:

- departmental memory
- departmental learnings
- relevant Deliveri company knowledge

No agent should complete meaningful work without considering whether:

- reusable knowledge belongs in memory
- new insight belongs in learnings

This protocol is mandatory for all Deliveri Operations Team agents.
