# Experiment 11
________________

# Understanding inodes, I/O redirection, Piping, and Process control commands in Linux

## Introduction

Linux internally manages files using data structures known as inodes, which store metadata about files rather than file names. In addition, Linux provides powerful mechanisms such as input/output redirection, pipes, and process control commands to efficiently manage command execution and system resources. These concepts are fundamental for automation, scripting, system monitoring, and cyber security operations.

The problem is to understand the concept of inodes, practice I/O redirection and piping, and use process control commands to manage running processes in a Linux environment.

---

## Course Outcome Mapping

| CO | Description |
|----|-------------|
| CO1 | Familiarity with Linux system internals and file system concepts |
| CO3 | Execution and manipulation of command output using redirection, piping, and process control |

---

## Learning Outcomes

| LO | Description |
|----|-------------|
| LO1 | Understand and interpret inode information of files |
| LO2 | Use input and output redirection for managing command data |
| LO3 | Combine commands using pipes for advanced output processing |
| LO4 | Monitor and control running processes in Linux |

---

## Theory

### Inodes
An inode is a data structure that stores metadata of a file such as:
- File size
- Ownership
- Permissions
- Timestamps
- Disk location

File names are stored separately in directory entries and point to inodes.

### I/O Redirection
Redirection allows changing the standard input, output, or error streams:
- `>` – Redirect output (overwrite)
- `>>` – Redirect output (append)
- `<` – Redirect input
- `2>` – Redirect error output

### Pipes
Pipes (`|`) allow the output of one command to be used as input to another command.
Example: `ls | grep txt`

### Process Control
Linux supports multitasking. Processes can be monitored and controlled using commands such as:
- `ps`: Display running processes
- `top`: Real-time process monitoring
- `kill`: Terminate a process
- `jobs`: List background jobs
- `bg`, `fg`: Resume job in background/foreground

---

## Commands Reference

| Command | Description |
|---------|-------------|
| `ls -i` | Display inode number of files |
| `stat` | Display file inode details |
| `>` | Output redirection (overwrite) |
| `>>` | Output redirection (append) |
| `<` | Input redirection |
| `ps` | Display running processes |
| `top` | Real-time process monitoring |
| `kill` | Terminate a process |
| `jobs` | List background jobs |
| `bg` | Resume job in background |
| `fg` | Bring job to foreground |

---

## Procedure

### A. Understanding Inodes
1. Create a test file: `touch inode_test.txt`
2. Display inode number: `ls -i inode_test.txt`
3. View inode details: `stat inode_test.txt`

### B. Input / Output Redirection
4. Redirect output to a file: `ls > file_list.txt`
5. Append output: `date >> file_list.txt`
6. Redirect input: `wc -l < file_list.txt`

### C. Using Pipes
7. Combine commands using pipe: `ls -l | grep ".txt"`
8. Count number of text files: `ls | grep ".txt" | wc -l`

### D. Process Control Commands
9. Display running processes: `ps`
10. Monitor processes in real-time: `top`
11. Run a command in background: `sleep 60 &`
12. List background jobs: `jobs`
13. Bring job to foreground: `fg`
14. Terminate a process: `kill <PID>`

### Screenshot 
________________
<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/eed3c21d-a4bb-4f64-b565-baffa6937b64" />
<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/6b0e9081-73ce-4fb0-bb20-d1f695dc29a4" />
