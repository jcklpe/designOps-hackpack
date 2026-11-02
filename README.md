# DesignOps HackPack

Reusable DesignOps resources, being developed as an agent-aware skills-and-tools package. The repository holds both reusable material and documentation for maintaining the package; it does not require a separate development repository.

## Using the package
The available material includes example component specifications, token palettes, icon assets and a GitHub-based governance example. Select and adapt useful resources to your project. The governance example below is optional; cloning this repository does not adopt it as your team’s process. Keep your project’s actual work and private information in its own workspace.

An agentic skill/tool catalog is planned, not yet implemented. Package here describes the reusable repository’s role, not an existing package-manager release or installer.

## Developing the package
Start with [AGENTS.md](AGENTS.md), [TODO.md](TODO.md) and the [agent-aware DesignOps direction spike](docs/active-spikes/agent-aware-designops.md). Development records live in this repository’s `docs/`; their proposals and tasks apply to maintaining the toolkit, not to consumers using its resources. Maintenance uses the pinned [Project Workflows](project-workflows/README.md) collection on `project/designops-hackpack`. Its procedures govern development of this package; they do not automatically govern consumer projects.

The source repository is [jcklpe/designOps-hackpack](https://github.com/jcklpe/designOps-hackpack). Broader governance tooling and adoption into other projects remain future work.

## Join package development
Clone with submodules, or restore the recorded dependency in an existing checkout:

```sh
git clone --recurse-submodules https://github.com/jcklpe/designOps-hackpack.git
# In an existing checkout:
git submodule update --init --recursive -- project-workflows
```

Keep the exact recorded dependency revision. Read `AGENTS.md` before changing files. Skills can be used directly from their files; global registration and service authentication are separate, optional setup steps.

**Paste into your agent:**

```text
Help me get ready to contribute to this DesignOps HackPack repository. Read README.md and AGENTS.md, preserve existing work, and restore the pinned project-workflows submodule if needed. Read project-workflows/setup-project-workflows/SKILL.md and follow its collaborator onboarding procedure. Explain how to use the available maintenance skills without requiring global installation. Do not change pins, adopt governance in another project, publish, or enable forge automation as part of onboarding.
```

When starting a contribution, ask the agent to read `project-workflows/coordinate-project-contribution/SKILL.md`, agree on the requested scope, and use an agent-owned spike in this repository. Check relevant relative links, configuration and changed resources; no runtime tooling is required just to read or use the existing guidance.

## Design Tokens

Design tokens are standardized design elements that can be shared and reused across an organization's design system to provide consistent representation of design elements like color, typography, and spacing. Design tokens enable designers and developers to work with a consistent set of design elements, ensuring the design of a product is cohesive and consistent, and making it easier to update and maintain the design. They are a crucial part of a design system as they provide a shared language and guidelines for designers and developers to follow when creating user interfaces.

> If Components are the [atoms](https://bradfrost.com/blog/post/atomic-web-design/) of a design system, then design tokens are the sub-atomic particles.

![](https://specifyapp.com/_nuxt/img/button-component-design-tokens-anatomy-light.62d0c2c.jpg)

*(borrowed from [this article](https://specifyapp.com/blog/introduction-to-design-tokens))*

The essential structure is:

Product > Features > Interfaces > Components > Design Tokens

`Products` are composed of `Features`, `Features` are composed of `Interfaces`,`Interfaces` are composed of `Components`, `Components` are composed of `Design Tokens`.

Every value of every key-value pair in the JSON specs is a design token.

Recommended reading for design systems:

- [What are Design Tokens by CSS Tricks](https://css-tricks.com/what-are-design-tokens/)
- [What are Design Tokens by Specify App](https://specifyapp.com/blog/introduction-to-design-tokens)
- [Adobe's Design Token Page](https://spectrum.adobe.com/page/design-tokens/)

## Palettes

Palettes are collections of design token values that are used globally. The 4 palettes included in this repo as examples are:

### [Color](./component-specs/color-palette.json)

Probably the most well known sort of palette, this is how semantic UI, branding, dark mode alts, and theme colors are defined.

### [Type](./component-specs/type-palette.json)

Another common palette is the Type palette, which defines the semantic hierarchy expressed through type family, sizing, and weight.

### [Icon](./component-specs/icon-palette.json)

Defines the semantic hierarchy of iconography. Icons are stored as SVGs in the asset folder, and are referenced by the palette. You can use this git repo as a direct dependency for code that uses these SVGs.

### [Shape](./component-specs/icon-palette.json)

Shape covers general tokens like border radius, and layout stuff like margin and padding.

## Design System Governance
The Design System Governance is centered on the Product Team context in order to ground the work in the particular needs of the applications as they exist and are built. The purpose of this is to encourage an agile, iterative, collaborative, bottom-up organization of Design System standards rather than a slow top-down organization.

Governance isn't a hinderance to agility, it is the source of agility. Clear process benefits everyone.
```mermaid
graph TB
    subgraph Design System Working Group Context
        direction TB
        DESIGNIT--create-->NEW[/Document component needs <br/>and design in a git repo ticket/]
        NEW-->DISCUSS[Discuss new spec.]
        DISCUSS-->JSON[Write JSON Component specs]
        JSON-->PULL[Make pull request with proposed <br/> changes outlined in the JSON specs]
        PULL-->TEST{Test for consensus?}
        TEST--yes-->SPEC[Consensus achieved. <br/>Spec passes]
        TEST--no-->CONCERN{Raise concerns?}
        CONCERN--no-->ASIDE[Stand aside.]
        CONCERN--yes-->DISCUSS
        ASIDE-->SPEC


        DESIGNCHANGES-->PROPOSECHANGES[/Document proposed needs and design changes <br/> in git repo ticket./]
        PROPOSECHANGES-->DISCUSSEDIT[Discuss edits.]
        DISCUSSEDIT-->JSONEDIT[Edit existing <br/> JSON Component specs]
        JSONEDIT-->PULLEDIT[Make pull request with proposed changes <br/>outlined in the JSON specs]
        PULLEDIT-->TESTEDIT{Test for consensus?}
        TESTEDIT--yes-->SPEC[Consensus achieved. <br/>Spec passes]
        TESTEDIT--no-->CONCERNEDIT{Raise concerns?}
        CONCERNEDIT--no-->ASIDEEDIT[Stand aside.]
        CONCERNEDIT--yes-->DISCUSSEDIT
        ASIDEEDIT-->SPEC
    end

    subgraph Product Team Context
        direction TB
        START([design needed]) --> EXIST{Does the component style or <br/>pattern exist in <br/>the design system?}
        EXIST--yes--> CHANGES{Does the component need <br/>any changes to fit a new use case?}
        EXIST--no--> DESIGNIT[ Design component as you need for your product team context.]
        CHANGES--no--> END([Design app according to established spec])
        CHANGES--yes--> DESIGNCHANGES[Create a variant of the component<br/> according to the necessary changes<br/> needed in your product line ]
    SPEC-->END
    end


```

The Design System Governance work can be aided by the [Github issue templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates) found in this repo. See some examples of this with [this discussion ticket](https://github.com/jcklpe/design-ops-hackpack/issues/2), and this [pull request](https://github.com/jcklpe/design-ops-hackpack/pull/3).

### Bar for Consensus

You can adopt your own system for defining how a spec passes but for the sake of simplicity this repo assumes that a [consensus](https://en.wikipedia.org/wiki/Consensus_decision-making) method is used.

## Design Systems are not Component Libraries or UI Kits

Something important to understand is that a Design System is bigger than a single implementation.

![](https://specifyapp.com/_nuxt/img/how-design-decisions-are-applied-light.2053128.jpg)

*(borrowed from [this article](https://specifyapp.com/blog/introduction-to-design-tokens))*

Design Systems are bigger than just the code libraries or the Figma/Sketch/Penpot UI Kits that implement them. The Design System is the social construction that designers, devs, content creators, product, and stakeholders use to communicate and build consensus on how work gets done.
