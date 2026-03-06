# Optimization Protocol – Troubleshooting

← Back to [[Optimization-Protocol]]

---

## General Steps First

- Restart the application and try again.
- Make sure you are running the latest version.
- Run the application with administrator privileges if you encounter permission errors during scans.

---

## Application Will Not Launch

- Check that your operating system meets the minimum requirements.
- Try running as administrator (Windows: right-click → Run as administrator).
- Check that antivirus or security software is not blocking the executable.

## Scan Does Not Complete

- Make sure no other intensive processes are running that might interfere with measurement.
- Run as administrator — some system metrics require elevated permissions to read.
- If the scan stalls repeatedly, try restarting the application and running a scan from scratch.

## Recommendations Are Not Applying

- Confirm you have accepted any permission prompts that appear when applying changes.
- Some recommendations require a system restart to take effect — follow the prompts in the application.
- A small number of recommendations require manual steps; the application will indicate this.

## Before/After Comparison Shows No Change

- Allow adequate warm-up time before and after applying changes — run your benchmark scenario at least twice and use the second result.
- Some improvements are most visible under load conditions that match your specific use case.
- If results seem inconsistent, try disabling background processes (updaters, browsers) during measurement.

## Profile Sync Not Working

- Cloud profile sync requires an active internet connection and a signed-in WDS account.
- Check that the sync service is enabled in the application settings.
- If sync fails, your local profiles are not affected — they remain on the device.

## Scheduled Scans Not Running

- Verify that the application is set to run at startup or that a background service is enabled.
- Check that your system's power or sleep settings do not prevent the scan from running at the scheduled time.

---

## Still Having Issues?

1. Check [[Troubleshooting-Index]] for general guidance.
2. Search [existing issues](https://github.com/World-Domination-Software/Projects/issues).
3. Post in [Optimization Protocol Support Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/optimization-protocol-support).
4. File a bug report via [[Bug-Reporting]] if you have a reproducible problem.

---

**→ [[Optimization-Protocol]] · [[Optimization-Protocol-Overview]] · [[Optimization-Protocol-FAQ]] · [[Troubleshooting-Index]]**
