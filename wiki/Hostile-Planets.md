# Hostile Planets

**Type:** Game
**Developer:** World Domination Software LLC

---

## Overview

Hostile Planets is an action game set across environments inspired by alien worlds. Players navigate dangerous terrain, engage hostile forces, and work to survive and complete objectives across a series of increasingly challenging levels.

## Purpose

Hostile Planets delivers a challenging action experience focused on:

- Intense, skill-based gameplay in varied and dangerous environments.
- Exploration and discovery across distinct alien settings.
- Replayable encounters with escalating difficulty.

## Features

- **Multiple environments** – Each zone presents different hazards, enemies, and terrain.
- **Combat system** – Ranged and close-quarters combat with diverse enemy types.
- **Progression** – Character and equipment upgrades that carry through a run.
- **Leaderboards** – Competitive scoring for players who want to push for high placements.
- **Platform support** – Available on PC (Windows and Linux) and Steam Deck.

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

For current priorities and planned work, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

## Support

- **Discussions (User Support):** https://github.com/World-Domination-Software/Projects/discussions/categories/hostile-planets-support
- **Bug Reports:** https://github.com/World-Domination-Software/Projects/issues
- **Feature Requests:** https://github.com/World-Domination-Software/Projects/discussions/categories/hostile-planets-feature-requests
- **General Discussion:** https://github.com/World-Domination-Software/Projects/discussions/categories/hostile-planets-general

For general guidance on reporting bugs or using discussions effectively, see the [Community and Discussions guide](https://github.com/World-Domination-Software/Projects/blob/main/docs/discussions.md).
