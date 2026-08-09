## Desktop Environment
- Chose KDE Plasma initially fro daily-driver sability and zero friction setup
- Hyprland is the target long term - better focus, keyboard-driven workflow
- Deffered until AWS AI foundations is completed, ricing is a hobby not a priority
- Migration to Hyprland should happen as a deliberate prject, not a distraction

## Pending: Filesystem + Snapshots (bundle with LUKS reinstall)
- Switch root filesystem from ext4 to btrfs at next reinstall
- Use Snapper for automated snapshots (pre/post pacman transactions, scheduled)
- Subvolume layout needed: @, @home, @snapshots minimum
- This bundles with the LUKS encryption task - both require reinstall, do them together, not separately

## Reinstall Plan - Target Date: September 1, 2026
Scope for next Arch install on apollo:
- LUKS full-disk encryption on root partition (set up at partition time)
- Btrfs root filesystem (replacing ext4) with subvolumes: @, @home, @snapshots
- Snapper configured for automated pre/post pacman snapshots
- Reuse validated choices from first install: systemd-boot, KDE Plasma (minimal group + targeted additions, not full plasma-meta blind), NetworkManager, mesa/vulkan-radeon for AMD graphics
- Pre-reqs before reinstall day: confirm all local work is pushed to GitHub (apollo-config, any other repos), Obsidian vault backed up/synced, verify SSH keys backed up or regenerate fresh post-install
