# Signal Desktop Flatpak Profile Switcher
A simple Bash script to **back up, manage, and switch between multiple Signal Desktop accounts** installed via Flatpak on Linux (Fedora, Ubuntu, Linux Mint, etc.). Use different profiles/accounts without needing to re-link or reconfigure each time.

---

## 🚀 Features
- Switch between **multiple Signal Desktop Flatpak profiles** (e.g., work/personal accounts).
- Fully **isolated Signal accounts** with their own data directories.
- **Safe backup** of Signal Desktop user data before switching.
- Custom profile descriptions (```Signal1```, ```Signal2```, etc.).
- **Automatic check** to ensure Signal Desktop is closed before switching (prevents corruption).
- Keeps backups in ```~/.signal-flatpak-backups/ ```.
- Tracks last used profile to show current active account.

---

## 🧰 Requirements

- **Signal Desktop** installed via Flatpak.
- **Linux** system (Fedora, Ubuntu, Arch, etc.).
- ```bash```, ```rsync```, and ```pgrep``` installed _(most distros have them by default)_.
- You **must close Signal Desktop** before switching profiles.

---

## 🛠️ Compatibility

This script **works with all versions of Signal Desktop installed via Flatpak**, by backing up and replacing the user data directory at:(`~/.var/app/org.signal.Signal`). It does **not rely on internal file formats**, so it remains compatible across updates, though it is still recommended to load each profile after updating Signal Desktop.

---

## 📦 Usage Instructions

1. Download the latest script release from the [Releases page](https://github.com/colvdv/Signal-Desktop_Flatpak-Profile-Switcher/releases/latest).

2. Open a terminal and navigate to the folder containing the downloaded script:

   ```bash
   cd /PATH/TO/DOWNLOADED/SCRIPT
   ```
   
3. Make the script executable (_only needs to be done once_):

   ```bash
   chmod +x COLVDV_Signal-Desktop_Flatpak-Profile-Switcher.sh
   ```

4. Ensure Signal Desktop is **not running** (the script will also check for this).

5. Run the script:

   ```bash
   ./COLVDV_Signal-Desktop_Flatpak-Profile-Switcher.sh
   ```

6. Follow the interactive prompts to back up or switch between profiles.
