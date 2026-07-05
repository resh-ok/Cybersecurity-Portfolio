# Lab 4: Viewing and Reading Files

## Objective

The objective of this lab is to learn how to view and examine the contents of files using essential Linux commands. These commands are commonly used to inspect configuration files, log files, and other text-based data during system administration and cybersecurity investigations.

## Learning Outcomes

By completing this lab, I learned how to:

* Display the entire contents of a file.
* Read large files one page at a time.
* View the beginning of a file.
* View the end of a file.
* Inspect text files efficiently using different Linux commands.

## Commands Used

### Create a Sample File

```bash
echo "Cybersecurity is interesting." > notes.txt
```

Creates a text file named `notes.txt` with sample content.

---

### Display the Entire File

```bash
cat notes.txt
```

Displays the complete contents of the file in the terminal.

---

### Read a File Page by Page

```bash
less notes.txt
```

Opens the file in an interactive viewer, allowing you to scroll through its contents.

**Useful Controls:**

* `↑` / `↓` – Scroll line by line
* `Space` – Next page
* `b` – Previous page
* `q` – Quit

---

### Display the First Lines of a File

```bash
head notes.txt
```

Displays the first 10 lines of the file by default.

To display a specific number of lines:

```bash
head -n 5 notes.txt
```

Displays the first 5 lines.

---

### Display the Last Lines of a File

```bash
tail notes.txt
```

Displays the last 10 lines of the file by default.

To display a specific number of lines:

```bash
tail -n 5 notes.txt
```

Displays the last 5 lines.

## Observations

* The `cat` command displayed the entire contents of the file.
* The `less` command allowed the file to be viewed interactively without loading all content at once.
* The `head` command quickly displayed the beginning of the file.
* The `tail` command displayed the end of the file, making it useful for monitoring logs.
* Different commands are useful depending on the size of the file and the information needed.

## Security Insight

Security analysts frequently examine log files to investigate system activity and detect suspicious behavior. Commands such as `cat`, `less`, `head`, and `tail` allow analysts to efficiently inspect configuration files, authentication logs, and application logs. In particular, `tail` is commonly used to monitor the latest log entries during incident response and troubleshooting.


## Summary

This lab introduced essential Linux commands for viewing and reading files. These commands are widely used by Linux administrators and cybersecurity professionals to inspect system files, review logs, and analyze text-based information efficiently.
