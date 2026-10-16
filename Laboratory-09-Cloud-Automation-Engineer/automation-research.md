# Automation Research

## 1. Bash Script
A Bash script is a text file containing a series of shell commands that run in order, letting you automate tasks you would otherwise type by hand. The shebang line `#!/bin/bash` at the top tells the operating system to use the Bash interpreter to run the file.

## 2. Variables
Variables store a value, such as a folder path, once so it can be reused throughout a script. Using something like `$BACKUP_DIR` instead of typing the path every time reduces typing mistakes, and if the path changes, only one line needs to be updated.

## 3. Cron Job
A cron job is a task scheduled in Linux to run automatically at set times, managed by the cron service. It is essential for cloud operations because repetitive work like backups, log cleanup, and updates can run on schedule without anyone remembering to do it.
