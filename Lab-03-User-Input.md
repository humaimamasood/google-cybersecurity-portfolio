# Bash Lab 3 - User Input

## Objective

Learn how to accept and use user input in a Bash script with the `read` command.

## Script

```bash
#!/bin/bash

echo "Enter your name:"
read name

echo "Enter your favorite cybersecurity tool:"
read tool

echo "Enter your career goal:"
read goal

echo "Hello, $name!"
echo "Your favorite tool is $tool."
echo "Your career goal is $goal."
```

## Commands Used

```bash
cd ~/bash-labs
nano input.sh
chmod +x input.sh
./input.sh
```

## Concepts Learned

- Taking user input with `read`
- Storing input in variables
- Using variables in output
- Creating interactive Bash scripts

## Result

Successfully created and executed an interactive Bash script that accepts multiple inputs from the user.
