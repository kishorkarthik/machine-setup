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

```powershell
wsl --install
```

## Workspace

- `~/projects` - GitHub repos, including `machine-setup/` (this repo: shared `.gitconfig`, setup docs) and `agent-scripts/`

The workspace root also contains:

- `.gitconfig` -> `~/projects/.gitconfig`
- `~/.claude/AGENTS.md` -> `~/projects/agent-scripts/AGENTS.md`