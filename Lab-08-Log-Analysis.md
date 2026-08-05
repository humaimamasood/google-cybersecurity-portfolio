# Bash Lab 8 - Log Analysis

## Objective

Learn how to analyze security logs using Bash commands and identify failed login attempts, authentication errors, and warnings.

## Sample Log

```text
INFO User login successful
INFO User login successful
WARNING Failed login attempt
INFO User login successful
ERROR Authentication failed
WARNING Failed login attempt
ERROR Authentication failed
INFO User logout
```

## Commands Used

```bash
cat security.log
grep "Failed" security.log
grep "ERROR" security.log
grep -c "Failed" security.log
grep -c "ERROR" security.log
grep -i "warning" security.log
chmod +x log_analysis.sh
./log_analysis.sh
```

## Analysis Script

```bash
#!/bin/bash

LOGFILE="security.log"

echo "=== Security Log Analysis ==="

echo ""
echo "Failed Login Attempts:"
grep -c "Failed" "$LOGFILE"

echo ""
echo "Authentication Errors:"
grep -c "ERROR" "$LOGFILE"

echo ""
echo "Warnings:"
grep -c "WARNING" "$LOGFILE"
```

## Concepts Learned

- Reading log files with `cat`
- Searching logs with `grep`
- Counting matching entries with `grep -c`
- Case-insensitive searching with `grep -i`
- Automating basic log analysis with Bash
- Identifying suspicious log patterns

## Result

Successfully analyzed a sample security log and created a Bash script to automatically count failed login attempts, authentication errors, and warnings.
