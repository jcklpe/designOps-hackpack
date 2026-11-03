---
id: SELECT-WORKFLOWS
type: operational
scope: "Agent selection of maintenance workflow source and work records in this repository."
status: adopted
authority: "Aslan, explicit adoption in the active migration conversation, 2026-11-02. Aslan approved the shared-source consumer rollout (G8–G10) in the active audit conversation on 2026-11-03."
revised: "2026-11-03"
depends_on: ["ADOPT-POLICIES"]
related_to: []
---
# Select the pinned maintenance workflows
When explicitly developing DesignOps HackPack, this repository is the project root. Use its complete pinned [Project Workflows](../../project-workflows/README.md) collection and project configuration before global seeds. Read [docs/workflow.toml](../workflow.toml) and resolve `project.root` relative to that project-owned file. The child uses an exact detached shared-source pin; the parent gitlink records the accepted shared commit. Local project instructions take precedence.

This dependency governs package maintenance; it does not impose operating rules on projects consuming DesignOps resources. Keep actual maintainer work records in this repository and follow its existing index, spike, scratch and archive conventions through the selected skills. Create directories only when they have content. Preserve a dirty or active dependency checkout rather than overwriting it to restore a pin.

Active spike metadata `attention: live` marks a maintained record, not approval to implement every idea. Keep agreed direction, agent proposals, open questions and implementation evidence distinct. The project-owned agent-policy copies remain separate from the workflow distribution; a source update does not adopt or refresh them.
