# Experiment 07 
______________

# Linux User and Group Management Lab

**Author:** Dr. Rajesh Kumar  
**Course:** Introduction to Linux with Bash Scripting Lab

---

## 1. Theory: Users in Linux
In Linux, every user is identified by specific attributes and belongs to a certain category of privileges.

### User Attributes
Every user account consists of:
* **Unique Username:** A human-readable name for the account.
* **User ID (UID):** A unique numerical identifier used by the system.
* **Home Directory:** The user's personal storage space (usually `/home/username`).
* **Default Shell:** The command-line interpreter assigned to the user (e.g., `/bin/bash`).

### Types of Users
1.  **Root User:** The superuser with full system privileges and unrestricted access.
2.  **Normal Users:** Regular accounts with limited privileges, restricted to their own files and specific system tasks.

---

## 2. Groups and Ownership
Groups are collections of users designed to simplify permission management. Instead of assigning permissions to individuals, you assign them to a group.

### File Ownership Levels
Every file or directory in Linux is associated with:
* **Owner:** The specific user who created the file or was assigned ownership.
* **Group:** A specific group that has shared access to the file.

### Special Permissions: The Sticky Bit
The **Sticky Bit** is a security flag used on shared directories. It ensures that even if multiple users have write access to a directory, they can only delete or rename files that they personally own.
* **Command:** `chmod +t directory_name`

---

## 3. Essential Commands

| Command | Description |
| :--- | :--- |
| `useradd` | Create a new user account |
| `passwd` | Set or change a user's password |
| `usermod` | Modify an existing user account |
| `userdel` | Delete a user account |
| `groupadd` | Create a new group |
| `groupdel` | Delete a group |
| `groups` | Display the groups a user belongs to |
| `chown` | Change file/directory owner and group |
| `chgrp` | Change the group ownership of a file |
| `chmod` | Change file permissions |
| `id` | Display UID, GID, and group membership for a user |

---

## 4. Lab Procedure

Follow these steps to practice user and group administration in the terminal.

### Step 1: User Creation and Verification
1.  **Log in** to your Linux system and open the **Terminal**.
2.  **Create a new user:**
    ```bash
    sudo useradd testuser
    ```
3.  **Set a password** for the new user:
    ```bash
    sudo passwd testuser
    ```
4.  **Verify the user identity:**
    ```bash
    id testuser
    ```

### Step 2: Group Management
1.  **Create a new group:**
    ```bash
    sudo groupadd testgroup
    ```
2.  **Add the user to the group** (Append mode):
    ```bash
    sudo usermod -aG testgroup testuser
    ```
3.  **Check group membership:**
    ```bash
    groups testuser
    ```

### Step 3: Shared Directory and Permissions
1.  **Create a directory:**
    ```bash
    mkdir shared_dir
    ```
2.  **Change group ownership** of the directory:
    ```bash
    sudo chgrp testgroup shared_dir
    ```
3.  **Set permissions** (Owner: rwx, Group: rwx, Others: None):
    ```bash
    sudo chmod 770 shared_dir
    ```
4.  **Apply the Sticky Bit** for security:
    ```bash
    sudo chmod +t shared_dir
    ```

### Step 4: File Ownership
1.  **Change ownership** of a specific file (setting both owner and group):
    ```bash
    sudo chown testuser:testgroup shared_file.txt
    ```

### Screenshot
_______________

<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/3ce21d6e-53de-4f31-bb34-47f88bcbde06" />
