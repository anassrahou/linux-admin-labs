# Filesystem Management

Reference guide for managing files and directories in Linux environments through the command-line interface (CLI).

---

# Filesystem Navigation

## Display Current Directory

```bash
pwd
```

Displays the current working directory.

---

## List Directory Contents

```bash
ls
```

### Detailed Listing

```bash
ls -lah
```

Options:
- `-l` → long listing format
- `-a` → show hidden files
- `-h` → human-readable sizes

---

## Change Directory

```bash
cd directory_name
```

### Move Back One Directory

```bash
cd ..
```

### Go To Home Directory

```bash
cd ~
```

### Go To Root Directory

```bash
cd /
```

---

# File Management

## Create Empty File

```bash
touch file.txt
```

---

## Copy Files

```bash
cp source.txt destination.txt
```

### Copy Directory Recursively

```bash
cp -r source_dir destination_dir
```

---

## Move or Rename Files

```bash
mv oldname.txt newname.txt
```

### Move File To Another Directory

```bash
mv file.txt /home/user/Documents
```

---

## Remove Files

```bash
rm file.txt
```

### Force File Removal

```bash
rm -f file.txt
```

---

# Directory Management

## Create Directory

```bash
mkdir directory_name
```

### Create Multiple Directories

```bash
mkdir dir1 dir2 dir3
```

### Create Nested Directories

```bash
mkdir -p parent/child/grandchild
```

---

## Remove Empty Directory

```bash
rmdir directory_name
```

### Remove Directory Recursively

```bash
rm -r directory_name
```

### Force Remove Directory

```bash
rm -rf directory_name
```

---

# File Viewing

## Display File Contents

```bash
cat file.txt
```

---

## Read Large Files

```bash
less file.txt
```

Navigation:
- `q` → quit
- `/` → search inside file

---

## Display First Lines

```bash
head file.txt
```

---

## Display Last Lines

```bash
tail file.txt
```

### Monitor File Changes

```bash
tail -f logfile.log
```

---

# File Search Operations

## Search Files By Name

```bash
find . -name filename.txt
```

---

## Search Case Insensitive

```bash
find . -iname filename.txt
```

---

## Locate Files Quickly

```bash
locate filename.txt
```

---

# Hidden Files

Hidden files begin with a dot (`.`).

Example:

```bash
.hidden_file
```

Display hidden files:

```bash
ls -a
```

---

# Symbolic Links

## Create Symbolic Link

```bash
ln -s target_file symlink_name
```

---

# File Information

## Determine File Type

```bash
file filename
```

---

## Display File Statistics

```bash
stat filename
```

---

# Disk Usage

## Display Disk Usage

```bash
df -h
```

---

## Display Directory Size

```bash
du -sh directory_name
```

---

# Security Relevance

Filesystem management is essential for:
- Linux administration
- Log analysis
- File auditing
- Malware investigation
- Incident response
- Server management

---

# Common Risks

| Risk | Description |
|---|---|
| `rm -rf` misuse | Permanent file deletion |
| Incorrect permissions | Unauthorized access |
| Wrong path operations | Accidental data loss |
| Running commands as root | System-wide impact |

---

# Best Practices

- Verify paths before deletion
- Use `ls` before `rm`
- Avoid unnecessary root usage
- Keep backups of important files
- Use recursive deletion carefully
