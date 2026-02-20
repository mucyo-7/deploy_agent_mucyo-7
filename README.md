# deploy_agent_mucyo-7

## What this script does
An automated shell script that bootstraps a Student Attendance Tracker project. It creates the full directory structure, populates all required files, allows dynamic configuration of attendance thresholds, and handles interruptions gracefully.

## How to run
```bash
bash setup_project.sh
```

## What happens when you run it
1. You are prompted to enter a project name
2. The script creates `attendance_tracker_{name}/` with all required files
3. You are asked if you want to update the attendance thresholds
4. A health check verifies Python3 is installed and the structure is correct

## How to trigger the archive feature
While the script is running, press **Ctrl+C** to interrupt it. The script will:
- Bundle whatever has been created into `attendance_tracker_{name}_archive.tar.gz`
- Delete the incomplete directory
- Exit cleanly

## Requirements
- Bash
- Python3