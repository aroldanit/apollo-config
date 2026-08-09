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
