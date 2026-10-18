
# Mission 9: The Cloud Automation Engineer

## Mission Overview

This mission focuses on automating routine cloud operations using a Bash script and the Linux cron scheduler. A backup script was created to compress sample application data into a timestamped archive and schedule the backup to run automatically.

## Objectives

- Understand Bash scripts, variables, and cron jobs.
- Create and execute a backup script.
- Use `chmod` to grant execution permission.
- Schedule an automated backup using crontab.
- Document the script and its schedule in Markdown.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Bash scripting and variable usage.
- File permissions in Linux.
- Creating compressed `.tar.gz` backups.
- Scheduling automated tasks with cron.
- Writing technical documentation in Markdown.
