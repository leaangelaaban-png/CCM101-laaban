
# Backup Script Guide

## 1. Purpose

The `backup.sh` script automates the creation of a compressed backup of the `app-data` directory. It creates a timestamped `.tar.gz` archive inside the `backups` directory.

## 2. Full Bash Script

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. File Permissions

The command `chmod +x backup.sh` adds execute permission to the script. This allows the user to run it as a program using `./backup.sh`, provided the user has the necessary access.

## 4. Cron Schedule

The cron expression used is:

`0 2 * * * /root/backup.sh`

The five time fields mean:

- **Minute (`0`):** At minute zero.
- **Hour (`2`):** At 2 AM.
- **Day of Month (`*`):** Every day of the month.
- **Month (`*`):** Every month.
- **Day of Week (`*`):** Every day of the week.

The command runs `/root/backup.sh` every day at 2:00 AM.
