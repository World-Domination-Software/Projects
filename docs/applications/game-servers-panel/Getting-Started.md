# Game Servers Panel – Getting Started

← [Back to README](./README.md)

---

## Overview

Game Servers Panel is a self-hosted application. You install and run the panel on your own infrastructure. WDS does not manage your panel instance.

The panel consists of two components:
- **Panel web application** – Installed on a central host; provides the dashboard and API.
- **Agent process** – Installed on each server host you want to manage.

---

## Prerequisites

Before installing, ensure you have:

- A server or VM to host the panel web application (Linux recommended).
- Network access between the panel host and each server host.
- A supported runtime environment (see release notes for current requirements).

---

## Installation

### Step 1: Install the panel

1. Download the latest panel release from the [Releases page](https://github.com/World-Domination-Software/Projects/releases).
2. Extract and run the installer on your panel host.
3. Follow the on-screen setup wizard to configure:
   - Listening port and hostname.
   - Administrator account credentials.
   - Database location (local SQLite or remote database, depending on your setup).
4. Start the panel service. Confirm it is accessible in a browser at your configured address.

### Step 2: Install the agent on each server host

1. Download the agent package from the same release.
2. Install it on each server host you want to manage.
3. Configure the agent with:
   - Your panel's address.
   - An authentication token (generated in the panel under **Settings → Agents**).
4. Start the agent service.

### Step 3: Register servers in the panel

1. Open the panel in your browser.
2. Go to **Servers → Add Server**.
3. Enter the server host details and confirm the agent connection.
4. Repeat for each server host.

---

## First Use

After setup, you can:

- View server status from the **Dashboard**.
- Deploy a new server instance from **Servers → Deploy**.
- Edit server configuration from the **Configuration** tab for any server.
- Access server logs from **Logs and Diagnostics**.

---

## Tips

- Use role-based access control to give operators the minimum permissions they need.
- Schedule maintenance windows for server restarts to minimize disruption.
- Monitor the **Health** view regularly to catch resource issues before they affect players.

---

**→ [README](./README.md) · [Overview](./Overview.md) · [Implementation Notes](./Implementation-Notes.md)**
