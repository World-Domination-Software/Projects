# Wiki Map

This file documents the mapping between source files in the repo `wiki/` and `docs/` folders and their corresponding destination pages in the actual GitHub Wiki.

---

## Shared Help Pages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Home.md` | `wiki/Home.md` (updated) |
| `_Sidebar.md` | `wiki/_Sidebar.md` (new) |
| `Projects.md` | `wiki/Projects.md` (new, based on `wiki/Applications.md`) |
| `Troubleshooting-Index.md` | `wiki/Troubleshooting-Index.md` (new, based on `docs/troubleshooting.md` + `docs/multiplayer.md`) |
| `Bug-Reporting.md` | `wiki/Bug-Reporting.md` (new, based on `docs/bug-reporting.md`) |
| `Support.md` | `wiki/Support.md` (new) |
| `FAQ.md` | `wiki/FAQ.md` (new, based on `docs/faq.md`) |
| `Roadmap.md` | `wiki/Roadmap.md` (new, based on `docs/roadmap.md`) |
| `Community-and-Discussions.md` | `wiki/Community-and-Discussions.md` (new, based on `docs/discussions.md`) |

---

## Project Landing Pages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Hostile-Planets.md` | `wiki/Hostile-Planets.md` (updated to landing page) |
| `Optimization-Protocol.md` | `wiki/Optimization-Protocol.md` (updated to landing page) |
| `Pure-OPS.md` | `wiki/Pure-OPS.md` (updated to landing page) |
| `Van-Inventory.md` | `wiki/Van-Inventory.md` (updated to landing page) |
| `Roadkill.md` | `wiki/Roadkill.md` (updated to landing page) |
| `Game-Servers-Panel.md` | `wiki/Game-Servers-Panel.md` (updated to landing page) |

---

## Hostile Planets Subpages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Hostile-Planets-Overview.md` | `wiki/Hostile-Planets-Overview.md` (new, content from `wiki/Hostile-Planets.md` original) |
| `Hostile-Planets-Getting-Started.md` | `wiki/Hostile-Planets-Getting-Started.md` (new, from `docs/getting-started.md`) |
| `Hostile-Planets-Troubleshooting.md` | `wiki/Hostile-Planets-Troubleshooting.md` (new, from `docs/troubleshooting.md`) |
| `Hostile-Planets-FAQ.md` | `wiki/Hostile-Planets-FAQ.md` (new, from `docs/faq.md`) |

---

## Optimization Protocol Subpages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Optimization-Protocol-Overview.md` | `wiki/Optimization-Protocol-Overview.md` (new, content from `wiki/Optimization-Protocol.md` original) |
| `Optimization-Protocol-Troubleshooting.md` | `wiki/Optimization-Protocol-Troubleshooting.md` (new) |
| `Optimization-Protocol-FAQ.md` | `wiki/Optimization-Protocol-FAQ.md` (new) |

---

## Pure OPS Subpages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Pure-OPS-Overview.md` | `wiki/Pure-OPS-Overview.md` (new, content from `wiki/Pure-OPS.md` original) |
| `Pure-OPS-Troubleshooting.md` | `wiki/Pure-OPS-Troubleshooting.md` (new, from `docs/multiplayer.md`) |
| `Pure-OPS-FAQ.md` | `wiki/Pure-OPS-FAQ.md` (new) |

---

## Van Inventory Subpages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Van-Inventory-Overview.md` | `wiki/Van-Inventory-Overview.md` (new, content from `wiki/Van-Inventory.md` original) |
| `Van-Inventory-Troubleshooting.md` | `wiki/Van-Inventory-Troubleshooting.md` (new) |
| `Van-Inventory-FAQ.md` | `wiki/Van-Inventory-FAQ.md` (new) |

---

## Roadkill Subpages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Roadkill-Overview.md` | `wiki/Roadkill-Overview.md` (new, content from `wiki/Roadkill.md` original) |
| `Roadkill-Gameplay.md` | `wiki/Roadkill-Gameplay.md` (new) |
| `Roadkill-Troubleshooting.md` | `wiki/Roadkill-Troubleshooting.md` (new) |
| `Roadkill-FAQ.md` | `wiki/Roadkill-FAQ.md` (new) |

---

## Game Servers Panel Subpages

| Destination Wiki Page | Source File(s) |
|---|---|
| `Game-Servers-Panel-Overview.md` | `wiki/Game-Servers-Panel-Overview.md` (new, content from `wiki/Game-Servers-Panel.md` original) |
| `Game-Servers-Panel-Troubleshooting.md` | `wiki/Game-Servers-Panel-Troubleshooting.md` (new) |
| `Game-Servers-Panel-FAQ.md` | `wiki/Game-Servers-Panel-FAQ.md` (new) |

---

## Existing Source Files (Not Renamed, Still Used by MkDocs)

The following files in `docs/` remain unchanged and continue to serve the MkDocs documentation site. Their content has been adapted and reorganized into the wiki pages above.

| Source File | Content Used In |
|---|---|
| `docs/troubleshooting.md` | `Troubleshooting-Index.md`, per-project troubleshooting pages |
| `docs/bug-reporting.md` | `Bug-Reporting.md` |
| `docs/faq.md` | `FAQ.md`, per-project FAQ pages |
| `docs/roadmap.md` | `Roadmap.md` |
| `docs/discussions.md` | `Community-and-Discussions.md` |
| `docs/multiplayer.md` | `Troubleshooting-Index.md`, `Pure-OPS-Troubleshooting.md`, `Roadkill-Troubleshooting.md` |
| `docs/getting-started.md` | `Hostile-Planets-Getting-Started.md` |
| `docs/applications/*.md` | Content in Overview pages |

---

## Missing Content (Requires Manual Writing)

The following items have wiki page stubs or minimal content that would benefit from additional work:

- **Per-project Getting Started pages** – Optimization Protocol, Pure OPS, Van Inventory, Roadkill, and Game Servers Panel do not yet have dedicated Getting Started / onboarding pages. These should be added when product-specific setup documentation becomes available.
- **Game Servers Panel installation guide** – A dedicated setup/installation page would be valuable given the self-hosted nature of the panel.
- **Screenshots and images** – Visual content for gameplay, UI, and the panel dashboard would improve the wiki pages significantly.
