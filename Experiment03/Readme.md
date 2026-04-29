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
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/1d494123-077a-4233-be86-ea188ec9a0b4" />

### Step 2: List Files and Directories
```bash
ls
ls-a
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/fe2b6799-797c-40b7-ba76-06de4e5b0575" />

### Step 3: Create and Enter Directory
```bash
```
###Step 4: Create Files
```bash
touch file1.txt file2.txt
```
###Step 5: Edit File Using nano
``` bash
nano file1.txt
```
Type text
Press Ctrl + O to save
Press Ctrl + X to exit

###Step 6: Edit File Using vi
```bash
vi file2.txt
```
Press i (Insert mode)
Type text
Press Esc
Type :wq and press Enter
###Step 7: Display File Content
```bash
cat file1.txt
```
###Step 8: Check File Permissions
```bash
ls -l
```

###Step 9: Change File Permissions
```bash
chmod 755 file1.txt
```

###Step 10: Verify Permissions
```bash
ls -l file1.txt
```

