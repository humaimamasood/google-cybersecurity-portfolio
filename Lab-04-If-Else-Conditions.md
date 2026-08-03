# Bash Lab 4 - If/Else Conditions

## Objective

Learn how to use conditional statements in Bash to make decisions based on whether a file or directory exists.

## Script

```bash
#!/bin/bash

echo "Enter a filename or directory:"
read filename

if [ -d "$filename" ]; then
    echo "It is a directory."
elif [ -f "$filename" ]; then
    echo "It is a file."
else
    echo "It does not exist."
fi
```

## Commands Used

```bash
cd ~/bash-labs
nano check_file.sh
chmod +x check_file.sh
touch test.txt
./check_file.sh
```

## Concepts Learned

- `if` statements
- `elif` statements
- `else` statements
- `-f` file test
- `-d` directory test
- `then` and `fi`
- Conditional decision-making in Bash

## Result

Successfully created and tested a Bash script that determines whether a given path is a file, directory, or does not exist.
