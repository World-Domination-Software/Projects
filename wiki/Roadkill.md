# Roadkill

**Type:** Game
**Developer:** World Domination Software LLC

---

## Overview

Roadkill is a vehicular action game. Players drive high-speed vehicles through arenas and open environments, competing in races, combat challenges, and objective-based modes. The game focuses on fast, chaotic fun with a variety of vehicles and play styles.

## Purpose

Roadkill is built for players who want:

- High-energy vehicular gameplay with accessible controls and immediate feedback.
- A range of modes from pure racing to combat-focused objectives.
- Replayable content through unlockable vehicles, tracks, and competitive scoring.

## Features

- **Multiple vehicle classes** – From nimble racers to heavy combat rigs, each with distinct handling.
- **Game modes** – Race, elimination, last-vehicle-standing, and objective-based modes.
- **Arena and open-track maps** – Closed arenas for combat and sprawling tracks for racing.
- **Multiplayer** – Online and local multiplayer for head-to-head and team play.
- **Progression and unlocks** – Earn vehicles, skins, and upgrades through play.
- **Controller support** – Full controller support for couch and desk play.
- **Platform support** – PC (Windows and Linux), Steam Deck.

## Architecture

Roadkill is a multiplayer-capable application with both local and online play. Online matches are handled by dedicated servers; local multiplayer runs directly on the client.

Key components:

- **Game client** – Rendering, physics, input, and game logic layer.
- **Online match server** – Dedicated server for authoritative multiplayer sessions.
- **Matchmaking and lobby service** – WDS-hosted service for player matchmaking.
- **Backend services** – Progression, leaderboards, and player data.

## Development Status

| Area | Status |
|---|---|
| Core gameplay | Available |
| PC (Windows/Linux) support | Available |
| Steam Deck support | Available |
| Online multiplayer | Available |
| Additional maps and modes | In development |
| Mobile port | Under consideration |

For current priorities and planned work, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

## Support

- **Discussions (User Support):** https://github.com/World-Domination-Software/Projects/discussions/categories/roadkill-support
- **Bug Reports:** https://github.com/World-Domination-Software/Projects/issues
- **Feature Requests:** https://github.com/World-Domination-Software/Projects/discussions/categories/roadkill-feature-requests
- **General Discussion:** https://github.com/World-Domination-Software/Projects/discussions/categories/roadkill-general

For general guidance on reporting bugs or using discussions effectively, see the [Community and Discussions guide](https://github.com/World-Domination-Software/Projects/blob/main/docs/discussions.md).
