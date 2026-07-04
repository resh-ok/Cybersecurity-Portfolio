# Lab 3: Creating Files and Directories

## Objective

The objective of this lab is to learn how to create, organize, and manage files and directories using basic Linux commands. These skills are essential for maintaining an organized file system and preparing environments for system administration and cybersecurity tasks.

## Learning Outcomes

By completing this lab, I learned how to:

* Create new directories.
* Create empty files.
* Create multiple directories at once.
* Create files inside specific directories.
* View directory contents recursively.
* Organize files into a structured directory hierarchy.

## Commands Used

### Create a New Directory

```bash
mkdir LinuxLab
```

Creates a new directory named `LinuxLab`.

---

### Navigate to the Directory

```bash
cd LinuxLab
```

Changes the current working directory to `LinuxLab`.

---

### Create an Empty File

```bash
touch notes.txt
```

Creates an empty file named `notes.txt`.

---

### Create Multiple Directories

```bash
mkdir logs reports evidence
```

Creates three directories in the current location:

* `logs`
* `reports`
* `evidence`

---

### Create a File Inside a Directory

```bash
touch reports/report1.txt
```

Creates a file named `report1.txt` inside the `reports` directory.

---

### View the Directory Structure

If the `tree` command is installed:

```bash
tree
```

If `tree` is not available:

```bash
ls -R
```

Displays the directory structure recursively.

## Final Directory Structure

```text
LinuxLab/
├── evidence/
├── logs/
├── notes.txt
└── reports/
    └── report1.txt
```

## Observations

* The `mkdir` command created new directories.
* The `touch` command created empty files without opening a text editor.
* Multiple directories were created using a single `mkdir` command.
* Files can be created directly inside a specific directory by providing the relative path.
* The directory structure became easier to understand using `tree` or `ls -R`.

## Security Insight

Maintaining an organized directory structure is important in cybersecurity. Analysts often separate logs, reports, scripts, and evidence into dedicated folders to keep investigations organized and prevent accidental modification or deletion of important files. Proper file organization also supports documentation, incident response, and digital forensics workflows.

## Summary

This lab introduced the fundamental Linux commands used to create and organize files and directories. Learning how to structure data efficiently is an essential skill for Linux system administration and cybersecurity, where organized storage of logs, reports, scripts, and evidence is critical for effective analysis and incident response.
