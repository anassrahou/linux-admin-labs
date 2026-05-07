# Troubleshooting Notes

Collection of common Linux command-line and system administration issues encountered during lab practice.

---

# Permission Denied

## Problem

Unable to execute a script or access a file.

## Possible Causes

- File is not executable
- Insufficient user permissions
- Incorrect ownership

## Solutions

### Make Script Executable

```bash
chmod +x script.sh
```

### Check File Permissions

```bash
ls -l script.sh
```

### Change Ownership

```bash
sudo chown user:user script.sh
```

---

# Command Not Found

## Problem

Shell cannot locate command.

## Possible Causes

- Package not installed
- PATH variable issue
- Typographical error

## Solutions

### Verify Command Installation

```bash
which command_name
```

### Install Missing Package

```bash
sudo apt install package_name
```

### Verify PATH Variable

```bash
echo $PATH
```

---

# No Such File or Directory

## Problem

System cannot locate specified file or directory.

## Possible Causes

- Incorrect path
- File does not exist
- Wrong current directory

## Solutions

### Verify Current Directory

```bash
pwd
```

### List Files

```bash
ls -lah
```

### Search For File

```bash
find . -name filename
```

---

# Directory Not Empty

## Problem

Unable to remove directory using `rmdir`.

## Cause

Directory contains files or subdirectories.

## Solution

### Remove Recursively

```bash
rm -r directory_name
```

### Force Removal

```bash
rm -rf directory_name
```

---

# File Already Exists

## Problem

Unable to create or move file because target already exists.

## Solutions

### Verify Existing Files

```bash
ls
```

### Rename File

```bash
mv oldfile.txt newfile.txt
```

### Overwrite Carefully

```bash
cp -f source.txt target.txt
```

---

# Cannot Change Directory

## Problem

Unable to enter directory using `cd`.

## Possible Causes

- Directory does not exist
- Permission restrictions

## Solutions

### Verify Directory

```bash
ls
```

### Check Permissions

```bash
ls -ld directory_name
```

---

# Broken Symbolic Link

## Problem

Symbolic link points to invalid location.

## Verify Link

```bash
ls -l
```

## Remove Broken Link

```bash
rm symlink_name
```

## Create New Link

```bash
ln -s target_file symlink_name
```

---

# Disk Space Full

## Problem

System reports insufficient disk space.

## Solutions

### Check Disk Usage

```bash
df -h
```

### Analyze Directory Sizes

```bash
du -sh *
```

### Remove Temporary Files

```bash
sudo rm -rf /tmp/*
```

---

# Process Already Running

## Problem

Application or script already active.

## Identify Process

```bash
ps aux | grep process_name
```

## Terminate Process

```bash
kill PID
```

### Force Termination

```bash
kill -9 PID
```

---

# Incorrect File Permissions

## Problem

Users cannot access files properly.

## Verify Permissions

```bash
ls -l
```

## Modify Permissions

```bash
chmod 644 file.txt
```

## Modify Ownership

```bash
chown user:user file.txt
```

---

# Package Installation Failed

## Problem

APT installation errors or dependency issues.

## Solutions

### Update Package Lists

```bash
sudo apt update
```

### Fix Broken Dependencies

```bash
sudo apt --fix-broken install
```

### Upgrade Packages

```bash
sudo apt upgrade
```

---

# Network Connectivity Issues

## Problem

Unable to reach external systems.

## Solutions

### Test Connectivity

```bash
ping google.com
```

### Verify IP Configuration

```bash
ip a
```

### Verify DNS Resolution

```bash
nslookup google.com
```

---

# History Command Not Showing Entries

## Problem

Shell history appears empty.

## Solutions

### Verify History

```bash
history
```

### Reload Bash History

```bash
history -r
```

### Verify Shell

```bash
echo $SHELL
```

---

# Terminal Frozen

## Problem

Terminal becomes unresponsive.

## Solutions

### Interrupt Process

```bash
Ctrl + C
```

### Suspend Process

```bash
Ctrl + Z
```

### Reset Terminal

```bash
reset
```

---

# Useful Diagnostic Commands

```bash
pwd
whoami
hostname
uname -a
history
df -h
free -h
top
ip a
```
