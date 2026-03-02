<p align="center">
  <!-- Replace with your actual hero image/screenshot -->
  <!-- <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/images/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="docs/images/hero-light.png">
    <img alt="Whendows" src="docs/images/hero-light.png" width="800">
  </picture> -->
</p>

<h1 align="center">Whendows</h1>

<p align="center">
  A native Windows desktop client for <a href="https://github.com/anthropics/claude-code">Claude Code</a> and <a href="https://github.com/openai/codex">Codex CLI</a>.
</p>

<p align="center">
  <a href="https://github.com/GSonofNun/Whendows/releases/latest"><img alt="Latest Release" src="https://img.shields.io/github/v/release/GSonofNun/Whendows?style=flat-square"></a>
  <a href="https://github.com/GSonofNun/Whendows/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/GSonofNun/Whendows/total?style=flat-square"></a>
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%2010%2B-blue?style=flat-square">
</p>

---

## Features

- Native WinUI 3 interface with Fluent Design
- Real-time streaming of AI responses
- Support for both **Claude** (Anthropic) and **Codex** (OpenAI) as providers
- Session management — create, resume, and fork conversations
- Interactive permission prompts for file and command operations
- Inline file diff viewer
- Multi-project workspace support
- Per-session provider and model selection

## Download

Get the latest release from the **[Releases page](https://github.com/GSonofNun/Whendows/releases/latest)**.

### System Requirements

- Windows 10 (build 19041) or later
- At least one CLI provider installed (see below)

## Getting Started

### 1. Install a CLI Provider

Whendows requires at least one of the following CLI tools installed on your system.

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

### 2. Install Whendows

1. Download the latest release from the [Releases page](https://github.com/GSonofNun/Whendows/releases/latest)
2. Extract the archive
3. Run the application

### 3. Start a Session

- Whendows auto-detects installed CLI providers on startup
- Right-click a project in the sidebar to create a new **Claude** or **Codex** session
- Each session is tied to a single provider and can be resumed or forked at any time

## Reporting Issues

Found a bug or have a feature idea?

- [Report a bug](https://github.com/GSonofNun/Whendows/issues/new?template=bug_report.yml)
- [Request a feature](https://github.com/GSonofNun/Whendows/issues/new?template=feature_request.yml)

## Security

To report a security vulnerability, please see [SECURITY.md](SECURITY.md).
