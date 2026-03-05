# World Domination Software - Projects Repository Guidelines

## Repository Role

- This repository (`World-Domination-Software/Projects`) is the **customer-facing hub** for all WDS projects (games, tools, hosting, and related products).
- It centralizes:
  - High-level project descriptions and design documents (Wiki)
  - Future project ideas and feature proposals (Discussions → Ideas category)
  - Bug reports, incidents, and support tickets (Issues)
  - General project discussions and community feedback (Discussions)
- The public website repository (`WDS_Website`) links to this repo from its `projects.php` page for all detailed project information and customer interaction.

## How This Repo Interacts With Others

- **WDS_Website**
  - Lists projects and shows short summaries only.
  - Each project row links here for wiki pages, ideas, discussions, and issue reporting.
  - Changes to project naming, categories, or status here should be reflected in the website’s project list (and vice versa) so they stay in sync.

- **GSP / Agents and Other Service Repos**
  - Game server panel and agent repos are internal implementation details.
  - Customer-facing documentation, roadmaps, and issue tracking for those services should live **in this repo** (Wiki/Issues/Discussions), then link out to the underlying technical repos when necessary.

## Guidance for AIs Working in This Repo

- Treat this repo as the **source of truth for customer-visible project information and planning**.
- When adding or modifying structures (labels, discussion categories, issue templates, wiki organization):
  - Keep terminology consistent with what the WDS website uses for project names and categories.
  - Prefer adding new templates/structures over breaking existing ones that might already be in use.
- Do **not** move long-form documentation back into the website codebase; the website should point here instead.
- When suggesting or generating new content (issue templates, discussion prompts, wiki outlines), make it:
  - Professional, clear, and accessible (non-hyperbolic, but engaging).
  - Organized so non-technical community members can navigate easily.

## Future Structure (for Templates and Automation)

- This repo is expected to contain:
  - Issue templates for bug reports, feature requests, and support.
  - Discussion templates/categories for ideas, playtesting feedback, and devlogs.
  - Wiki templates for per-project overview pages (summary, status, links to builds, etc.).
- When creating new templates or automation, assume they will be:
  - Linked from `projects.php` on the WDS website.
  - Used by both internal staff and external community members.
