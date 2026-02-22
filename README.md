# Privacy Policy — DBine

**Last updated:** February 22, 2026

## Overview

DBine is a browser extension that provides a collaborative SQLite and CSV viewer in the Chrome sidebar. Your privacy is important to us. This policy explains what data DBine accesses, how it is used, and your rights.

## Data Collection

**DBine does not collect, store, or transmit any personal data to any server.**

All database files, queries, and edits remain entirely within your browser using local storage technologies (Origin Private File System and IndexedDB).

## Local Storage

DBine stores the following data locally on your device:

- **User preferences** — theme selection (light/dark/system) and SQL query history, saved via the Chrome Storage API.
- **Database files** — any SQLite or CSV files you import are stored locally in your browser's Origin Private File System (OPFS) and IndexedDB. They never leave your device unless you explicitly use the collaboration feature.

## Collaboration (Peer-to-Peer)

When you choose to start or join a collaboration session:

- Data is transmitted **directly between participants** using WebRTC (peer-to-peer).
- **No central server** processes or stores your database content.
- A third-party signaling service (via the Trystero library) is used only to establish the initial peer-to-peer connection. It does not have access to your database content.
- You control who joins your session through an approval mechanism.

## AI Feature

DBine includes an optional "Ask AI" feature that converts natural language questions into SQL queries:

- **Machine learning models** are downloaded from HuggingFace (huggingface.co) and cached locally in your browser.
- **All AI inference runs locally** in your browser. No queries, database content, or personal data is sent to any AI service or external server.

## Third-Party Services

- **HuggingFace CDN** — used only to download open-source ML model files. No user data is uploaded.
- **Trystero signaling** — used only to establish WebRTC peer connections for collaboration. No database content passes through this service.

## Permissions

- `storage` — save user preferences locally
- `offscreen` — run SQLite and WebRTC in a background document (required by Manifest V3)
- `sidePanel` — display the extension UI in the browser sidebar

## Analytics and Tracking

DBine does **not** use any analytics, telemetry, tracking scripts, or cookies. There are no user accounts and no sign-up required.

## Children's Privacy

DBine does not knowingly collect any data from children or any other users.

## Changes to This Policy

If this privacy policy is updated, the changes will be reflected in this document with an updated date.

## Contact

If you have questions about this privacy policy, please open an issue on the [DBine GitHub repository](https://github.com/javisantos/DBine).
