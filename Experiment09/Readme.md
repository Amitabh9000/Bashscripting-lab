# Experiment 09
_______________

# Mounting and unmounting devices in Linux

## Introduction

Linux systems use a unified directory structure in which storage devices such as hard disks, USB drives, and external storage must be explicitly attached to the file system to access their contents. Unlike some operating systems where devices are automatically available, Linux requires administrators to understand how devices are identified, mounted, and unmounted.

The problem is to identify storage devices in Linux, mount and unmount file systems manually, and understand the significance of mounting points and device management in system administration and cyber security environments.

---

## Course Outcome Mapping

| CO | Description |
|----|-------------|
| CO1 | Familiarity with Linux system utilities and file system structure |
| CO3 | Understanding system-level operations and resource management |

---

## Learning Outcomes

| LO | Description |
|----|-------------|
| LO1 | Identify storage devices and partitions in Linux |
| LO2 | Create mount points and mount file systems manually |
| LO3 | Unmount devices safely to prevent data corruption |
| LO4 | Understand the importance of mounting in Linux system administration |

---

## Theory

### Linux File System and Mounting
Linux follows a single-rooted directory structure where all files and devices are accessible through `/`. Storage devices must be mounted to a directory (mount point) before their contents can be accessed.

### Device Files
Linux represents hardware devices as files located in the `/dev` directory. Common examples include:
- `/dev/sda`, `/dev/sdb` – Hard disks
- `/dev/sda1`, `/dev/sdb1` – Disk partitions

### Mount Points
A mount point is an empty directory where a device’s file system is attached.
Example: `/mnt`, `/media`

### Unmounting Devices
Unmounting safely disconnects the device from the file system, ensuring all data is written properly and preventing corruption.

---

## Commands Reference

| Command | Description |
|---------|-------------|
| `lsblk` | List block devices |
| `fdisk -l` | Display disk partition information |
| `mount` | Mount a file system |
| `umount` | Unmount a file system |
| `df -h` | Display mounted file systems in human-readable format |
| `mkdir` | Create mount point |
| `blkid` | Display block device attributes (UUID, type, etc.) |

---

## Procedure

### Step 1: Identifying Devices
1. Open the terminal.
2. List available block devices: `lsblk`
3. Display detailed disk information: `sudo fdisk -l`

### Step 2: Creating a Mount Point
1. Create a directory to be used as a mount point: `sudo mkdir /mnt/usb`

### Step 3: Mounting a Device
1. Mount a partition (example `/dev/sdb1`) to the mount point: `sudo mount /dev/sdb1 /mnt/usb`
2. Verify the mount: `df -h` or simply `mount`

### Step 4: Accessing the Mounted Device
1. Navigate to the mounted directory: `cd /mnt/usb`
2. List files: `ls`

### Step 5: Unmounting the Device
1. Exit the mounted directory: `cd ~`
2. Unmount the device: `sudo umount /mnt/usb`
3. Verify unmounting: `df -h`

---

## Sample Execution

```bash
$ lsblk
sda      8:0    0   50G  0 disk 
├─sda1   8:1    0   45G  0 part /
└─sda2   8:2    0    5G  0 part [SWAP]
sdb      8:16   0    8G  0 disk 
└─sdb1   8:17   0    8G  0 part 

$ sudo mkdir /mnt/usb
$ sudo mount /dev/sdb1 /mnt/usb

$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        45G   10G   33G  24% /
/dev/sdb1       8.0G  1.0G  7.0G  15% /mnt/usb
```

### Screenshot
<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/f6ba915d-9cb7-49fb-b87a-7add82f6c9ad" />
