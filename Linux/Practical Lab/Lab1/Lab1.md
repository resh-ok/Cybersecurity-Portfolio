# Lab 1: Linux Terminal Basics

## Objective

The objective of this lab is to become familiar with the Linux terminal and learn basic commands for interacting with the operating system. These commands provide the foundation for using Linux efficiently and are essential for system administration and cybersecurity tasks.

## Learning Outcomes

By completing this lab, I learned how to:

* Open and use the Linux terminal.
* Display text in the terminal.
* Identify the currently logged-in user.
* View user and group information.
* Display only the current username.

## Commands Used

### Display Text

```bash
echo "Hello, World!"
```

Displays the specified text in the terminal.

---

### Display the Current User

```bash
whoami
```

Displays the username of the currently logged-in user.

---

### Display User and Group Information

```bash
id
```

Displays the current user's:

* User ID (UID)
* Primary Group ID (GID)
* Group memberships

---

### Display Only the Username

```bash
id -un
```

Displays only the username of the current user.

## Observations

* The `echo` command successfully displayed text in the terminal.
* The `whoami` command identified the currently logged-in user.
* The `id` command displayed the user's UID, GID, and group memberships.
* The `id -un` command returned only the username, which is useful for scripting and automation.

## Security Insight

Understanding user identity is fundamental in cybersecurity. Commands such as `whoami` and `id` help security analysts verify which user account is executing commands and determine the privileges associated with that account. This information is valuable during system administration, access control verification, and incident investigations.


## Summary

This lab introduced the Linux terminal and basic user identification commands. These commands provide a strong foundation for working in Linux environments and are commonly used in cybersecurity for verifying user identities and understanding system permissions.
