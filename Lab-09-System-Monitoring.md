# Bash Lab 9 - System Monitoring

## Objective

Learn how to automate basic Linux system monitoring using a Bash script.

## Script

```bash
#!/bin/bash

echo "=== SYSTEM MONITORING REPORT ==="

echo ""
echo "Hostname:"
hostname

echo ""
echo "Current User:"
whoami

echo ""
echo "System Uptime:"
uptime

echo ""
echo "Disk Usage:"
df -h

echo ""
echo "Memory Usage:"
free -h

echo ""
echo "Top Processes:"
ps aux --sort=-%cpu | head -6

echo ""
echo "Current Date and Time:"
date
```

## Commands Used

```bash
cd ~/bash-labs
nano system_monitor.sh
chmod +x system_monitor.sh
./system_monitor.sh
```

## Concepts Learned

- Checking system hostname
- Identifying the current user
- Monitoring system uptime
- Checking disk usage
- Checking memory usage
- Viewing running processes
- Sorting processes by CPU usage
- Automating system information collection

## Result

Successfully created and executed a Bash system monitoring script that collects important information about a Linux system.
