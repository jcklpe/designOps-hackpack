# Agent instructions
This repository owns the reusable DesignOps HackPack and its development documentation. Start with the [README](README.md) for available resources and package-development context.

## Agent policy routing
Read the project-owned [agent policy index](docs/agent-policies/policy.index.md) for scopes and operative status. Load applicable adopted policies with their complete prerequisite closure before acting. For policy management, load ADOPT-POLICIES, PRESERVE-IDENTITY and RESOLVE-DEPENDENCIES, then use the selected task procedure below. Policy source updates and structural checks do not establish adoption.

## Maintenance procedures
The selected collection is [Project Workflows](project-workflows/README.md). Read its [project configuration](project-workflows/workflow.toml) and resolve `project.root` relative to that collection. [SELECT-WORKFLOWS](docs/agent-policies/SELECT-WORKFLOWS-use-the-pinned-maintenance-source.md) owns workflow-source selection; [MAINTAIN-PACKAGE](docs/agent-policies/MAINTAIN-PACKAGE-maintain-package-and-consumer-boundaries.md) owns package and consumer boundaries.

`TODO.md` indexes development work. Use [Run Project Spike](project-workflows/run-project-spike/SKILL.md) for conceptual and `.todo.md` pairs in `docs/active-spikes/`, [Capture for Later](project-workflows/capture-for-later/SKILL.md) for individual parked subjects in `docs/scratch/`, and `docs/archive/` for authorized closure history.

Restore the recorded submodule with `git submodule update --init --recursive -- project-workflows` when needed; preserve an already dirty or active checkout. Use [Setup Project Workflows](project-workflows/setup-project-workflows/SKILL.md) for collaborator onboarding and [Update Project Workflows](project-workflows/update-project-workflows/SKILL.md) for ancestry-aware upgrades.

Use the selected [Create](project-workflows/create-agent-policy/SKILL.md), [Edit](project-workflows/edit-agent-policy/SKILL.md), [Review](project-workflows/review-agent-policies/SKILL.md), [Adopt](project-workflows/adopt-agent-policies/SKILL.md) and [Retire](project-workflows/retire-agent-policy/SKILL.md) procedures for policy work.

## Contribution and checkpoints
Use [Coordinate Project Contribution](project-workflows/coordinate-project-contribution/SKILL.md) for human-directed scope, separate agent-owned spikes and reviewable contributions. Use [Commit Work](project-workflows/commit-work/SKILL.md) for scoped checkpoints when authorized. [HONOR-AUTHORITY](docs/agent-policies/HONOR-AUTHORITY-respect-coordination-and-checkpoint-permissions.md) owns action and checkpoint authority; [PRESERVE-WORK](docs/agent-policies/PRESERVE-WORK-preserve-concurrent-edits-and-design-evidence.md) owns concurrent-work, content and validation safeguards.
