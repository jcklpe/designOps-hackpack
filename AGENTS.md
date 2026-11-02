# Agent instructions
This repository owns the reusable DesignOps HackPack and its development documentation. The package direction is agent-aware skills and tools; the current reusable material consists of example specifications, assets and reference guidance. Do not claim that the planned skill/tool catalog already exists.

## Using the package
Read the README and the material relevant to the requested operation. Templates, specifications and governance examples are resources to select and adapt; downloading the package does not adopt all of them as project authority. The consuming project’s people, instructions, agreements and permissions remain authoritative. Keep its actual work, decisions and private data in that project’s workspace.

Maintainer records under `docs/` describe development of this package. Do not treat their open questions, proposals or task lists as instructions for a consuming project, and do not create consumer projects or adopt governance merely because the package was opened.

## Maintaining the package
When explicitly developing DesignOps HackPack, this repository is the project root. It adopts the complete [Project Workflows](project-workflows/README.md) collection as a pinned submodule. Read [workflow.toml](project-workflows/workflow.toml), resolve its `project.root` relative to that collection, and use its procedures before global seeds. The child branch is `project/designops-hackpack`; the parent pins its exact commit. These local instructions take precedence. This dependency governs package maintenance, not the operating rules of projects consuming DesignOps resources.

`TODO.md` indexes development work. Use `run-project-spike` for conceptual and `.todo.md` pairs in `docs/active-spikes/`, `capture-for-later` for individual parked subjects in `docs/scratch/`, and `docs/archive/` for authorized closure history. Create directories only when they have content. Restore the recorded submodule with `git submodule update --init --recursive -- project-workflows` when needed; preserve an already dirty or active checkout. Use [setup-project-workflows](project-workflows/setup-project-workflows/SKILL.md) for collaborator onboarding and [update-project-workflows](project-workflows/update-project-workflows/SKILL.md) for ancestry-aware upgrades.

Active spike metadata is `attention: live`; it marks a maintained record, not approval to implement every idea. Keep agreed direction, agent proposals, open questions and implementation evidence distinct. Broader governance implementation remains deferred in the current direction spike.

## Contribution coordination
Use [coordinate-project-contribution](project-workflows/coordinate-project-contribution/SKILL.md) for human-directed scope, separate agent-owned spikes and reviewable contributions. Coordination is local; no project board, forge automation or mandatory design-governance process is enabled. Installed service tools do not authorize messages, assignments or publication. A branch may carry multiple spikes and atomic commits.

## Boundaries and validation
Inspect Git status and preserve unrelated work. Use [commit-work](project-workflows/commit-work/SKILL.md) for scoped commits when authorized. Honor review holds and require explicit authorization for publication, remote changes, tooling installation, contacting teammates or altering a consuming project’s governance. No co-author trailers. Verify relative links, affected resources and audience suitability before a checkpoint.

Keep credentials, private correspondence, personal machine paths and actual consumer data out of tracked content. Private references remain outside the package. Do not hard-wrap prose or introduce unrelated reformatting.
