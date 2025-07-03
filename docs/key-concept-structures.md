---
layout: default
---
# Key Concept Structures (LinkML & Other Models)

CKP governs shared meaning through well-structured schemas. Each concept, class, attribute, or relationship is both defined for reuse and made governable by agentic processes.

**CKP schemas and plug-in mechanisms are intentionally designed for interoperability and extensibility. Through the CKP extension model, developers can augment MCP agents with new “senses,” skills, or data sources, seamlessly knitting together capabilities from CKP, MCP, AAP, and beyond.**

## Theory

- **Concept types:** Core elements include classes, properties, and relationships, modelled for clarity and extensibility.
- **Schema modeling:** CKP draws upon LinkML (YAML/JSON-LD) for formalized, machine-actionable concept definitions, but remains flexible for new paradigms, agent senses, and cross-protocol plugins.
- **Governable objects:** Each schema or data type is subject to proposal, validation, and audit by subordinate agents; logs retain all changes for transparency.

*From algorithm ([agentic_concept_governance.py](../ingest_only_do_not_link/agentic_concept_governance.py)):
- Agents are instantiated per concept for localized governance — every data structure has an owner and validator.*
- Community review and consensus can refine or extend structures over time.

*To enable new abilities or senses in MCP agents, simply propose a new extension schema—CKP ensures these additions are subject to the same robust governance as core concepts.*

## Example

```yaml
# Example: Concept schema snippet using LinkML
name: ExampleConcept
attributes:
  confidence:
    range: float
```

_Agent groups will instantiate and supervise the evolution of each such concept or extension._

[Back to Home](index.md)