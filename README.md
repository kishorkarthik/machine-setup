# Machine-setup

Machine setup guides, configurations, dotfiles, and utility scripts.

## System setup

Here are the setup details for my laptops.

- [Linux](setup/linux.md)
- [Windows](setup/windows.md)

Tools and configurations across my machines.

- [Visual Studio Code](setup/vscode.md)

## Dropbox

Dropbox Basic is used for personal file synchronization and transferring files between my laptop and mobile devices.

Location: `C:\Users\kisho\Dropbox\`

```text
Dropbox/
├── Documents/    # Personal documents
├── Photos/       # Selected photos
└── Transfers/    # Cross-device file transfers
```

Dropbox runs natively on Windows. WSL accesses the synchronized directory through a symbolic link:

```bash
ln -s /mnt/c/Users/<username>/Dropbox ~/Dropbox
```

Note (2026-11-25): Dropbox replaces WhatsApp as the primary file-transfer mechanism between my mobile and laptop.