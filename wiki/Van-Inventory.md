# Van Inventory

**Type:** Business Tool
**Developer:** World Domination Software LLC

---

## Overview

Van Inventory is a business application for managing inventory in mobile and van-based operations. It is designed for field technicians, mobile service providers, and small business operators who need to track stock, manage replenishment, and keep records of what is on their vehicles — without relying on complex desktop software.

## Purpose

Managing stock across mobile units is a persistent challenge for field service businesses. Van Inventory solves this by:

- Providing a lightweight, portable interface for real-time stock tracking.
- Reducing errors from manual record-keeping and end-of-day reconciliation.
- Giving business owners visibility across multiple vehicles or operators.

## Features

- **Stock tracking** – Log items in and out of each van with timestamps.
- **Low-stock alerts** – Configurable thresholds to notify when supplies need replenishment.
- **Multi-vehicle support** – Manage inventory for multiple vans from a single account.
- **Barcode / QR scanning** – Scan items in the field using a mobile device camera.
- **Replenishment lists** – Auto-generated lists based on current stock vs. targets.
- **Audit history** – Full log of stock changes with operator attribution.
- **Export** – Download inventory reports as CSV or PDF for accounting and operations review.

## Architecture

Van Inventory is a mobile-first application backed by a cloud service for data sync and multi-device access. The mobile app supports offline operation for field use; changes sync when connectivity is restored.

Key components:

- **Mobile app** – iOS and Android client for field use, including offline support.
- **Web dashboard** – Browser-based interface for business owners and managers.
- **Sync service** – WDS-hosted backend for data synchronization and storage.
- **Notification service** – Push and email alerts for low-stock and audit events.

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

## Support

- **Discussions (User Support):** https://github.com/World-Domination-Software/Projects/discussions/categories/van-inventory-support
- **Bug Reports:** https://github.com/World-Domination-Software/Projects/issues
- **Feature Requests:** https://github.com/World-Domination-Software/Projects/discussions/categories/van-inventory-feature-requests
- **General Discussion:** https://github.com/World-Domination-Software/Projects/discussions/categories/van-inventory-general

For general guidance on reporting bugs or using discussions effectively, see the [Community and Discussions guide](https://github.com/World-Domination-Software/Projects/blob/main/docs/discussions.md).
