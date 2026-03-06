# Hostile Planets – Overview

**Type:** Game | **Developer:** World Domination Software LLC

← Back to [[Hostile-Planets]]

---

## What Is Hostile Planets?

Hostile Planets is an action game set across environments inspired by alien worlds. Players navigate dangerous terrain, engage hostile forces, and complete objectives across a series of increasingly challenging levels. The game focuses on intense, skill-based play in varied environments with meaningful progression between runs.

## Purpose

Hostile Planets delivers a challenging action experience focused on:

- Intense, skill-based gameplay in varied and dangerous environments.
- Exploration and discovery across distinct alien settings.
- Replayable encounters with escalating difficulty.

## Features

| Feature | Description |
|---|---|
| **Multiple environments** | Each zone presents different hazards, enemies, and terrain. |
| **Combat system** | Ranged and close-quarters combat with diverse enemy types. |
| **Progression** | Character and equipment upgrades that carry through a run. |
| **Leaderboards** | Competitive scoring for players who want to push for high placements. |
| **Platform support** | PC (Windows and Linux) and Steam Deck. |

## Architecture

Hostile Planets is a standalone application built for desktop platforms. The game client handles all gameplay logic locally; online features such as leaderboards communicate with WDS backend services.

Key components:

- **Game client** – Core application handling rendering, input, and gameplay simulation.
- **Backend services** – Cloud-side services for leaderboards and player data.
- **Platform integrations** – Steam achievements and cloud saves where supported.

## Development Status

| Area | Status |
|---|---|
| Core gameplay | Available |
| PC (Windows/Linux) support | Available |
| Steam Deck support | Available |
| Additional environments | Planned |
| Mobile port | Under consideration |

For current priorities, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

---

**→ [[Hostile-Planets]] · [[Hostile-Planets-Getting-Started]] · [[Hostile-Planets-Troubleshooting]] · [[Hostile-Planets-FAQ]]**
