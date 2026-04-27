
# 🐧 Introduction to Linux with Bash Scripting Lab

**Instructor:** Dr. Rajesh Kumar  

---

## 📌 Overview

The Linux Command Line Interface (CLI) allows users to interact with the operating system by typing commands. It provides precise control over system operations and is often faster and more powerful than graphical interfaces for many tasks.

---

## 🎯 Course Outcome Mapping

- **CO1:** Familiarity with Linux environment, command-line interface, and system utilities.

---

## 📚 Learning Outcomes

After completing this experiment, the student will be able to:

- **LO1:** Execute basic Linux system and user-level commands  
- **LO2:** Understand Linux run levels (systemd targets)  
- **LO3:** Use Linux help utilities effectively  

---

## ⚙️ Linux System Run Levels / Targets

In modern Linux distributions using `systemd`, traditional run levels are replaced by **targets**, which define the system’s operating state.

### Common Targets

- `graphical.target` → Multi-user mode with GUI  
- `multi-user.target` → Multi-user mode without GUI  
- `rescue.target` → Single-user rescue mode  
- `poweroff.target` → Shutdown system  
- `reboot.target` → Reboot system  

---

## 🛠️ Linux Help Utilities

Linux provides built-in documentation tools:

- `man` → Displays the manual page for a command  
- `--help` → Displays brief command usage  
- `Tab` → Auto-completes commands and file names  

---

## 💻 Commands Used

| Command      | Description                          |
|-------------|--------------------------------------|
| `pwd`       | Display current working directory    |
| `ls`        | List files and directories           |
| `cd`        | Change directory                     |
| `whoami`    | Display current user                 |
| `date`      | Show system date and time            |
| `uptime`    | Show system running time             |
| `man`       | Display manual pages                 |
| `--help`    | Display command help                 |
| `systemctl` | Manage system services and targets   |
| `runlevel`  | Display current run level            |
| `clear`     | Clear terminal screen                |

---

## 🔬 Procedure

1. Log in to the Linux virtual machine  
2. Open the Terminal  

### ▶️ Execute Basic Commands

```
pwd
ls
whoami
date
uptime
```

<img width="644" height="507" alt="image" src="https://github.com/user-attachments/assets/275447f5-8a73-4c2f-90af-7ea966684c6c" />

## 📂 Navigate Directories

<img width="643" height="510" alt="image" src="https://github.com/user-attachments/assets/a6114f75-6b0e-455b-8920-c89fc1f5c9fe" />


## 📖 Use Manual Pages

<img width="647" height="511" alt="image" src="https://github.com/user-attachments/assets/e210ad0a-73e1-4a52-8ff8-c96d066c0f3c" />
exit the man page by typing "q"

## ❓ Use Help Options


<img width="960" height="942" alt="Screenshot 2026-04-27 184759" src="https://github.com/user-attachments/assets/a8f43fe4-f8ee-41e6-b87d-9e4a6b9070bb" />


<img width="946" height="939" alt="Screenshot 2026-04-27 184907" src="https://github.com/user-attachments/assets/86cb61e2-dcc3-460e-918e-74c3c952e86e" />

## 🔄 Run Level / Target Management
Check Current Run Level / Target
runlevel
systemctl get-default

Switch to multi-user mode (text mode)
systemctl isolate multi-user.target

Switch to graphical mode
systemctl isolate graphical.target


⌨️ Auto-Completion
*Type part of a command and press Tab
*The system will auto-complete commands or file names
