# Bash Lab 6 - Functions

## Objective

Learn how to create and use reusable functions in Bash scripts.

## Script

```bash
#!/bin/bash

greeting() {
    echo "Welcome to my cybersecurity lab!"
}

show_user() {
    echo "Current user: $USER"
}

check_file() {
    if [ -f "$1" ]; then
        echo "$1 is a file."
    else
        echo "$1 is not a file."
    fi
}

show_date() {
    date
}

greeting
show_user
check_file "test.txt"
show_date
```

## Commands Used

```bash
cd ~/bash-labs
nano functions.sh
chmod +x functions.sh
touch test.txt
./functions.sh
```

## Concepts Learned

- Creating Bash functions
- Calling functions
- Using function arguments
- Using `$1` for the first argument
- Reusing code through functions
- Combining functions with conditional statements

## Result

Successfully created and executed a Bash script containing multiple reusable functions.
