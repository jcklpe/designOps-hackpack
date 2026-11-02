---
status: parked
---
# Agentic DesignOps evolution
Captured from the maintainer’s wireframing and toolkit-architecture discussion on 2026-11-01. This is context for future bounded spikes, not an implementation backlog or adopted team-governance process. Package setup is tracked in the [direction spike](../active-spikes/agent-aware-designops.md).

## Package direction
DesignOps HackPack is a reusable package containing its own development process and records. It may distribute templates without turning its checkout into a consumer’s project. The maintainer chose this approach for DesignOps; a possible ResearchOps migration remains a separate parked decision. Package-maintenance procedures, consumer capabilities and a consumer’s own governance need distinct instructions.

## Start from actual collaboration
A design system includes the social arrangements through which people make and maintain design decisions. Its component library, tokens, documents and automation are artifacts of that process. Writing a policy or consolidating a library does not establish that people agree with it or use it.

The prospective use case has informal collaboration. Explore assistance that makes existing practice legible before prescribing committees, formal consensus or pull requests. Useful distinctions include what is agreed, by whom and within what scope; what is implemented; where divergence exists; and what requires a human conversation. Avoid status labels such as “current” or “checked” that imply more agreement or evidence than exists.

Agents participate by interpreting, proposing, challenging and executing within delegated scope. Their contribution is mediated by the human directing the work and differs from that of another human stakeholder. Preserve this collaborative relationship without manufacturing agreement on behalf of others. These operational distinctions do not depend on claims about subjective experience.

## Candidate areas for future skills
- Help articulate an existing design practice and its actual decision participants without turning a descriptive account into a newly adopted policy.
- Prepare a shared-component change for discussion, including need, affected consumers, alternatives, exceptions and migration implications.
- Track an agreed decision through its artifacts and verification while leaving disagreement or incomplete adoption visible.
- Help retire or replace components with historical dependencies and ownership boundaries accounted for.
- Surface where collaborators need to talk, while avoiding automatic messages, assignments or adjudication by the agent.

These are candidates, not a committed skill catalog. Choose one concrete recurring problem before building tools or introducing more ceremony.

## Boundaries and integration
Wireframe Workflows owns prototype operation, exploration, migration and verification under a project’s existing authority. DesignOps can address the shared agreements around that work without becoming a prerequisite for routine wireframing. Project Workflows supplies work records and contribution coordination; Agent Hands or another connector supplies service operations. None supplies permission merely by being installed.

Inspect Project Workflows’ evolving GitHub collaboration support before inventing another tracking mechanism. A GitHub issue, discussion or pull request may provide useful evidence and review surfaces; it need not become a required format for every design decision. Keep local and non-GitHub use viable. Human judgment about design acceptance remains distinct from technical review or merge permission.

## Existing material and token tooling
Assess the current JSON component specifications, palettes and Product → Features → Interfaces → Components → Tokens model against actual needs. The existing issue/PR/consensus diagram is an optional example, not the universal future process.

The maintainer flagged Style Dictionary and automated token synchronization as possible sources of overlap or supersession. Compare schemas, source ownership, transformations, aliases and supported integrations before deciding what to keep, replace or delegate. No obsolescence or compatibility conclusion has been established yet. Do not rebuild token tooling merely to give the package more tools.

## Questions for a future spike
How should an adopter select relevant procedures without treating the entire package as authority? What is the smallest useful decision record? How should acceptance, implementation and verification be linked without being conflated? Which coordination work belongs in shared project tooling, and which needs DesignOps-specific interpretation? What would demonstrate that an agent-assisted process helps the people involved rather than only producing more documentation?
