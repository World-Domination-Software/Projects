# Game Servers Panel – Implementation Notes

← [Back to README](./README.md)

---

## Architecture

Game Servers Panel is a web-based application with a server-side backend that communicates with agent processes running on each hosted machine. The panel UI is served from a central host; agents relay commands and telemetry between the panel and the underlying servers.

### Key Components

| Component | Description |
|---|---|
| **Panel web application** | User-facing dashboard and API layer. Hosted on a central server. |
| **Agent process** | Lightweight service installed on each server host, handling lifecycle and telemetry. |
| **Communication layer** | Secure channel between the panel and agents. |

---

## Deployment Model

Game Servers Panel is **self-hosted**. You install and run both the panel and agents on your own infrastructure. WDS provides the software and documentation; you provide the hosting environment.

---

## Development Status

| Area | Status |
|---|---|
| Core panel and agent | Active development |
| Monitoring and dashboards | Available |
| Role-based access control | Available |
| Extended log analysis | Planned |

For current priorities and planned work, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

---

**→ [README](./README.md) · [Overview](./Overview.md) · [Getting Started](./Getting-Started.md)**
