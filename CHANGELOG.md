Changelog - Linux Backup Automation

All notable changes to the `linux-backup-automation` Ansible role will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-07-28

### Added
* ** Restic Engine Deployment:** Tasks for automated installation, initialisation, and repository configuration using AES-256 encryption.
* ** Rclone Integration:** Support for multi-destination offsite synchronisation (SFTP, Google Drive, Backblaze B2, AWS S3, GCS).
* ** Systemd Automation:** Deployed `restic-backup.service` and `restic-backup.timer` to replace legacy crontabs.
* ** Pruning & Retention Policy:** Standardised automated retention rules (7 daily, 4 weekly, 12 monthly, 1 yearly).
* ** CLI Restore Utility:** Installed `restic-restore.sh` helper utility to `/usr/local/bin` for interactive snapshot inspection and file recovery.
* ** CI Quality Enforcement:** Added `.github/workflows/lint.yml` for automated `ansible-lint` testing and status badge.
* ** Modular Provider Examples:** Created example configurations for various cloud storage targets under `examples/cloud-providers/`.
