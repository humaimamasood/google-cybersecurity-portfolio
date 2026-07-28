# Linux Lab 8 - Archive and Compression

## Objective

Learn how to create, view, and extract archives using Linux commands.

## Commands Used

```bash
mkdir archive-lab
cd archive-lab
touch report.txt
touch notes.txt
touch evidence.txt
ls
tar -cvf evidence.tar report.txt notes.txt evidence.txt
tar -tvf evidence.tar
mkdir extracted
tar -xvf evidence.tar -C extracted
ls extracted
zip evidence.zip report.txt notes.txt evidence.txt
unzip -l evidence.zip
```

## Skills Learned

- Create an archive using `tar`
- View archive contents
- Extract archive files
- Create ZIP archives
- View ZIP archive contents

## Result

Successfully created, viewed, and extracted archives using Linux commands.
