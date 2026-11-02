---
id: SELECT-WORKFLOWS
type: operational
scope: "Agent selection of maintenance workflow source and work records in this repository."
status: adopted
authority: "Aslan, explicit adoption in the active migration conversation, 2026-11-02."
revised: "2026-11-02"
depends_on: ["ADOPT-POLICIES"]
related_to: []
---
# Select the pinned maintenance workflows
When explicitly developing DesignOps HackPack, this repository is the project root. Use its complete pinned [Project Workflows](../../project-workflows/README.md) collection and project configuration before global seeds. Resolve `project.root` relative to that collection's `workflow.toml`. The child branch is `project/designops-hackpack`; the parent gitlink records the exact adopted commit. Local project instructions take precedence.

This dependency governs package maintenance; it does not impose operating rules on projects consuming DesignOps resources. Keep actual maintainer work records in this repository and follow its existing index, spike, scratch and archive conventions through the selected skills. Create directories only when they have content. Preserve a dirty or active dependency checkout rather than overwriting it to restore a pin.

Active spike metadata `attention: live` marks a maintained record, not approval to implement every idea. Keep agreed direction, agent proposals, open questions and implementation evidence distinct. The project-owned agent-policy copies remain separate from the workflow distribution; a source update does not adopt or refresh them.
