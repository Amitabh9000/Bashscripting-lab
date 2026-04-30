# Experiment: Virtual Terminals and Graphical System in Linux

## Course Outcome Mapping
- **CO1**: Familiarity with Linux environment and system-level components.

---

## Learning Outcomes
After completing this experiment, the student will be able to:

- **LO1**: Understand the concept of virtual terminals in Linux  
- **LO2**: Switch between multiple virtual terminals  
- **LO3**: Understand the role of the display manager and graphical login system  
- **LO4**: Identify X clients and window managers in Linux  

---

## Theory

### Virtual Terminals
Linux supports multiple virtual terminals (VTs) that allow users to access several independent terminal sessions simultaneously.  
These terminals run in text mode and are useful for system recovery and troubleshooting.

**Common key combinations:**
- `Ctrl + Alt + F1` to `Ctrl + Alt + F6` → Text-based virtual terminals  
- `Ctrl + Alt + F7` (or `F1` on some systems) → Graphical interface  

---

### Display Manager
A display manager provides the graphical login interface and manages user sessions.  
It starts the graphical server and handles authentication.

**Common display managers:**
- GDM (GNOME Display Manager)  
- LightDM  
- SDDM  

---

### X Window System
The X Window System (X11) is responsible for handling graphical display, keyboard, and mouse input.  
It enables graphical applications (X clients) to run on a Linux system.

---

### X Clients
X clients are graphical applications that communicate with the X server to display windows.

**Examples:**
- Terminal emulator  
- Web browser  
- Text editor  

---

### Window Manager
A window manager controls the placement, appearance, and behavior of windows on the screen.

**Examples:**
- GNOME Shell  
- KDE Plasma  
- Xfce  
- Openbox  

---

## Commands Used

| Command | Description |
|---------|------------|
| `tty` | Display current terminal |
| `who` | Show logged-in users |
| `w` | Show user activity |
| `startx` | Start X Window System |
| `systemctl status` | Check display manager status |
| `echo $DISPLAY` | Display X session variable |
| `ps` | View running processes |

---

## Procedure

### Step 1: Open Terminal
Log in to the Linux system and open the terminal.

---

### Step 2: Check Current Terminal
```bash
tty
```
###Step 3: Switch Virtual Terminal
press:
```
Ctrl + Alt + F1
```
Log in and verify access.

### Step 4: Return to Graphical Mode
Press: 
```bash
Ctrl + Alt + F1
```

### Step 5: Check Logged-in Users
```bash
who
```

### Step 6: Check Display Manager Status
```bash
systemctl status gdm
```

### Step 7: Verify X Session Variable
```bash
echo $DISPLAY
```

### Step 8: List X-related Processes
```bash
ps -e | grep X
```

## Screenshot
_____________
<img width="960" height="1080" alt="Screenshot 2026-04-30 185510" src="https://github.com/user-attachments/assets/97e236d5-d850-42c8-b7e5-129c745bbfc7" />
