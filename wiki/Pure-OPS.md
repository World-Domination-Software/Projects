# Pure OPS

**Type:** Game
**Developer:** World Domination Software LLC

---

## Overview

Pure OPS is a fast-paced tactical operations game. Players take on mission-based objectives requiring quick decision-making, coordinated movement, and precise execution. The game emphasizes clarity of purpose — each match has a defined objective, a clear win condition, and minimal friction between rounds.

## Purpose

Pure OPS is designed for players who want a focused, high-clarity tactical experience:

- Short, objective-driven sessions that reward skill over time investment.
- Tactical depth without excessive complexity or long onboarding curves.
- Clean competitive play with clear feedback on performance.

## Features

- **Mission-based structure** – Each session is built around a defined objective with a clear outcome.
- **Tactical movement and cover** – Positioning and decision-making are core to success.
- **Multiplayer and solo modes** – Play against others online or against AI opponents.
- **Progression system** – Unlockable loadouts and cosmetic items through play.
- **Replay and stats** – Post-match breakdown of key decisions and performance metrics.
- **Platform support** – PC (Windows and Linux) with controller support.

## Architecture

Pure OPS is a networked multiplayer application with a dedicated server backend for online matches. Solo and offline modes run against local AI. Client and server are distinct components.

Key components:

- **Game client** – Rendering, input, and UI layer.
- **Match server** – Authoritative server handling game state for online matches.
- **Matchmaking service** – WDS-hosted service for pairing players.
- **Backend services** – Progression, stats, and player data storage.

## Development Status

| Area | Status |
|---|---|
| Core gameplay | Available |
| Online multiplayer | Available |
| Solo / AI modes | Available |
| Ranked matchmaking | In development |
| Additional mission types | Planned |
| Steam Deck support | Planned |

For current priorities and planned work, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

## Support

- **Discussions (User Support):** https://github.com/World-Domination-Software/Projects/discussions/categories/pure-ops-support
- **Bug Reports:** https://github.com/World-Domination-Software/Projects/issues
- **Feature Requests:** https://github.com/World-Domination-Software/Projects/discussions/categories/pure-ops-feature-requests
- **General Discussion:** https://github.com/World-Domination-Software/Projects/discussions/categories/pure-ops-general

For general guidance on reporting bugs or using discussions effectively, see the [Community and Discussions guide](https://github.com/World-Domination-Software/Projects/blob/main/docs/discussions.md).
