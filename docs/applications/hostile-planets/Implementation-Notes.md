# Hostile Planets – Implementation Notes

← [Back to README](./README.md)

---

## Architecture

Hostile Planets is a standalone application built for desktop platforms. The game client handles all gameplay logic locally; online features such as leaderboards communicate with WDS backend services.

### Key Components

| Component | Description |
|---|---|
| **Game client** | Core application handling rendering, input, and gameplay simulation. |
| **Backend services** | Cloud-side services for leaderboards and player data. |
| **Platform integrations** | Steam achievements and cloud saves where supported. |

---

## Platform Support

| Platform | Status |
|---|---|
| PC – Windows | Available |
| PC – Linux | Available |
| Steam Deck | Available (Verified) |
| Android | Under consideration |
| iOS | Under consideration |

---

## Development Status

| Area | Status |
|---|---|
| Core gameplay | Available |
| PC (Windows/Linux) support | Available |
| Steam Deck support | Available |
| Additional environments | Planned |
| Mobile port | Under consideration |

For current priorities and planned work, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

---

**→ [README](./README.md) · [Overview](./Overview.md) · [Getting Started](./Getting-Started.md) · [Gameplay](./Gameplay.md)**
