# Lab 8: Linux File Permissions

## Objective

The objective of this lab is to understand how Linux controls access to files and directories using file permissions. This lab introduces permission types, how to view permissions, and how to modify them using the `chmod` command.

## Learning Outcomes

By completing this lab, I learned how to:

* View file and directory permissions.
* Understand the meaning of read, write, and execute permissions.
* Modify file permissions using the `chmod` command.
* Apply numeric permission values.
* Verify permission changes.

## Commands Used

### View File Permissions

```bash id="tx58l4"
ls -l
```

Displays detailed information about files and directories, including their permissions.

---

### Create a Sample File

```bash id="f8i2rw"
touch secret.txt
```

Creates an empty file named `secret.txt`.

---

### Change File Permissions

```bash id="xm5f6o"
chmod 600 secret.txt
```

Sets the file permissions to:

* Owner: Read and Write
* Group: No permissions
* Others: No permissions

---

### Grant Read Permission to Everyone

```bash id="wz4zy6"
chmod 644 secret.txt
```

Sets the file permissions to:

* Owner: Read and Write
* Group: Read
* Others: Read

---

### Make a File Executable

```bash id="mnr0q9"
chmod 755 secret.txt
```

Sets the file permissions to:

* Owner: Read, Write, Execute
* Group: Read and Execute
* Others: Read and Execute

---

### Verify Permission Changes

```bash id="q4xjhj"
ls -l secret.txt
```

Displays the updated permissions for `secret.txt`.

## Observations

* The `ls -l` command displayed file permissions in symbolic format.
* The `chmod` command successfully modified file permissions.
* Numeric permission values made it easy to assign different permission levels.
* Permission changes were immediately reflected when viewing the file with `ls -l`.

## Security Insight

File permissions are a critical part of Linux security. They determine who can read, modify, or execute files on a system. Security analysts and system administrators regularly review and modify permissions to protect sensitive files, prevent unauthorized access, and enforce the principle of least privilege.


## Summary

This lab introduced Linux file permissions and the `chmod` command. By practicing permission management, I gained a better understanding of how Linux protects files and directories through access control, an essential concept in Linux administration and cybersecurity.
