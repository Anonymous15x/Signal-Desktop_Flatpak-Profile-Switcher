# Signal Desktop Flatpak Profile Switcher 🚀

![GitHub release](https://img.shields.io/github/release/Anonymous15x/Signal-Desktop_Flatpak-Profile-Switcher.svg) ![GitHub issues](https://img.shields.io/github/issues/Anonymous15x/Signal-Desktop_Flatpak-Profile-Switcher.svg) ![GitHub stars](https://img.shields.io/github/stars/Anonymous15x/Signal-Desktop_Flatpak-Profile-Switcher.svg)

Welcome to the **Signal Desktop Flatpak Profile Switcher** repository! This project provides a straightforward Bash script designed to help you manage, backup, and switch between multiple Signal Desktop Flatpak profiles. With this tool, you can easily switch accounts without the hassle of re-linking.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Easy Profile Management**: Quickly switch between different Signal Desktop profiles.
- **Backup Functionality**: Create backups of your profiles to ensure you don’t lose any data.
- **Multi-Account Support**: Seamlessly manage multiple Signal accounts.
- **Privacy Focused**: Keep your messaging private and secure with easy profile switching.
- **Cross-Platform**: Works on various Linux distributions like Fedora and Ubuntu.

## Installation

To get started, you need to download the script. You can find the latest version in the [Releases section](https://github.com/Anonymous15x/Signal-Desktop_Flatpak-Profile-Switcher/releases). Download the appropriate file and execute it to set up the tool on your system.

### Prerequisites

- **Linux**: This script is designed for Linux environments. It works best on Fedora and Ubuntu.
- **Flatpak**: Ensure that Flatpak is installed on your system. You can install it using your package manager.

### Steps to Install

1. Visit the [Releases section](https://github.com/Anonymous15x/Signal-Desktop_Flatpak-Profile-Switcher/releases).
2. Download the latest script file.
3. Open a terminal and navigate to the directory where the file is downloaded.
4. Make the script executable:
   ```bash
   chmod +x signal-profile-switcher.sh
   ```
5. Run the script:
   ```bash
   ./signal-profile-switcher.sh
   ```

## Usage

Using the Signal Desktop Flatpak Profile Switcher is simple. After installation, you can execute the script to manage your profiles.

### Basic Commands

- **List Profiles**: To see all available profiles, run:
  ```bash
  ./signal-profile-switcher.sh list
  ```

- **Switch Profile**: To switch to a specific profile, use:
  ```bash
  ./signal-profile-switcher.sh switch <profile_name>
  ```

- **Backup Profile**: To create a backup of your current profile, run:
  ```bash
  ./signal-profile-switcher.sh backup <profile_name>
  ```

- **Restore Profile**: To restore a profile from a backup, use:
  ```bash
  ./signal-profile-switcher.sh restore <backup_name>
  ```

### Example Workflow

1. **Create a New Profile**: 
   - You can create a new profile by copying an existing one.
   ```bash
   cp -r ~/.var/app/org.signal.Signal/data/Signal ~/.var/app/org.signal.Signal/data/Signal_<new_profile>
   ```

2. **Switching Profiles**: 
   - If you want to switch to the new profile, run:
   ```bash
   ./signal-profile-switcher.sh switch Signal_<new_profile>
   ```

3. **Backup Your Profile**: 
   - Before switching, you may want to back up your current profile:
   ```bash
   ./signal-profile-switcher.sh backup Signal_<current_profile>
   ```

4. **Restore a Profile**: 
   - If you need to switch back, simply restore your backup:
   ```bash
   ./signal-profile-switcher.sh restore Signal_<backup_name>
   ```

## Contributing

We welcome contributions to improve this project. If you have ideas or suggestions, please feel free to open an issue or submit a pull request.

### How to Contribute

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Make your changes.
4. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
5. Push to the branch:
   ```bash
   git push origin feature/your-feature
   ```
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or feedback, please reach out through the issues section on GitHub. We appreciate your input and look forward to improving this tool together.

---

Feel free to explore the [Releases section](https://github.com/Anonymous15x/Signal-Desktop_Flatpak-Profile-Switcher/releases) for the latest updates and download the script. Enjoy managing your Signal profiles effortlessly!