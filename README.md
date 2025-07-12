# 🖥️ SysMon-Whiptail – Interactive Bash System Monitor

`SysMon-Whiptail` is a lightweight, interactive system monitoring tool built entirely in **Bash**, using `whiptail` to provide a simple terminal-based GUI.

It allows Linux users to monitor essential system metrics, check service statuses, view system logs, and generate daily system reports — all from a clean menu-driven interface.

---

## 🔧 Features

- ✅ Live CPU usage with top processes
- 🧠 RAM usage display (free -h)
- 📀 Disk space usage with filesystem types
- 📡 Network statistics via `ifconfig`
- 🔥 Service checker with active/enabled status
- 📋 View recent critical system errors (via `journalctl`)
- 📝 Generate and save a daily system brief report
- 🧑‍💻 Designed for both root and normal users (where applicable)
- 📦 100% Bash + Whiptail — no external dependencies

---

## 📌 Quick Tip

> 🚀 **Want a quick system summary?**  
> From the main menu, **choose option `8` (Brief System Logs)** for an instant overview of your system's health and performance — saved to a log file!

---

## 📷 Screenshot

<img width="604" height="425" alt="Screenshot (245)" src="https://github.com/user-attachments/assets/e7dad3e1-1abe-4785-b1d6-f2cebdf4c017" />

---

## 📁 Log Output Example

The system report is saved to:  
`~/system_monitor_brief.log`

You can customize the location in the script.

---

## 🛠️ Requirements

- Any modern Linux distribution
- `whiptail` installed (usually pre-installed with `dialog` package)

---

## 🚀 Usage

```bash
git clone https://github.com/yourusername/SysMon-Whiptail.git
cd SysMon-Whiptail
chmod +x sys_check.sh
./sys_check.sh
