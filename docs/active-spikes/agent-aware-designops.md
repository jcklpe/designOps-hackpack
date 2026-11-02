---
attention: live
---
# Agent-aware DesignOps direction
Owner: the agent thread preparing the connected Workshop policy and repair/audit skills. Opened 2026-11-01. This bounded spike establishes package-local development records and captures direction for later work; implementing a governance toolkit is outside its present scope.

## Package structure and domain boundary
Wireframe work exposed questions about component ownership, agreement, lifecycle and shared standards. The maintainer wants a clean boundary: everyday wireframe operation should not acquire a mandatory governance process. DesignOps can address the broader human agreements separately and connect to the operational tools when there is a concrete need.

DesignOps HackPack is being developed as a reusable package. Its maintainer guidance, development index, spikes and future scratch/archive records live alongside reusable resources in this repository. Consumer projects remain separate, and the package’s development proposals do not become their operating rules. No separate `designOps-dev` repository or DesignOps adoption in agentic-wiki is required by this arrangement.

The package can contain templates without itself being the template for every consumer’s project. Development documentation placement and workflow availability are separate decisions. Maintenance adopts a pinned Project Workflows collection on `project/designops-hackpack`. This does not make its procedures requirements for consumers using DesignOps resources.

## Direction agreed for future work
- Move toward a skills-and-tools-first toolkit that is useful with agents, rather than automatically treating the existing template and formal governance example as the future product.
- Describe actual collaboration before prescribing a process. The initial prospective adopter has informal coordination; a published policy, library or status label does not establish shared adoption.
- Keep processes proportionate to the people and work. A design contribution need not require a pull request, committee or formal consensus ritual. The existing HackPack example can remain a selectable reference.
- Preserve the distinction between a design system as a social arrangement and its artifacts: component libraries, token data, specifications and automation.
- Agents can interpret, propose, challenge and execute within delegated scope. Their participation affects the collaboration, while human agreement and stakeholder authority cannot be manufactured by an agent consolidating components or relabeling work as current. This distinction does not depend on claims about subjective experience.
- Keep agreed design, implemented behavior, divergence and questions requiring conversation legible. Record who agreed to what scope when that information is known; do not invent approval or equate technical validation with social agreement.

## Boundaries with neighboring work
| Owner | Responsibility |
| --- | --- |
| Wireframe Workflows | Connected prototypes, exploration, naming, component dependencies and migrations, checks, merge and promotion under the project's existing authority |
| DesignOps HackPack | Future assistance for understanding and negotiating design practices, shared standards, exceptions and participation; exact skills and scope remain open |
| Project Workflows | Work records, agent-owned spikes, contributions, review and delivery under human direction; local use or explicitly selected forge coordination |
| Agent Hands and other connectors | Service access and execution mechanics; availability does not grant authority |
| Adopting project | Its actual people, permissions, agreements and chosen procedures |

Routine component lifecycle work remains possible without a formal governance layer. For example, checking a replacement's consumers and verifying an authorized migration is wireframe operation. Deciding who may redefine a shared component or how disagreement is resolved depends on the project's agreements.

## Existing HackPack baseline
Inspected source: `353eb18f6f025eb94d56fd87692a22ce1e2beed8` from [designOps-hackpack](https://github.com/jcklpe/designOps-hackpack). Its README describes Product → Features → Interfaces → Components → Design Tokens, JSON specifications and palettes, and a product-team-driven example using issues, discussion, pull requests and consensus. It contains example component specifications, icon assets and issue templates. The README already distinguishes a design system from a component library. This identifies the inspected baseline, not the current uncommitted documentation changes. The existing example specifications, assets and governance example have been retained.

Do not assume that all existing conventions should survive, or that they are all obsolete. The maintainer flagged possible overlap with Style Dictionary and token synchronization work. A future assessment should compare the actual schemas, transformations, source-of-truth decisions and supported tool capabilities before retaining or replacing anything. No compatibility or obsolescence claim has been validated in this setup spike.

## Future direction
The [agentic DesignOps evolution note](../scratch/agentic-designops-evolution.md) preserves candidate skills, collaboration questions and token-tooling assessment for later bounded work. These topics remain parked; this setup does not implement governance or change a consuming project’s procedures.

## References and resume points
- [DesignOps HackPack](../../README.md): package entrypoint, available material and maintenance routing.
- [Why Design Systems are not Component Libraries](https://aslanfrench.medium.com/why-design-systems-are-not-component-libraries-1e44ee417e58): conceptual framing supplied by the maintainer; the conversation used an author-supplied copy. It is not a template adoption decision.
- [ResearchOps Development](https://github.com/jcklpe/researchOps-dev): repository-boundary precedent, not a requirement to copy all of its setup.
- [Project Workflows contribution coordination](https://github.com/jcklpe/project-workflows/blob/main/coordinate-project-contribution/SKILL.md): inspect the current published revision when resuming; it separates project decisions from service mechanics and supports local coordination.
- [Wireframe Workflows](https://github.com/jcklpe/wireframe-workflows): operational neighbor; policy/repair work is handled separately and does not establish a governance dependency.

## Repository arrangement decision
On 2026-11-01 the maintainer chose to try the package approach for DesignOps, retaining `designOps-hackpack` naming and keeping its process and development documentation in the same repository. ResearchOps’s possible migration remains parked in its own maintainer workspace; this decision does not reorganize other collections.

The provisional local `designOps-dev` wrapper had no commits or remote. Its spike records were preserved and reconciled into this package, and the existing HackPack checkout retained its Git history and upstream. A recovery copy of the provisional wrapper was kept outside the active workspace. The maintainer subsequently authorized Project Workflows adoption and publication of the package setup.

## Next review boundary
Review the captured direction and package entrypoints. A later workstream should choose one concrete collaboration problem and inspect neighboring capabilities before defining skills or tooling. The current checkpoint includes the authorized Project Workflows adoption and publication. Broader governance implementation, license review and consuming-project integration remain future choices.
