# World Domination Software — Projects Repository Guidelines

## Repository Role

- This repository (`World-Domination-Software/Projects`) is the **customer-facing hub** for all WDS projects (games, tools, hosting, and related products).
- It centralizes:
  - Application-specific documentation under `docs/applications/`
  - Future project ideas and feature proposals (Discussions → Ideas category)
  - Bug reports, incidents, and support tickets (Issues)
  - General project discussions and community feedback (Discussions)
- The public website repository (`WDS_Website`) links to this repo from its `projects.php` page for all detailed project information and customer interaction.

## Terminology

**"wiki" in this repository refers only to the actual GitHub Wiki** at:
`https://github.com/World-Domination-Software/Projects/wiki`

Do **not** refer to files under `docs/` as "wiki". Do **not** create a top-level `wiki/` folder in the code repository. Any previously existing `wiki/` folder has been replaced with a stub.

## Documentation Structure

### docs/ — Application-specific documentation only

```
docs/
  README.md       – Overview of the docs/ folder and its structure.
  INDEX.md        – Table of all applications with links.
  applications/
    <app-name>/
      README.md             – Landing page; links to sub-docs and public resources.
      Overview.md           – What the application is, features, and architecture.
      Getting-Started.md    – Installation and first-use guide.
      Implementation-Notes.md – Architecture, components, and development status.
      Gameplay.md           – (Games only) Game modes, controls, and progression.
```

**Rules for docs/:**
1. `docs/` contains **application-specific documentation only**.
2. Shared/general pages — FAQ, support, bug reporting, roadmap, shared troubleshooting — must **not** live in `docs/` unless they are app-specific.
3. Every application gets its own subfolder under `docs/applications/`.
4. Every application folder must contain a `README.md` as its landing page.
5. Folder names must be **lowercase dash-separated** (e.g., `hostile-planets`, `game-servers-panel`).

### GitHub Wiki — Shared and public-facing documentation

The **actual GitHub Wiki** at `https://github.com/World-Domination-Software/Projects/wiki` is the public/shared documentation layer for:
- FAQ
- Shared troubleshooting
- Bug reporting guidance
- Support guidance
- Roadmap
- Community and discussions guides

Do not duplicate shared content between `docs/` and the GitHub Wiki.

## How This Repo Interacts With Others

- **WDS_Website**
  - Lists projects and shows short summaries only.
  - Each project row links here for app docs, discussions, and issue reporting.
  - Changes to project naming, categories, or status here should be reflected in the website's project list (and vice versa) so they stay in sync.

- **GSP / Agents and Other Service Repos**
  - Game server panel and agent repos are internal implementation details.
  - Customer-facing documentation, roadmaps, and issue tracking for those services should live **in this repo** (`docs/applications/`, Issues, Discussions), then link out to the underlying technical repos when necessary.

## Guidance for AIs Working in This Repo

- Treat this repo as the **source of truth for customer-visible project information and planning**.
- When adding or modifying structures (labels, discussion categories, issue templates, documentation):
  - Keep terminology consistent with what the WDS website uses for project names and categories.
  - Prefer adding new templates/structures over breaking existing ones that might already be in use.
- Do **not** move long-form documentation back into the website codebase; the website should point here instead.
- When suggesting or generating new content (issue templates, discussion prompts, documentation), make it:
  - Professional, clear, and accessible (non-hyperbolic, but engaging).
  - Organized so non-technical community members can navigate easily.

## Adding a New Application

When adding a new application to this repository:

1. Create a new folder: `docs/applications/<application-name>/`
2. Add the following files using the templates below:
   - `README.md`
   - `Overview.md`
   - `Getting-Started.md`
   - `Implementation-Notes.md`
   - `Gameplay.md` *(if the application is a game)*
3. Add a row to `docs/INDEX.md`.
4. Update `mkdocs.yml` to include the new files in the nav if the MkDocs site is in use.
5. Add a corresponding row to the applications table in the top-level `README.md`.

## Application README Template

Each `docs/applications/<app>/README.md` must follow this format:

```markdown
# Application Name

Short project description.

**Type:** <Game / Utility / Business Tool / etc.> | **Developer:** World Domination Software LLC

## Documentation
- [Overview](./Overview.md)
- [Getting Started](./Getting-Started.md)
- [Gameplay](./Gameplay.md)   ← include only if applicable
- [Implementation Notes](./Implementation-Notes.md)

## Public Links
- [GitHub Wiki](https://github.com/World-Domination-Software/Projects/wiki/<App-Wiki-Page>)
- [Bug Reports](https://github.com/World-Domination-Software/Projects/issues)
- [Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/<app-discussions-category>)

## Notes
This folder contains application-specific documentation only.
Shared FAQ, support, roadmap, and shared troubleshooting are maintained in the [GitHub Wiki](https://github.com/World-Domination-Software/Projects/wiki).
```

## Linking Rules

- Use **relative links** for links within `docs/` (e.g., `[Overview](./Overview.md)`).
- Use **full GitHub URLs** for:
  - The actual GitHub Wiki (e.g., `https://github.com/World-Domination-Software/Projects/wiki/...`)
  - Issues (e.g., `https://github.com/World-Domination-Software/Projects/issues`)
  - Discussions (e.g., `https://github.com/World-Domination-Software/Projects/discussions/...`)
- Update all links when moving documentation files.

## Automation

- Issue templates for bug reports, feature requests, and support live in `.github/ISSUE_TEMPLATE/`.
- When creating new templates or automation, assume they will be:
  - Linked from `projects.php` on the WDS website.
  - Used by both internal staff and external community members.
