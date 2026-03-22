# Linux Sysadmin Assignment

## Overview
This repository contains the implementation of a Linux system administration assignment focused on setting up and managing development environments for two new developers, Sarah and Mike. The assignment covers system monitoring, user management, access control, and automated backup procedures for web servers.

## Tasks Completed

### Task 1: System Monitoring Setup
- **Objective**: Configure monitoring tools to track CPU, memory, processes, and disk usage for system health and performance.
- **Implementation**:
  - Installed and configured `htop` and `nmon` for real-time monitoring of system resources.
  - Set up disk usage monitoring using `df` and `du` commands.
  - Implemented logging of system metrics to `system_metrics_logs.txt`.
  - Created screenshots demonstrating the monitoring setup and tools in action.
- **Files**: 
  - `task1/system_metrics_logs.txt` - Log file containing system metrics
  - `task1/htop.png` - Screenshot of htop monitoring
  - `task1/nmon.png` - Screenshot of nmon monitoring
  - `task1/monitoring_setup1.png` & `task1/monitoring_setup2.png` - Setup screenshots

### Task 2: User Management and Access Control
- **Objective**: Create secure user accounts for Sarah and Mike with proper access controls and password policies.
- **Implementation**:
  - Created user accounts for Sarah and Mike with secure passwords.
  - Set up isolated working directories:
    - Sarah: `/home/Sarah/workspace`
    - Mike: `/home/mike/workspace`
  - Configured appropriate permissions to ensure only respective users can access their directories.
  - Implemented password policy with expiration (30 days) and complexity requirements.
- **Files**:
  - `task2/user_mgmt_1.png` & `task2/user_mgmt_2.png` - Screenshots of user creation and setup

### Task 3: Backup Configuration for Web Servers
- **Objective**: Set up automated backups for Apache (Sarah) and Nginx (Mike) web servers.
- **Implementation**:
  - Created backup scripts for:
    - Sarah: Apache configuration (`/etc/httpd/`) and document root (`/var/www/html/`)
    - Mike: Nginx configuration (`/etc/nginx/`) and document root (`/usr/share/nginx/html/`)
  - Configured cron jobs to run backups every Tuesday at 12:00 AM.
  - Backups are saved as compressed files in `/backups/` with naming convention: `{server}_backup_YYYY-MM-DD.tar.gz`
  - Implemented backup integrity verification by listing contents of compressed files.
- **Files**:
  - `task3/backup_setup.png` - Backup setup screenshot
  - `task3/backup_task1.png` - Backup task execution screenshot
  - `task3/sarah_mike_backup_script.png` - Backup script screenshot

## Challenges Encountered
- Ensuring proper permissions and ownership for user directories
- Configuring cron jobs with correct timing and paths
- Verifying backup integrity and compression

## Submission
This assignment has been completed and is ready for submission via Vlearn with the GitHub repository link.