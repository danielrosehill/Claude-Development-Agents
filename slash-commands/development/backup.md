# Backup

Create an on-demand backup of the current repository.

## What This Command Does

Generates a timestamped archive backup of the repository. By default, creates a tar.gz file with the naming convention:

`DDMMYYYY_HHMM_backup.tar.gz`

## Usage

Simply invoke this command. Optionally specify:
- What to include/exclude from the backup
- Alternative backup location or format
- Whether to use an existing backup target/script

## Companion Agent

This slash command pairs with the `agents/github/backup-repo.md` agent for more complex backup workflows involving remote targets or incremental backups.

## Notes

- GitHub is not a complete backup system - this provides local/offline copies
- Archives always include timestamps for versioning
- Respects .gitignore by default unless instructed otherwise
