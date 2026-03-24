# Privacy Policy

**Effective Date:** March 23, 2026
**App:** Jericode
**Developer:** Joshua Grzybowski

## Overview

Jericode is a native Windows desktop client for Claude Code and Codex CLI. Your privacy is important — Jericode does **not** collect, transmit, or share any personal data or usage analytics.

## Data Storage

All data created by Jericode is stored **locally on your device** and never sent to external servers. This includes:

- **Conversation history** — stored as local files in `%LOCALAPPDATA%\Jericode\Sessions\`
- **Workspace and session metadata** — stored in a local SQLite database at `%LOCALAPPDATA%\Jericode\workspace.db`
- **Application logs** — stored locally for troubleshooting purposes
- **User preferences** — theme, layout, and configuration settings stored locally

You can delete this data at any time by removing sessions within the app or by deleting the `%LOCALAPPDATA%\Jericode` directory.

## Data Collection

Jericode does **not** collect:

- Personal information
- Usage analytics or telemetry
- Crash reports sent to external services
- Advertising or tracking data
- Cookies or browser fingerprints

## Network Communication

Jericode makes **no network requests** except:

- **CLI binary downloads** — When you install or update Claude Code through the app, Jericode downloads the binary from a secure (HTTPS) distribution endpoint. No user data is sent during this process.

All conversations with Claude or Codex are handled by their respective CLI processes running locally on your machine. Jericode communicates with these processes via local stdin/stdout — it does not contact Anthropic's or OpenAI's servers directly.

## Third-Party Services

Jericode acts as a frontend for **Claude CLI** and **Codex CLI**, which have their own privacy policies and terms of service:

- [Anthropic Privacy Policy](https://www.anthropic.com/privacy)
- [OpenAI Privacy Policy](https://openai.com/privacy)

Jericode does not control how these CLI tools handle your data. Please review their respective policies for details.

## Children's Privacy

Jericode does not knowingly collect any information from children under the age of 13.

## Changes to This Policy

Updates to this privacy policy will be reflected in this document with an updated effective date. Continued use of Jericode after changes constitutes acceptance of the revised policy.

## Contact

If you have questions about this privacy policy, please open an issue at [github.com/GSonofNun/Jericode-ADE](https://github.com/GSonofNun/Jericode-ADE/issues).
