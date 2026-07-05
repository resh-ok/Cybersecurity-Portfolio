# Lab 11: Viewing System Logs

## Objective

The objective of this lab is to learn how to view and analyze system log files in Linux. System logs record important events such as user authentication, system activity, and service messages, making them a valuable source of information during troubleshooting and cybersecurity investigations.

## Learning Outcomes

By completing this lab, I learned how to:

* View system logs using `journalctl`.
* Display the most recent log entries.
* View authentication logs.
* Read log files using `cat`.
* Understand the importance of system logs in cybersecurity.

## Commands Used

### View System Logs

```bash id="k7h8qt"
journalctl
```

Displays all system logs managed by `systemd`.

Press **`q`** to exit the log viewer.

---

### Display the Most Recent Log Entries

```bash id="34s5vn"
journalctl -n 20
```

Displays the last 20 log entries.

---

### View Authentication Logs (Ubuntu)

```bash id="g6m2wp"
cat /var/log/auth.log
```

Displays authentication-related events such as logins and authentication attempts.

> **Note:** Some systems may require `sudo`:

```bash id="m9r1kc"
sudo cat /var/log/auth.log
```

---

### Search Authentication Logs (Optional)

```bash id="c5x9rd"
grep "Failed" /var/log/auth.log
```

Searches the authentication log for failed login attempts.

## Observations

* The `journalctl` command displayed system events collected by `systemd`.
* The `journalctl -n 20` command quickly showed the most recent log entries.
* The authentication log contained records of login and authentication events.
* Using `grep` made it easier to locate specific events within large log files.

## Security Insight

System logs are one of the primary sources of evidence during cybersecurity investigations. Security analysts review authentication logs, service logs, and system events to identify failed login attempts, unauthorized access, system errors, and suspicious activity. Regular log analysis is essential for incident detection, forensic investigations, and security monitoring.

## Summary

This lab introduced Linux system logging using `journalctl` and authentication log analysis. By learning how to access and inspect system logs, I developed foundational skills for troubleshooting Linux systems and investigating security-related events.
