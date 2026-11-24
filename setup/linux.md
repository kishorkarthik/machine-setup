# Linux

Here is the setup for my Linux environments.

## HP Victus, 24 Nov 2026

[HP Victus](https://www.amazon.in/HP-i5-13420H-Windows-Office24-fa2196TX/dp/B0G2R8YYXZ/)
running Ubuntu 26.04.1 LTS on Windows 11 through WSL2.

### Ubuntu on WSL2

- Distribution: Ubuntu 26.04.1 LTS
- Hostname: HP
- Kernel: 6.18.58.1-microsoft-standard-WSL2
- Architecture: x86-64

### Installation

Installed WSL2 and Ubuntu using PowerShell:

```bash
wsl --install                                        # wsl - windows subsytem for linux
```

## Workspace

- `~/projects` - GitHub repos, including `machine-setup/` (this repo: shared `.gitconfig`, setup docs) and `agent-scripts/`

The workspace root also contains:

- `.gitconfig` -> `~/projects/.gitconfig`
- `~/.claude/AGENTS.md` -> `~/projects/agent-scripts/AGENTS.md`

## Install tools

```bash

sudo apt install -y curl                             # curl - Transfer data with URLs

sudo apt install -y git                              # Git - Version control
sudo apt install -y gh                               # GitHub CLI - Interact with GitHub from the terminal

curl -LsSf https://astral.sh/uv/install.sh | sh      # uv - Python package and project manager

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash # NVM - Node.js version manager
nvm install 26.13.1                                  # Node.js - JavaScript runtime (includes npm 11.20.0)

code --install-extension ms-vscode-remote.remote-wsl # WSL - Connect VS Code to WSL environments
npm install -g @anthropic-ai/claude-code             # Claude Code - AI coding assistant

uvx duckduckgo-mcp-server --help                     # DuckDuckGo MCP Server - Web search for AI agents

```