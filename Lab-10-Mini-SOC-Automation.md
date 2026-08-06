# Bash Lab 10 - Mini SOC Automation Project

## Objective

Build a basic SOC automation script that analyzes security logs and generates a security report.

## Scenario

A junior SOC analyst needs to review security events and quickly identify failed login attempts, authentication errors, and warnings.

## Security Log

```text
INFO User login successful
WARNING Failed login attempt
INFO User login successful
ERROR Authentication failed
WARNING Failed login attempt
INFO User logout
ERROR Authentication failed
INFO User login successful
WARNING Failed login attempt
```

## Bash Script

```bash
#!/bin/bash

LOGFILE="soc.log"
REPORT="soc_report.txt"

echo "=== SOC SECURITY REPORT ===" > "$REPORT"

echo "" >> "$REPORT"
echo "Date and Time:" >> "$REPORT"
date >> "$REPORT"

echo "" >> "$REPORT"
echo "Hostname:" >> "$REPORT"
hostname >> "$REPORT"

echo "" >> "$REPORT"
echo "Current User:" >> "$REPORT"
whoami >> "$REPORT"

echo "" >> "$REPORT"
echo "Failed Login Attempts:" >> "$REPORT"
grep -c "Failed" "$LOGFILE" >> "$REPORT"

echo "" >> "$REPORT"
echo "Authentication Errors:" >> "$REPORT"
grep -c "ERROR" "$LOGFILE" >> "$REPORT"

echo "" >> "$REPORT"
echo "Warnings:" >> "$REPORT"
grep -c "WARNING" "$LOGFILE" >> "$REPORT"

echo "" >> "$REPORT"
echo "Failed Login Details:" >> "$REPORT"
grep "Failed" "$LOGFILE" >> "$REPORT"

echo "" >> "$REPORT"
echo "=== END OF REPORT ===" >> "$REPORT"

cat "$REPORT"
```

## Commands Used

```bash
cd ~/bash-labs
nano soc.log
nano soc_monitor.sh
chmod +x soc_monitor.sh
./soc_monitor.sh
cat soc_report.txt
```

## Concepts Learned

- Bash variables
- File input and output
- `grep` for log analysis
- Counting security events
- Generating automated reports
- Using `>` to create/overwrite files
- Using `>>` to append data
- Collecting system information
- Basic SOC automation

## Result

Successfully created a Bash-based SOC monitoring tool that analyzes security logs and automatically generates a security report containing important security events and system information.
