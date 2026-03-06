# Game Servers Panel – FAQ

← Back to [[Game-Servers-Panel]]

---

## General

### What is Game Servers Panel?

Game Servers Panel is a web-based management interface for game server infrastructure. It lets operators deploy, monitor, configure, and control game server instances from a central dashboard, without needing direct command-line access to the server hosts.

### What types of game servers can be managed?

Game Servers Panel is designed to work with WDS-supported game server types. Support for specific games and server types is documented in the panel itself. Ask in [Game Servers Panel Support Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/game-servers-panel-support) for specifics.

### Is it cloud-hosted or self-hosted?

Game Servers Panel is self-hosted — you install and run the panel and agents on your own infrastructure. WDS does not manage your panel instance.

---

## Setup and Access

### How do I install the panel?

Installation documentation is included in the panel release package. For the latest guidance, see the [release notes](https://github.com/World-Domination-Software/Projects/releases) or ask in [Game Servers Panel Support Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/game-servers-panel-support).

### How do I add a new server to the panel?

Install the agent process on the server host, configure it with your panel address and authentication token, then register it in the panel dashboard. Detailed steps are in the panel's documentation.

### Can multiple operators manage the same panel?

Yes. Role-based access control allows you to create accounts with different permission levels (viewer, operator, administrator).

---

## Operations

### Do configuration changes require a server restart?

Most configuration changes require a server restart to take effect. The panel will indicate when a restart is needed after applying changes.

### Can I schedule maintenance windows?

Yes. The panel supports scheduled lifecycle actions including maintenance windows and restarts.

### How do I access server logs?

Server logs are accessible directly from the panel's **Logs and Diagnostics** section for any connected server.

---

## Technical

### How do I report a bug?

See [[Bug-Reporting]] for how to choose the right template and what to include.

### Something is wrong with the agent connection. What should I check?

See [[Game-Servers-Panel-Troubleshooting]] for a step-by-step agent connectivity guide.

---

**→ [[Game-Servers-Panel]] · [[Game-Servers-Panel-Troubleshooting]] · [[Support]] · [[Bug-Reporting]]**
