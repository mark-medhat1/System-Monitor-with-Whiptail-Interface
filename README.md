# 🖥️ SysMon-Whiptail – Bash-Based System Monitor (Whiptail + CLI)

`SysMon-Whiptail` is a lightweight Linux system monitoring toolkit written entirely in **Bash**.

It includes **two scripts**:
- 🎛️ `sys_check_with_whiptail`: Interactive terminal-based GUI using `whiptail`
- 🧾 `sys_check_without_whiptail`: Simple, direct CLI version without a menu — ideal for cron jobs or log exports

---

## 🔧 Features

### `sys_check_with_whiptail` (Whiptail Interface)
- ✅ Live CPU usage with top processes
- 🧠 RAM usage display (`free -h`)
- 📀 Disk space usage with filesystem types
- 📡 Network statistics via `ifconfig`
- 🔥 Service checker with active/enabled status
- 📋 View recent critical system errors (`journalctl`)
- 📝 Generate and save a daily system report
- 🧑‍💻 Works for both root and normal users
- 📦 Built with pure Bash + Whiptail (no extra dependencies)

### `sys_check_without_whiptail` (CLI Version)
- 🧠 Gathers CPU, memory, disk, network, logs, services, uptime
- 📁 Saves full system report to a log file: `~/system_check.log`
- 🧩 Can be easily scheduled with `cron`
- ✅ Same backend logic, without GUI

---

## 📌 Quick Tip

> 🚀 **Want a quick system summary?**  
> In `sys_check_with_whiptail`, choose menu option `8` (Brief System Logs)  
> In `sys_check_without_whiptail`, just run the script — it prints and logs automatically.

---

## 📷 Screenshot (Whiptail Script)

<img width="604" height="425" alt="Screenshot (245)" src="https://github.com/user-attachments/assets/e7dad3e1-1abe-4785-b1d6-f2cebdf4c017" />

---

## 📁 Log Output Example

System reports are saved to:
- `~/system_monitor_brief.log` (from Whiptail interface)
- `~/system_check.log ` (from CLI version)

---

## 🛠️ Requirements

- Any modern Linux distribution
- `whiptail` (typically comes with `dialog` package)

---

## 🚀 Usage

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/SysMon-Whiptail.git
cd SysMon-Whiptail
