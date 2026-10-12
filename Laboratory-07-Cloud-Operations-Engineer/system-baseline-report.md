# System Baseline Report

## Host Memory

The total RAM available on the server is 1.9 GiB, as shown by the `free -h` command. The system had 411 MiB of used memory and 1.1 GiB of free memory when checked.

## Root Filesystem Storage

The root (/) filesystem has a total capacity of 19G. The `df -h /` command showed 5.5G used and 13G available, with 30% of the filesystem currently used.

## Why Disk Space Matters

Checking disk space before a traffic surge is important because insufficient storage can affect application operations and prevent logs or other data from being written correctly. Monitoring available disk space helps engineers identify storage limitations before they affect the service.
