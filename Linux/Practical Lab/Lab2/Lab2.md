# Lab 2: Linux File System Navigation

## Objective

The objective of this lab is to learn how to navigate the Linux file system using essential terminal commands. File system navigation is a fundamental Linux skill that enables users to locate files, move between directories, and understand the structure of the operating system.

## Learning Outcomes

By completing this lab, I learned how to:

* Display the current working directory.
* List files and directories.
* View detailed file information.
* Display hidden files and directories.
* Navigate between directories.
* Return to the home directory.

## Commands Used

### Display the Current Working Directory

```bash
pwd
```

Displays the full path of the current working directory.

---

### List Files and Directories

```bash
ls
```

Lists the visible files and directories in the current location.

---

### Display Detailed File Information

```bash
ls -l
```

Displays detailed information, including file permissions, owner, group, size, and last modified date.

---

### Display Hidden Files

```bash
ls -a
```

Lists all files and directories, including hidden files that begin with a period (`.`).

---

### Change Directory

```bash
cd Documents
```

Changes the current working directory to the `Documents` folder.

To move back to the previous directory:

```bash
cd ..
```

---

### Return to the Home Directory

```bash
cd
```

or

```bash
cd ~
```

Returns to the current user's home directory.

## Observations

* The `pwd` command displayed the absolute path of my current location.
* The `ls` command listed the contents of the current directory.
* Using `ls -l` provided additional details such as permissions, ownership, and file sizes.
* The `ls -a` command revealed hidden files and directories used for system and user configuration.
* The `cd` command allowed me to move between directories, while `cd ..` moved to the parent directory and `cd` returned me to my home directory.

## Security Insight

Navigating the Linux file system is an essential skill for cybersecurity professionals. Security analysts frequently move through directories to locate log files, configuration files, scripts, and evidence during investigations. Understanding directory navigation helps ensure commands are executed in the correct location and reduces the risk of modifying the wrong files.

## Summary

This lab provided hands-on experience with Linux file system navigation. By practicing essential navigation commands, I developed a stronger understanding of the Linux directory structure, which serves as a foundation for future system administration and cybersecurity tasks.
