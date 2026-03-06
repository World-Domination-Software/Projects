# Van Inventory – Implementation Notes

← [Back to README](./README.md)

---

## Architecture

Van Inventory is a mobile-first application backed by a cloud service for data sync and multi-device access. The mobile app supports offline operation for field use; changes sync when connectivity is restored.

### Key Components

| Component | Description |
|---|---|
| **Mobile app** | iOS and Android client for field use, including offline support. |
| **Web dashboard** | Browser-based interface for business owners and managers. |
| **Sync service** | WDS-hosted backend for data synchronization and storage. |
| **Notification service** | Push and email alerts for low-stock and audit events. |

---

## Platform Support

| Platform | Status |
|---|---|
| iOS | Available |
| Android | Available |
| Web dashboard | Available |

---

## Development Status

| Area | Status |
|---|---|
| Mobile app (iOS/Android) | Available |
| Web dashboard | Available |
| Multi-vehicle support | Available |
| Offline sync | Available |
| Advanced reporting | In development |
| Third-party integrations | Planned |

For current priorities and planned work, see the [Roadmap discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/roadmap).

---

**→ [README](./README.md) · [Overview](./Overview.md) · [Getting Started](./Getting-Started.md)**
