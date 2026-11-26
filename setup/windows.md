# Windows

Here is the setup for my Windows environments.

## Configuration, 26 Nov 2026

### WSL2

This machine also serves as the host for Ubuntu 26.04.1 LTS through WSL2.

- Distribution: Ubuntu 26.04.1 LTS

The `.wslconfig` file is maintained in `machine-setup/dotfiles` and symlinked to the Windows user profile.

```powershell
# Run as Administrator
New-Item -ItemType SymbolicLink `
  -Path "$env:USERPROFILE\.wslconfig" `
  -Target "\\wsl.localhost\Ubuntu\home\karthik\projects\machine-setup\dotfiles\.wslconfig"
```

### End State

Workspace root: `~/projects` (WSL2) — the primary workspace for GitHub repositories, software development, kept within the Linux filesystem for native Linux performance and compatibility.

`C:\Users\kisho` contains:

- `Desktop/`: Windows desktop.
- `Documents/`: General and work-related documents.
- `Downloads/`: Downloaded files.
- `Pictures/`, `Videos/`, `Music/`: Personal media.
- `Dropbox/`: Synchronized personal files.
  - `Documents/`: Important personal documents.
  - `Photos/`: Selected photos.
  - `Transfers/`: Cross-device file transfers.
- Application configuration such as .config/, .claude/, .codex/ and .vscode/.

Windows-native development projects: `C:\Projects\`.

## HP Victus 15, 20 Sept 2025

[HP Victus](https://www.amazon.in/HP-i5-13420H-Windows-Office24-fa2196TX/dp/B0G2R8YYXZ/) running Windows 11 Home.

- 13th Generation Intel Core i5-13420H
- 16 GB DDR4-3200 RAM
- NVIDIA GeForce RTX 3050 (6 GB GDDR6)
- 512 GB NVMe SSD
- 39.6 cm (15.6) diagonal, FHD, IPS, anti-glare display

Setup: Original installation retained without a clean reinstall.