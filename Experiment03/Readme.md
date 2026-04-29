# Experiment 03 
________________
# Experiment: Linux File System and Basic Commands

## Aim
To understand the Linux file system structure and perform basic file and directory operations using commands.

---

## Theory

### Linux File System
Linux follows a hierarchical file system structure starting from the root directory `/`.  
All files and directories are organized in a tree-like structure, enabling efficient file management and security control.

---

### Files and Directories
- **Files**: Store data such as text, scripts, or binaries  
- **Directories**: Containers that organize files and other directories  

---

### File and Directory Permissions

Linux enforces security using a permission model:

| Permission | Meaning |
|------------|--------|
| r (Read)   | Read file contents / list directory |
| w (Write)  | Modify file or directory |
| x (Execute)| Execute file / access directory |

Permissions are assigned to:
- Owner  
- Group  
- Others  

---

### Text Editors

- **nano** – Beginner-friendly text editor  
- **vi** – Advanced and powerful editor  

---

## Commands Used

| Command | Description |
|---------|------------|
| `ls` | List files and directories |
| `ls -l` | Detailed file information |
| `pwd` | Show current directory |
| `cd` | Change directory |
| `mkdir` | Create directory |
| `rmdir` | Remove empty directory |
| `touch` | Create empty file |
| `cat` | Display file content |
| `nano` | Edit file using nano |
| `vi` | Edit file using vi |
| `chmod` | Change file permissions |
| `stat` | Display file status |

---

## Procedure

### Step 1: Open Terminal and Check Current Directory
```bash
pwd
