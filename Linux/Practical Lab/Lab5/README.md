# Lab 5: Copying, Moving, and Deleting Files

## Objective

The objective of this lab is to learn how to manage files and directories using essential Linux commands. These operations are fundamental for organizing files, maintaining system data, and handling evidence during cybersecurity investigations.

## Learning Outcomes

By completing this lab, I learned how to:

* Copy files and directories.
* Move files between directories.
* Rename files and directories.
* Delete files.
* Remove empty directories.
* Remove directories containing files.

## Commands Used

### Copy a File

```bash id="cxj98t"
cp notes.txt reports/
```

Copies `notes.txt` into the `reports` directory while keeping the original file.

---

### Copy a Directory

```bash id="hcfp8d"
cp -r reports reports_backup
```

Creates a copy of the `reports` directory and all of its contents.

---

### Rename a File

```bash id="4hh3gs"
mv notes.txt linux_notes.txt
```

Renames `notes.txt` to `linux_notes.txt`.

---

### Move a File

```bash id="j0j5dt"
mv linux_notes.txt evidence/
```

Moves `linux_notes.txt` into the `evidence` directory.

---

### Delete a File

```bash id="4e5uyw"
rm temp.txt
```

Permanently removes the file `temp.txt`.

---

### Remove an Empty Directory

```bash id="jwz8c7"
rmdir empty_folder
```

Deletes an empty directory.

---

### Remove a Directory and Its Contents

```bash id="r7zgf4"
rm -r reports_backup
```

Recursively deletes the `reports_backup` directory and all files it contains.

## Observations

* The `cp` command created a duplicate file while preserving the original.
* The `cp -r` command copied an entire directory and its contents.
* The `mv` command was used to both rename and move files.
* The `rm` command permanently deleted a file.
* The `rmdir` command removed only empty directories.
* The `rm -r` command deleted a directory along with all of its contents.

## Security Insight

File management is an essential skill in cybersecurity. Analysts often copy log files before analysis to preserve the original evidence, organize investigation files into dedicated directories, and remove temporary files after completing an investigation. Understanding how to safely copy, move, and delete files helps maintain data integrity and prevents accidental loss of important evidence.

## Summary

This lab provided hands-on experience with managing files and directories in Linux. By practicing commands for copying, moving, renaming, and deleting files, I developed essential file management skills that are widely used in Linux system administration and cybersecurity workflows.
