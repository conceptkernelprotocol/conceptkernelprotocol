---
layout: default
---
# Protocol Actors: Agents, Guardians, Participants

CKP’s ecosystem relies on distinct yet overlapping roles for meaningful governance. Each role plays a part in robust decision-making, semantic alignment, and continuous system improvement.

## Theory

- **Agent:** Software entity (or human proxy) that can propose new concepts, validate others’ work, and vote on changes. Realized in the agentic governance algorithm as a `ConceptAgent`—each concept gets its own.
- **Guardian:** Maintainer of semantic or operational integrity; reviews proposals for compliance and monitors logs/audits. Can be implemented as a class or as privileged actors/rulesets.
- **Participant:** Broader set of contributors who engage in proposal, discussion, and voting, influencing consensus and system evolution.

Agents and guardians work as subordinates to an orchestrator (see [Agentic Governance Lifecycle](agentic-governance-lifecycle.md)), collaborating to steer concept evolution.

## Practical Interaction Example

| Role        | Core Responsibility                                                 |
|-------------|---------------------------------------------------------------------|
| Agent       | Proposes/validates concepts, casts votes, logs actions              |
| Guardian    | Ensures protocol integrity, audits processes, may have veto rights  |
| Participant | Engages in consensus, proposes and discusses improvements           |

**In code:**  
- Agent instances created per schema (see [agentic_concept_governance.py](../ingest_only_do_not_link/agentic_concept_governance.py))
- Orchestrators manage coordination across agents.

[Back to Home](index.md)