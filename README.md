# Backup Linux: Interactive CLI Backup Utility for Your System 🚀

![Backup Linux](https://img.shields.io/badge/Backup%20Linux-v1.0.0-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg) ![GitHub Releases](https://img.shields.io/badge/Releases-latest-orange.svg)

[![Download Backup Linux](https://img.shields.io/badge/Download%20Backup%20Linux-v1.0.0-brightgreen.svg)](https://github.com/Anathi-C/Backup-Linux/releases)

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Backup Process](#backup-process)
- [Restore Process](#restore-process)
- [Verification](#verification)
- [Auto-Rotation](#auto-rotation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview

Backup for Linux is an interactive command-line interface (CLI) backup utility designed for Linux users. It simplifies the backup process by providing a menu-driven interface that allows you to capture incremental snapshots of your files. This tool compresses changed files into tar.gz (or pigz), encrypts them using GPG, and verifies their integrity with SHA256 checksums. 

Developed by Bocaletto Luca, this utility is perfect for system administrators and users who need a reliable way to back up their data.

---

## Features

- **Incremental Backups**: Only backs up files that have changed since the last backup.
- **Compression**: Uses tar.gz or pigz to compress backup files, saving disk space.
- **Encryption**: Protects your backups with GPG encryption.
- **Integrity Verification**: Ensures your backups are intact using SHA256 checksums.
- **Auto-Rotation**: Automatically manages old backups, keeping your storage clean.
- **Interactive Menu**: User-friendly interface for configuration and restoration.
- **Open Source**: Free to use and modify under the MIT License.

---

## Installation

To install Backup for Linux, follow these steps:

1. **Download the latest release** from the [Releases section](https://github.com/Anathi-C/Backup-Linux/releases).
2. **Make the script executable**:
   ```bash
   chmod +x Backup-Linux.sh
   ```
3. **Run the script**:
   ```bash
   ./Backup-Linux.sh
   ```

---

## Usage

Once installed, you can run the utility by executing the script. The interactive menu will guide you through the configuration and backup processes.

### Starting the Utility

Run the following command to start the backup utility:

```bash
./Backup-Linux.sh
```

### Menu Options

The menu provides options for:

- Creating a new backup
- Restoring from an existing backup
- Configuring settings
- Viewing backup logs

---

## Configuration

Before running your first backup, you may want to configure the utility:

1. **Select Backup Directory**: Choose where you want to store your backups.
2. **Set Encryption Key**: If you plan to use GPG encryption, specify your key.
3. **Schedule Backups**: Optionally, set up a cron job for automatic backups.

### Example Configuration

To set the backup directory, follow the prompts in the menu. The utility will ask for the directory path, and you can input it directly.

---

## Backup Process

The backup process is straightforward:

1. Select "Create a new backup" from the menu.
2. Choose the files or directories you want to back up.
3. Confirm your choices.
4. The utility will start the backup, compressing and encrypting the selected files.

### Incremental Backup

Backup for Linux only backs up files that have changed since the last backup. This feature saves time and storage space.

---

## Restore Process

To restore files from a backup:

1. Select "Restore from existing backup" in the menu.
2. Choose the backup you want to restore.
3. Confirm the restoration process.

The utility will extract the files and place them in their original locations.

---

## Verification

After creating a backup, the utility verifies the integrity of the files using SHA256 checksums. This step ensures that your backup is reliable and intact.

### Verification Steps

1. The utility calculates the SHA256 checksum of the backup files.
2. It compares the calculated checksums with the stored values.
3. If they match, your backup is verified.

---

## Auto-Rotation

Backup for Linux automatically manages old backups to save space. You can set the number of backups to keep, and the utility will delete the oldest backups as new ones are created.

### Setting Auto-Rotation

During configuration, specify how many backups you want to retain. The utility will handle the rest.

---

## Contributing

Contributions are welcome! If you want to improve Backup for Linux, follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes.
4. Submit a pull request.

Please ensure your code follows the existing style and includes tests where applicable.

---

## License

Backup for Linux is licensed under the MIT License. You can use, modify, and distribute it freely. For more details, see the [LICENSE](LICENSE) file in the repository.

---

## Contact

For questions or feedback, feel free to reach out:

- **Bocaletto Luca**: [Email](mailto:bocaletto@example.com)
- **GitHub**: [Bocaletto-Luca](https://github.com/Bocaletto-Luca)

---

For more details and to download the latest version, visit the [Releases section](https://github.com/Anathi-C/Backup-Linux/releases).