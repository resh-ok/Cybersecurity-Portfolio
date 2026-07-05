# Lab 6: Searching for Files

## Objective

The objective of this lab is to learn how to locate files and directories using Linux search commands. Efficient file searching is an essential skill for system administration and cybersecurity, where analysts often need to quickly locate log files, configuration files, scripts, or evidence during investigations.

## Learning Outcomes

By completing this lab, I learned how to:

* Search for files by name.
* Search for files by file extension.
* Search within the current directory and its subdirectories.
* Locate specific files using the `find` command.

## Commands Used

### Search for a Specific File

```bash id="o4s7hn"
find . -name "password.txt"
```

Searches the current directory and all subdirectories for a file named `password.txt`.

---

### Search for All Text Files

```bash id="x91b9r"
find . -name "*.txt"
```

Finds all files with the `.txt` extension within the current directory and its subdirectories.

---

### Search for a Directory

```bash id="r82mxy"
find . -type d -name "reports"
```

Searches for a directory named `reports`.

---

### Search for a File Only

```bash id="s5kd9g"
find . -type f -name "notes.txt"
```

Searches specifically for a file named `notes.txt`.

## Observations

* The `find` command searched recursively through the current directory and its subdirectories.
* Using wildcard characters (`*`) made it easy to locate multiple files with the same extension.
* The `-type` option allowed searches to be limited to either files or directories.
* Searching by filename was faster and more efficient than manually browsing directories.

## Security Insight

Searching for files is a common task during cybersecurity investigations. Analysts frequently locate authentication logs, configuration files, backup files, scripts, and forensic evidence across Linux systems. Mastering the `find` command enables faster incident response and more efficient system analysis.

## Summary

This lab introduced the Linux `find` command for locating files and directories. By practicing different search options, I developed the ability to efficiently locate important files within the Linux file system, an essential skill for both system administration and cybersecurity investigations.
