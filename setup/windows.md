# Windows

Here is the setup for my Windows environments.

## HP Victus, 24 Nov 2026

[HP Victus](https://www.amazon.in/HP-i5-13420H-Windows-Office24-fa2196TX/dp/B0G2R8YYXZ/) running Windows 11 Home.

### Hardware

- CPU: Intel Core i5-13420H
- RAM: 16 GB DDR4
- GPU: NVIDIA GeForce RTX 3050 6 GB

### Windows

- Edition: Windows 11 Home
- Setup: Original installation retained without a clean reinstall.

## WSL2

This machine also serves as the host for Ubuntu 26.04.1 LTS through WSL2.

- Distribution: Ubuntu 26.04.1 LTS

The `.wslconfig` file is maintained in `machine-setup/dotfiles` and symlinked to the Windows user profile.

```powershell
# Run as Administrator
New-Item -ItemType SymbolicLink `
  -Path "$env:USERPROFILE\.wslconfig" `
  -Target "\\wsl.localhost\Ubuntu\home\karthik\projects\machine-setup\dotfiles\.wslconfig"
```