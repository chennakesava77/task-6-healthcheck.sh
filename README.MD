# System Health Check Script

## 📌 Project Overview
This project provides a **system health monitoring script (`healthcheck.sh`)** that collects key metrics like uptime, CPU load, memory, disk usage, top processes, and service status.  
It logs the output into a file (`healthlog.txt`) with a timestamp, making it useful for DevOps engineers and system admins.

---

## ⚙️ Features
- Logs:
  - System date & time
  - Uptime
  - CPU load (from `uptime`)
  - Memory usage (from `free -m`)
  - Disk usage (from `df -h`)
  - Top 5 memory-consuming processes
  - Status of critical services (e.g., `nginx`, `ssh`)
- Appends results to `healthlog.txt`
- Can be automated with **cron jobs**

---

## 📂 Files
- `healthcheck.sh` → Main script  
- `healthlog.txt` → Log file containing health reports  
- `README.md` → Documentation  

---

## 🚀 Usage

### 1. Make the script executable
```bash
chmod +x healthcheck.sh
