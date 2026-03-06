# Roadkill – Implementation Notes

← [Back to README](./README.md)

---

## Architecture

Roadkill is a multiplayer-capable application with both local and online play. Online matches are handled by dedicated servers; local multiplayer runs directly on the client.

### Key Components

| Component | Description |
|---|---|
| **Game client** | Rendering, physics, input, and game logic layer. |
| **Online match server** | Dedicated server for authoritative multiplayer sessions. |
| **Matchmaking and lobby service** | WDS-hosted service for player matchmaking. |
| **Backend services** | Progression, leaderboards, and player data. |

---

## Platform Support

| Platform | Status |
|---|---|
| PC – Windows | Available |
| PC – Linux | Available |
| Steam Deck | Available |
| Mobile | Under consideration |

---

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

---

**→ [README](./README.md) · [Overview](./Overview.md) · [Getting Started](./Getting-Started.md) · [Gameplay](./Gameplay.md)**
