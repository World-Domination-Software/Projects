# Troubleshooting Index

This page provides a symptom-based index for common issues across WDS products. Find your symptom below and follow the linked guidance.

---

## Game Issues

### Game will not launch

- Verify the game files are complete. On Steam, use **Steam → Right-click game → Properties → Installed Files → Verify integrity of game files**.
- Make sure your operating system and graphics drivers are up to date.
- Disable overlays (Steam Overlay, Discord Overlay, GeForce Experience) and try again.
- Run the game as administrator on Windows if you get a permissions error.
- Check for antivirus or firewall software blocking the game executable.

### Low FPS or stuttering

- Lower graphics settings: resolution, shadows, anti-aliasing, and post-processing have the biggest impact.
- Close background applications that use CPU, GPU, or disk heavily (browsers, video players, update managers).
- Prefer running from an SSD over an HDD.
- On laptops or mobile devices, disable battery saver mode and check that GPU usage is on the dedicated card.
- Make sure your drivers (GPU, chipset) are current.

### Game crashes or freezes

- Update your GPU drivers to the latest version.
- Check that your system meets the minimum hardware requirements for the game.
- Verify game file integrity (see above).
- Check the game's log files for error messages and include them in a bug report.
- See [[Bug-Reporting]] for how to file a crash report.

### Missing files or download issues

- Re-run the game installer or use your platform's file verification tool.
- Check available disk space — some platforms require extra space beyond the installed size during updates.
- Temporarily disable antivirus software during download or installation.

### UI not loading or displaying incorrectly

- Restart the game fully (quit and relaunch, do not just Alt+Tab back in).
- Check for pending OS or driver updates.
- Try resetting in-game settings to defaults if the option is available.
- If the issue persists, file a bug report with a screenshot. See [[Bug-Reporting]].

---

## Multiplayer Issues

### Multiplayer disconnects

- Check your internet connection stability — run a speed test or ping test during play.
- Prefer Ethernet over Wi-Fi when hosting or playing competitively.
- Disable VPNs and proxies during play, as they can reroute or block game traffic.
- Make sure all players are on the same game version.

### Cannot connect to server or match

- Check that your firewall is not blocking the game's network ports.
- Strict or symmetric NAT types can prevent direct connections — try from a different network (mobile hotspot) to test.
- If you are behind a corporate, school, or public network, required ports may be blocked entirely.
- Reboot your router and modem, then try again.

For extended multiplayer troubleshooting, see the project-specific pages below.

---

## Per-Project Troubleshooting

| Project | Troubleshooting Page |
|---|---|
| Hostile Planets | [[Hostile-Planets-Troubleshooting]] |
| Optimization Protocol | [[Optimization-Protocol-Troubleshooting]] |
| Pure OPS | [[Pure-OPS-Troubleshooting]] |
| Van Inventory | [[Van-Inventory-Troubleshooting]] |
| Roadkill | [[Roadkill-Troubleshooting]] |
| Game Servers Panel | [[Game-Servers-Panel-Troubleshooting]] |

---

## Still having issues?

If these steps do not resolve your problem:

1. Check [[FAQ]] for known answers.
2. Search existing [GitHub Issues](https://github.com/World-Domination-Software/Projects/issues) for similar reports.
3. Open a [Support Discussion](https://github.com/World-Domination-Software/Projects/discussions) if you are not sure it is a bug.
4. File a bug report using [[Bug-Reporting]] if you have a clear, reproducible problem.

---

**→ [[Home]] · [[Projects]] · [[Bug-Reporting]] · [[Support]]**
