# 13 — IT

> Part of the **Kojiki Decision System**. This repo is the
> **IT** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/robfuj/kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> How do we keep technology reliable, secure, and effective for the organization?

## Purpose
Ensure employees and functions have reliable, secure, effective technology.

## Sub-functions
IT Operations, Service Desk, Infrastructure, End-User Computing, Identity & Access, IT Governance, Automation/Consolidation

## Typical roles
CIO, VP IT, IT Director, IT Manager, Systems Administrator, Service Desk Lead, IT Operations Engineer

## Inputs
Systems, users, incidents, access requests, availability, cost, utilization.

## Outputs
Reliable systems, resolved incidents, access provisioning, technology roadmap.

## Learning focus
Recurring incidents; technology bottlenecks; adoption patterns; unnecessary systems; access risks; automation/consolidation opportunities.

## Operating tree
```text
ASSET →
    USERS →
    INCIDENT →
    ROOT CAUSE →
    OPTIONS →
    TRADEOFFS →
    DECISION →
    IMPLEMENTATION →
    VERIFICATION →
    MONITORING →
    LEARNING
```

## Decision states
```text
INVENTORIED → MONITORING → INCIDENT → ROOT-CAUSED → DECIDING → IMPLEMENTING → VERIFYING → RECOVERING → LEARNED
```

## Decision outputs
`Maintain · Automate · Consolidate · Remediate · Escalate · Monitor`

## Critical prompts (what this function thinks about)
> What systems serve this function?
> Who depends on them?
> What incidents recur?
> What is the user impact?
> What is the cost of downtime?
> What access risks exist?
> What can be automated?
> What should be consolidated?
> What controls are missing?
> What evidence proves reliability?
> What changed after the incident?
> What should be tested?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/13-it.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
