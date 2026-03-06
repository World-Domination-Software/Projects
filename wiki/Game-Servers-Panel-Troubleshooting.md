# Game Servers Panel – Troubleshooting

← Back to [[Game-Servers-Panel]]

---

## General Steps First

- Refresh the panel dashboard in your browser.
- Check that the panel service and the agent on the affected server are both running.
- Review logs in the panel's **Logs and Diagnostics** section for error messages.

---

## Panel Will Not Load

- Check that the panel service is running on the host machine.
- Verify that the correct port is open and accessible (not blocked by a firewall).
- Clear your browser cache and try again.
- If the panel is behind a reverse proxy, verify the proxy configuration has not changed.

## Agent Not Connecting to Panel

- Verify the agent is running on the server host (`systemctl status <agent-service>` on Linux).
- Check that the agent is configured with the correct panel address and authentication token.
- Check firewall rules on both the panel host and the server host — the communication port must be open in both directions.
- Review the agent log for connection error messages.

## Server Shows as Offline When It Should Be Running

- Check the server process status directly on the host machine.
- Confirm the agent is running and connected to the panel (check the agent status in the panel sidebar).
- If the agent recently lost and re-established its connection, the panel status may take a moment to update — refresh the page.

## Cannot Start or Stop a Server from the Panel

- Verify your account role — start/stop actions require operator or administrator permissions.
- Check the server's lifecycle log in the panel for errors during the start/stop attempt.
- Try the action again; if it fails consistently, review the agent log for error details.

## Configuration Changes Not Taking Effect

- Some configuration changes require a server restart to apply. Use the panel's restart control after applying changes.
- Verify that the configuration file was saved correctly — check the panel's configuration editor for validation errors.

## Monitoring Data Is Stale or Missing

- Check that the agent is connected and actively sending telemetry (look for a green status indicator).
- If telemetry was interrupted, it may take a moment to resume after the agent reconnects.
- Large time gaps in monitoring data indicate the agent was offline or disconnected during that period.

---

## Still Having Issues?

1. Check [[Troubleshooting-Index]] for general guidance.
2. Search [existing issues](https://github.com/World-Domination-Software/Projects/issues).
3. Post in [Game Servers Panel Support Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/game-servers-panel-support).
4. File a bug report via [[Bug-Reporting]] if you have a reproducible problem.

---

**→ [[Game-Servers-Panel]] · [[Game-Servers-Panel-Overview]] · [[Game-Servers-Panel-FAQ]] · [[Troubleshooting-Index]]**
