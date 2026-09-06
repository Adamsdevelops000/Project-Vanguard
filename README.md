

#  Vanguard Sys-Utils: Quickstart Guide

Follow these steps to get Vanguard installed and monitoring your system in less than 60 seconds.

### 1. Download & Extract
Once you have downloaded the `vanguard-sys.zip` file to your **Downloads** folder, open your terminal and run:

```bash
cd ~/Downloads
unzip vanguard-sys.zip
cd vanguard-sys
```

### 2. Run the Interactive Installer
The installer will set up the system paths, install necessary dependencies (like temperature sensors and battery tools), and ask for your initial Thermal Alarm settings.

```bash
chmod +x install.sh
./install.sh
```

### 3. Activate the Command Line
After the installer finishes, you must reload your shell to activate the `sys-utils` shortcut:

```bash
source ~/.bashrc
```

---

## 🛠 How to Use Vanguard

### Opening the Main Hub
Simply type the command below to open the interactive dashboard:
```bash
sys-utils
```

### Fast-Track Commands (Pro Tip)
You don't need to navigate menus. You can jump directly to any utility by adding `command` and the number:

*   **View History:** `sys-utils command 1`
*   **Check Power/Battery:** `sys-utils command 2`
*   **Whale Hunter (Disk):** `sys-utils command 3`
*   **Reliability Monitor:** `sys-utils command 6` (See every crash since boot!)
*   **Set Temp Alarm:** `sys-utils command 7`

### Setting up Temperature Alerts
1.  Run `sys-utils`.
2.  Press **7** to set your warning temperature (e.g., 85).
3.  Press **5** to turn the **Sentinel Guard ON**. 
4.  You can now close the terminal. Vanguard will run in the background and send you a desktop notification if your PC gets too hot!

---

### Troubleshooting
*   **Permission Denied?** The script will ask for your password using the prompt: `please enter your :`. This is required to read deep system logs and hardware sensors.
*   **Sentinel not starting?** Ensure you have `libnotify-bin` installed (the installer usually handles this for you).

--- 
