# Experiment04 
________________

# Experiment: File Management Commands and I/O Redirection in Linux

## Aim
To learn and perform file management operations and input/output redirection in Linux.

---

## Theory

### File Management Commands
Linux provides several commands to manage files and directories:

- **touch** – Create empty files  
- **cp** – Copy files or directories  
- **mv** – Move or rename files  
- **rm** – Delete files or directories  
- **cat** – Display file contents  

---

### Input/Output Redirection

Redirection allows command input/output to be redirected to or from files instead of the terminal:

| Symbol | Description |
|--------|------------|
| `>`  | Redirect output (overwrite) |
| `>>` | Redirect output (append) |
| `<`  | Redirect input |

These features are essential for scripting and automation.

---

## Commands Used

| Command | Description |
|---------|------------|
| `touch` | Create empty file |
| `cp` | Copy files |
| `mv` | Move or rename files |
| `rm` | Remove files |
| `cat` | Display file contents |
| `>` | Output redirection |
| `>>` | Append output |

---

## Procedure

### Step 1: Open Terminal
Log in to the Linux system and open the terminal.

---

### Step 2: Create Working Directory
```bash
mkdir file_ops
cd file_ops
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/1701b406-6a22-479b-a807-4b44fbe0451b" />

### Step 3: Create Files
```bash
touch file1.txt file2.txt
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/84431237-8a06-4b05-98e5-b97ff7b81d2d" />

### Step 4 : Add Content using Redirecting 
```bash
echo "This is file1" > file1.txt
echo "This is file2" > file2.txt
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/f6b8a474-12c9-40b5-ab2b-8e9825353710" />

###Step 5: Display File Content
```bash
cat file1.txt
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/ef2a1c6c-db58-43d1-895b-a04481eb4942" />

###Step 6: Copy a File
```bash
cp file1.txt copy_file1.txt
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/7e3dccbe-e127-4ec6-a280-b61edcdf57dc" />

### Step 7: Rename a File
```bash
mv file2.txt renamed_file2.txt
```
<img width="953" height="1080" alt="image" src="https://github.com/user-attachments/assets/892ced87-dbd3-4c5b-b2ef-8302561243f2" />

###Step8 : Move File to Another Directory
```bash
mkdir backup
mv copy_file1.txt backup/
```
