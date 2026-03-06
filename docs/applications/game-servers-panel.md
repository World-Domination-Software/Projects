# Game Servers Panel

**Type:** Hosting / Infrastructure
**Developer:** World Domination Software LLC

## Overview

Game Servers Panel is a hosting and management application for game server infrastructure. It provides a centralized interface for deploying, monitoring, and administering game server instances, giving operators control over their hosting environment without requiring deep command-line expertise.

## Purpose

Running game servers reliably is complex. Game Servers Panel simplifies that process by:

- Providing a single dashboard for all hosted server instances.
- Reducing the operational burden of manual server administration.
- Making server management accessible to operators who are not system administrators.

## Features

- **Server deployment** – Spin up new server instances quickly from a managed interface.
- **Monitoring and status** – View live status, resource usage, and health for each server.
- **Configuration management** – Edit and apply server configuration without direct file access.
- **Access control** – Role-based permissions for operators and administrators.
- **Logs and diagnostics** – Access server logs directly from the panel for troubleshooting.
- **Restart and lifecycle controls** – Start, stop, restart, and schedule maintenance windows.

## Architecture

Game Servers Panel is a web-based application with a server-side backend that communicates with agent processes running on each hosted machine. The panel UI is served from a central host; agents relay commands and telemetry between the panel and the underlying servers.

Key components:

- **Panel web application** – User-facing dashboard and API layer.
- **Agent process** – Lightweight service installed on each server host, handling lifecycle and telemetry.
- **Communication layer** – Secure channel between the panel and agents.

## Development Status

| Area | Status |
|---|---|
| Core panel and agent | Active development |
| Monitoring and dashboards | Available |
| Role-based access control | Available |
| Extended log analysis | Planned |

For current priorities and planned work, see the [Roadmap](../roadmap.md).

## Support

- **Discussions (User Support):** https://github.com/World-Domination-Software/Projects/discussions/categories/game-servers-panel-support
- **Bug Reports:** https://github.com/World-Domination-Software/Projects/issues
- **Feature Requests:** https://github.com/World-Domination-Software/Projects/discussions/categories/game-servers-panel-feature-requests
- **General Discussion:** https://github.com/World-Domination-Software/Projects/discussions/categories/game-servers-panel-general
