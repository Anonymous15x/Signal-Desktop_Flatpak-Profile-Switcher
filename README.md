# COLVDV's Signal-Desktop_Flatpak-Profile-Switcher
A simple Bash script to backup, manage, and switch between multiple Signal Desktop Flatpak profiles, allowing easy account switching without re-linking.

---

## Features

- Backup Signal Desktop Flatpak user data safely before switching profiles.  
- Switch between two profiles (`Signal1` and `Signal2`) with custom descriptions.  
- Ensures Signal Desktop is closed before switching to prevent data corruption.  
- Stores backups in `~/.signal-flatpak-backups/`.  
- Keeps track of last used profile for smooth switching.  

---

## Requirements

- Signal Desktop installed via Flatpak.  
- Linux system with Bash shell.  
- `rsync` and `pgrep` installed.  
- Signal Desktop must be closed before switching profiles.  

---

## Compatibility

This script supports **all Signal Desktop Flatpak releases**, as it works by backing up and swapping the entire Flatpak user data directory (`~/.var/app/org.signal.Signal`). It does not rely on specific internal file formats, making it compatible across versions.

---

## Installation

1. Download the latest release from the [Releases page](https://github.com/colvdv/Signal-Desktop_Flatpak-Profile-Switcher/releases/latest).

2. Open a terminal and navigate to the folder containing the downloaded script:

   ```bash
   cd /PATH/TO/DOWNLOADED/SCRIPT
   ```
   
3. Make the script executable:

   ```bash
   chmod +x COLVDV_Signal-Desktop_Flatpak-Profile-Switcher.sh
   ```

4. Ensure Signal Desktop isn't running. If it is, close it.

5. Run the script from the containing directory:

   ```bash
   ./COLVDV_Signal-Desktop_Flatpak-Profile-Switcher.sh
   ```
