# Name of the repo :deploy_agent_mucyo-7

## What this script (setup_project.sh)does
An automated shell script that bootstraps a Student Attendance Tracker project. It creates the full directory structure, populates all required files, allows dynamic configuration of attendance thresholds, and handles interruptions gracefully.

## How to run

bash setup_project.sh


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
## Video Walkthrough
[Click here to watch Part 1](https://www.loom.com/share/f4b04f73703a41e893c8c202a164f5c2)

## The next part of the video
[Click here to watch Part 2](https://www.loom.com/share/f8be0f003655460d88719b34f6f965c4)