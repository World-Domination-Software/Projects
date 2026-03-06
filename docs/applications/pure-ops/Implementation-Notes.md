# Pure OPS – Implementation Notes

← [Back to README](./README.md)

---

## Architecture

Pure OPS is a networked multiplayer application with a dedicated server backend for online matches. Solo and offline modes run against local AI. Client and server are distinct components.

### Key Components

| Component | Description |
|---|---|
| **Game client** | Rendering, input, and UI layer. |
| **Match server** | Authoritative server handling game state for online matches. |
| **Matchmaking service** | WDS-hosted service for pairing players. |
| **Backend services** | Progression, stats, and player data storage. |

---

## Platform Support

| Platform | Status |
|---|---|
| PC – Windows | Available |
| PC – Linux | Available |
| Steam Deck | Planned |

---

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

---

**→ [README](./README.md) · [Overview](./Overview.md) · [Getting Started](./Getting-Started.md)**
