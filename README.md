<h1 align="center">Jericode</h1>

<p align="center">
  A native Windows desktop client for <a href="https://github.com/anthropics/claude-code">Claude Code</a> and <a href="https://github.com/openai/codex">Codex CLI</a>.
</p>

<p align="center">
  <a href="https://apps.microsoft.com/detail/9N3W6PQ7X087" target="_blank" rel="noopener noreferrer"><img alt="Microsoft Store" src="https://img.shields.io/badge/Microsoft%20Store-Download-blue?style=flat-square&logo=microsoft"></a>
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%2010%2B-blue?style=flat-square">
  <a href="https://github.com/GSonofNun/Jericode-ADE/releases"><img alt="Beta" src="https://img.shields.io/badge/release-Beta-orange?style=flat-square"></a>
</p>

> **Jericode is currently in Beta.** Expect rough edges, and please [file issues](https://github.com/GSonofNun/Jericode-ADE/issues) when you hit them.

---

## Features

- **Real-time streaming** — Watch AI responses appear token-by-token with live token counting
- **Visual file diffs** — Side-by-side code diffs with syntax highlighting
- **Multi-provider** — Switch between Claude and Codex per session with independent configuration
- **Session management** — Create, resume, and fork conversations with full persistence
- **Permission controls** — Approve or deny tool permissions through a visual dialog with risk indicators
- **Token and cost tracking** — Monitor usage per turn and per session with budget limits
- **File mentions** — Reference project files with `@file` autocomplete and gitignore-aware fuzzy search
- **Sub-agent monitoring** — Track parallel agent activity in real time
- **Plan mode** — Review AI strategies before execution
- **Dark and light themes** — Native WinUI 3 with Windows accent color integration
- **Project workspaces** — Organize sessions by project with smart temporal grouping
- **Privacy first** — All data stays on your machine. No telemetry, no analytics, no tracking.

## Download

<a href="https://apps.microsoft.com/detail/9N3W6PQ7X087" target="_blank" rel="noopener noreferrer"><img alt="Download from Microsoft Store" src="https://get.microsoft.com/images/en-us%20dark.svg" width="200"></a>

**Prefer to sideload?** Grab the latest x64 or ARM64 MSIX from [GitHub Releases](https://github.com/GSonofNun/Jericode-ADE/releases). See the release notes for install steps — you'll need to trust the included developer certificate before the first install.

### System Requirements

- Windows 10 (build 19041) or later
- At least one CLI provider installed (see below)

## Getting Started

### 1. Install a CLI Provider

Jericode requires at least one of the following CLI tools installed on your system.

#### Claude Code (Anthropic)

Claude Code is Anthropic's agentic coding tool that runs in your terminal.

**Install:**

- **PowerShell (recommended):** Run the install script from [code.claude.com/docs/en/setup](https://code.claude.com/docs/en/setup)
- **WinGet:** `winget install Anthropic.ClaudeCode`
- Requires [Git for Windows](https://git-scm.com/download/win) (Claude Code uses Git Bash internally)

**Authenticate:**

1. Open a terminal and run `claude`
2. Follow the browser prompts to sign in with your Anthropic account
3. Requires a Claude subscription (Pro, Max, Teams, or Enterprise) or Anthropic API access

#### Codex (OpenAI)

Codex is OpenAI's lightweight coding agent that runs in your terminal.

**Install:**

- **npm:** `npm i -g @openai/codex`
- **Homebrew:** `brew install --cask codex`
- Or download a binary from the [Codex GitHub releases](https://github.com/openai/codex/releases)

**Authenticate:**

1. Open a terminal and run `codex`
2. Select **Sign in with ChatGPT** (recommended) and follow the browser prompts
3. Alternatively, set the `OPENAI_API_KEY` environment variable with your API key
4. Requires a ChatGPT Plus, Pro, Team, Edu, or Enterprise plan (or an OpenAI API key)

### 2. Install Jericode

Download Jericode from the [Microsoft Store](https://apps.microsoft.com/detail/9N3W6PQ7X087), or sideload from [GitHub Releases](https://github.com/GSonofNun/Jericode-ADE/releases).

### 3. Start a Session

- Jericode auto-detects installed CLI providers on startup
- Click new session button in the top of the left sidebar to start a new session
- Each session is tied to a single provider and can be resumed or forked at any time

## Privacy

Jericode does not collect, transmit, or share any personal data. All conversations, session data, and settings are stored locally on your device. See [PRIVACY.md](PRIVACY.md) for details.

## Reporting Issues

Found a bug or have a feature idea?

- [Report a bug](https://github.com/GSonofNun/Jericode-ADE/issues/new?template=bug_report.yml)
- [Request a feature](https://github.com/GSonofNun/Jericode-ADE/issues/new?template=feature_request.yml)

## Security

To report a security vulnerability, please see [SECURITY.md](SECURITY.md).
