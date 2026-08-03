# Bash Lab 5 - Loops

## Objective

Learn how to use `for` and `while` loops to repeat commands and automate tasks in Bash.

## For Loop

```bash
#!/bin/bash

echo "For loop:"

for i in 1 2 3 4 5
do
    echo "Number: $i"
done
```

## File Iteration

```bash
echo "Files in current directory:"

for file in *
do
    echo "$file"
done
```

## While Loop

```bash
#!/bin/bash

count=1

while [ $count -le 5 ]
do
    echo "Count: $count"
    count=$((count + 1))
done
```

## Commands Used

```bash
cd ~/bash-labs
nano loops.sh
chmod +x loops.sh
./loops.sh

nano counter.sh
chmod +x counter.sh
./counter.sh
```

## Concepts Learned

- `for` loops
- `while` loops
- Loop variables
- Iterating through files
- Arithmetic with `$(( ))`
- Bash automation

## Result

Successfully created and executed Bash scripts using `for` and `while` loops.
