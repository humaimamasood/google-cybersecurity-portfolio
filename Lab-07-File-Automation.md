# Bash Lab 7 - File Automation

## Objective

Learn how to automate file and directory creation using Bash loops and commands.

## Script

```bash
#!/bin/bash

mkdir -p reports
mkdir -p logs

for i in {1..5}
do
    touch "reports/report_$i.txt"
done

for file in reports/*.txt
do
    echo "Created: $file"
done

echo "File automation completed."
```

## Commands Used

```bash
cd ~/bash-labs
nano file_automation.sh
chmod +x file_automation.sh
./file_automation.sh
ls reports
```

## Concepts Learned

- Automating directory creation
- Creating multiple files with loops
- Using `mkdir -p`
- Using `touch` in automation
- Iterating through files with a `for` loop
- Using wildcards such as `*.txt`

## Result

Successfully automated the creation of directories and multiple report files using a Bash script.
