# Laboratory 9: The Cloud Automation Engineer

## Mission Overview
In this lab, I acted as a Cloud Automation Engineer at CloudNova Technologies. I wrote a Bash script that compresses and backs up an application directory, made it executable with chmod, and scheduled it with cron to run every night at 2:00 AM.

## Objectives
- Understand Bash script syntax, including variables
- Write scripts with the nano editor
- Modify file permissions with chmod
- Understand crontab syntax and scheduling
- Document automation in Markdown
- Complete the final chapter of my GitHub portfolio

## Commands Executed
```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned
- Writing Bash scripts with variables and command substitution
- Compressing files with tar
- Managing Linux file permissions
- Scheduling recurring tasks with cron
- Documenting code and schedules

