# Linux Administration Labs Roadmap

Structured hands-on Linux administration roadmap focused on command-line proficiency, system operations, troubleshooting, and cybersecurity foundations.

---

# Lab 01 — Command-Line Operations

## Objective

Develop practical experience working with files, directories, and the Linux system environment through the command-line interface (CLI).

### Concepts Covered

- Linux filesystem structure
- Terminal navigation
- File and directory management
- Command history
- Terminal efficiency
- Linux help system

### Main Commands

| Category | Commands |
|---|---|
| Navigation | pwd, cd, ls |
| File Management | touch, cp, mv, rm |
| Directory Management | mkdir, rmdir |
| File Viewing | cat, less, head, tail |
| Search | find, locate |
| Help | man, --help |
| Productivity | history, clear |

### Security Relevance

- Fundamental for Linux administration
- Required for remote server management
- Essential for incident response and log analysis
- Core skill in cybersecurity environments

---

# Lab 02 — Filesystem Management

## Objective

Understand Linux filesystem hierarchy, file organization, and storage management operations.

### Concepts Covered

- Linux directory hierarchy
- Absolute vs relative paths
- Hidden files
- Symbolic links
- Disk usage analysis

### Main Commands

| Category | Commands |
|---|---|
| Filesystem Analysis | df, du |
| File Search | find, locate |
| Links | ln |
| Path Operations | realpath |
| File Identification | file |

### Security Relevance

- Helps identify suspicious files
- Important for forensic analysis
- Essential for storage auditing

---

# Lab 03 — User and Group Management

## Objective

Practice Linux account administration and privilege management.

### Concepts Covered

- User creation
- Group management
- Password policies
- Sudo privileges
- Account security

### Main Commands

| Category | Commands |
|---|---|
| User Management | useradd, usermod, passwd |
| Group Management | groupadd, groups |
| Privileges | sudo, visudo |
| Account Information | id, whoami |

### Security Relevance

- Critical for access control
- Prevents privilege misuse
- Fundamental for system hardening

---

# Lab 04 — File Permissions and Ownership

## Objective

Understand Linux permission models and secure access control mechanisms.

### Concepts Covered

- Read/write/execute permissions
- Ownership
- Permission inheritance
- Numeric permissions
- Special permissions

### Main Commands

| Category | Commands |
|---|---|
| Permissions | chmod |
| Ownership | chown, chgrp |
| File Information | ls -l |
| Permission Analysis | stat |

### Security Relevance

- Prevents unauthorized access
- Essential for Linux security
- Common source of vulnerabilities

---

# Lab 05 — Process and Resource Management

## Objective

Monitor and manage active processes and system resource utilization.

### Concepts Covered

- Running processes
- Process lifecycle
- CPU and memory monitoring
- Background processes
- Process termination

### Main Commands

| Category | Commands |
|---|---|
| Monitoring | ps, top, htop |
| Process Control | kill, pkill |
| Background Jobs | jobs, bg, fg |
| System Usage | uptime, free |

### Security Relevance

- Detect suspicious activity
- Identify resource abuse
- Useful in incident response

---

# Lab 06 — Package Management

## Objective

Manage software packages and repositories in Linux systems.

### Concepts Covered

- Package installation
- Updates
- Dependency management
- Repository configuration

### Main Commands

| Category | Commands |
|---|---|
| Debian-based Systems | apt, dpkg |
| Repository Operations | apt update |
| Software Removal | apt remove |

### Security Relevance

- Security patch management
- Vulnerability reduction
- Software integrity maintenance

---

# Lab 07 — System Monitoring and Logs

## Objective

Monitor Linux system activity and analyze system logs.

### Concepts Covered

- Log files
- System events
- Authentication logs
- Real-time monitoring

### Main Commands

| Category | Commands |
|---|---|
| Log Analysis | journalctl, tail |
| System Information | uname, hostnamectl |
| Monitoring | watch |

### Security Relevance

- Core SOC skill
- Essential for threat detection
- Important for forensic investigations

---

# Lab 08 — Linux Networking Basics

## Objective

Practice Linux networking operations and troubleshooting techniques.

### Concepts Covered

- IP addressing
- Network interfaces
- Connectivity testing
- DNS resolution
- Port analysis

### Main Commands

| Category | Commands |
|---|---|
| Connectivity | ping |
| Interfaces | ip |
| DNS | dig, nslookup |
| Ports | ss, netstat |
| Routing | traceroute |

### Security Relevance

- Essential for network troubleshooting
- Important for traffic analysis
- Useful in threat investigations

---

# Lab 09 — SSH and Remote Access

## Objective

Configure and manage secure remote connections using SSH.

### Concepts Covered

- Remote administration
- SSH authentication
- Key-based login
- Secure file transfer

### Main Commands

| Category | Commands |
|---|---|
| Remote Access | ssh |
| Key Management | ssh-keygen |
| File Transfer | scp, sftp |

### Security Relevance

- Secure remote administration
- Prevents insecure access methods
- Critical for server management

---

# Lab 10 — Log Analysis and Incident Investigation

## Objective

Analyze Linux logs and investigate suspicious system activity.

### Concepts Covered

- Authentication logs
- Failed logins
- Service activity
- Basic incident investigation

### Main Commands

| Category | Commands |
|---|---|
| Log Filtering | grep |
| Log Reading | cat, less |
| Real-Time Analysis | tail -f |

### Security Relevance

- SOC analyst foundation
- Threat hunting basics
- Incident response workflows

---

# Lab 11 — Bash Scripting Basics

## Objective

Automate repetitive Linux administrative tasks using Bash scripting.

### Concepts Covered

- Variables
- Loops
- Conditions
- Script execution
- Automation

### Main Commands

| Category | Commands |
|---|---|
| Script Execution | bash |
| Permissions | chmod +x |
| Variables | echo |

### Security Relevance

- Improves operational efficiency
- Useful for automation
- Common in security operations

---

# Lab 12 — Service Management

## Objective

Manage Linux services and system startup behavior.

### Concepts Covered

- Services
- Daemons
- Startup processes
- Service monitoring

### Main Commands

| Category | Commands |
|---|---|
| Service Control | systemctl |
| Service Status | service |
| Boot Analysis | systemd-analyze |

### Security Relevance

- Helps identify malicious services
- Important for persistence analysis
- Essential for administration

---

# Long-Term Goals

- Build practical Linux administration skills
- Develop cybersecurity operational knowledge
- Improve troubleshooting methodology
- Create professional technical documentation
- Prepare for SOC and IT support roles
