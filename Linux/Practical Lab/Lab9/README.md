# Lab 9: Managing Processes

## Objective

The objective of this lab is to learn how to view, monitor, and manage running processes in Linux. Understanding processes is essential for system administration and cybersecurity, as analysts often investigate running applications, identify suspicious activity, and terminate unwanted processes.

## Learning Outcomes

By completing this lab, I learned how to:

* View running processes.
* Display detailed process information.
* Monitor system processes in real time.
* Start a background process.
* Terminate a running process using its Process ID (PID).

## Commands Used

### Display Running Processes

```bash id="x0b2gh"
ps
```

Displays the processes associated with the current terminal session.

---

### Display All Running Processes

```bash id="kz9q7m"
ps aux
```

Displays detailed information about all running processes on the system.

---

### Monitor Processes in Real Time

```bash id="s8e4np"
top
```

Displays a real-time view of system processes, including CPU and memory usage.

Press **`q`** to exit the `top` interface.

---

### Start a Background Process

```bash id="m4v7ck"
sleep 300 &
```

Starts a process that runs in the background for 300 seconds.

---

### View the Background Process

```bash id="q7ny8r"
ps
```

Displays the running background process and its Process ID (PID).

---

### Terminate a Process

```bash id="j5r3bw"
kill PID
```

Terminates the process with the specified Process ID.

Replace **`PID`** with the actual process ID displayed by the `ps` command.

## Observations

* The `ps` command displayed processes running in the current terminal session.
* The `ps aux` command provided detailed information about all active processes.
* The `top` command showed system activity in real time, including CPU and memory usage.
* The `sleep` command created a background process that could be managed without affecting the terminal.
* The `kill` command successfully terminated the selected process using its PID.

## Security Insight

Monitoring processes is an important part of cybersecurity. Security analysts regularly inspect running processes to identify suspicious applications, unauthorized software, excessive resource usage, or malware. Commands such as `ps`, `top`, and `kill` are commonly used during incident response and system troubleshooting.

## Summary

This lab introduced Linux process management using the `ps`, `top`, `sleep`, and `kill` commands. By practicing these commands, I developed the ability to monitor and manage running processes, an essential skill for Linux administration and cybersecurity investigations.
