# 🐧 Linux File System and File Management Lab

**Instructor:** Dr. Rajesh Kumar  

---

## 📌 Theory

### 🗂️ Linux File System

Linux follows a hierarchical file system structure starting from the root directory `/`. All files and directories are organized in a tree-like structure, enabling efficient file management and security control.

---

### 📁 Files and Directories

- **Files** store data such as text, scripts, or binaries.  
- **Directories** act as containers that organize files and other directories.  

---

### 🔐 File and Directory Permissions

Linux enforces security using a permission model that defines:

- **Read (r)** → Permission to read file contents or list directory contents  
- **Write (w)** → Permission to modify a file or directory  
- **Execute (x)** → Permission to execute a file or access a directory  

Permissions are assigned to:

- **Owner**  
- **Group**  
- **Others**  

---

### ✏️ Text Editors

- **nano** → A beginner-friendly, menu-driven text editor  
- **vi** → A powerful modal editor commonly used in Unix/Linux systems  

---

## 💻 Commands Used

| Command      | Description                          |
|-------------|--------------------------------------|
| `ls`        | List files and directories           |
| `ls -l`     | Display detailed file information    |
| `pwd`       | Show current directory               |
| `cd`        | Change directory                     |
| `mkdir`     | Create directory                     |
| `rmdir`     | Remove empty directory               |
| `touch`     | Create empty file                    |
| `cat`       | Display file content                 |
| `nano`      | Edit files using nano editor         |
| `vi`        | Edit files using vi editor           |
| `chmod`     | Change file permissions              |
| `stat`      | Display file status                  |

---

## 🔬 Procedure

1. Log in to the Linux virtual machine  
2. Open the terminal  

### 📍 Display Current Directory

pwd :

<img width="942" height="234" alt="Screenshot 2026-04-27 190050" src="https://github.com/user-attachments/assets/3151239a-3c87-4ddf-b676-c3e45d909a84" />

###📂 List Files and Directories
ls 
ls -l
<img width="950" height="593" alt="image" src="https://github.com/user-attachments/assets/9aafc777-6c1e-4457-a8ae-91296df95914" />

### 📁 Create and Navigate Directory

mkdir linux_lab
cd linux_lab

<img width="950" height="241" alt="image" src="https://github.com/user-attachments/assets/7e801020-1a0e-46e5-9722-c383f1e7f9d1" />

###📄 Create Files


<img width="937" height="194" alt="image" src="https://github.com/user-attachments/assets/94388780-fc84-41fe-82f4-91c62d602fa3" />

### ✏️ Edit File Using nano
```
nano file1.txt
```

<img width="947" height="268" alt="Screenshot 2026-04-27 192040" src="https://github.com/user-attachments/assets/43e655a4-52e2-4c14-a6d2-e55fbc7035a8" />

Type some text
Press Ctrl + O to save
Press Ctrl + X to exit

### ✏️ Edit File Using vi

<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/22823a8b-086e-460c-993f-0e19b905945b" />
Press i to enter insert mode
Type text
Press Esc, then type :wq to save and exit

###📖 Display File Contents
```
cat file1.txt
```

<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/82fbdbd4-5b6b-4f4d-8012-607d55bd1371" />
🔐 Check File Permissions
```
ls -l
```

###🔧 Change File Permissions
```
chmod 755 file1.txt
```

###✅ Verify Updated Permissions
```
ls -l file1.txt
```

