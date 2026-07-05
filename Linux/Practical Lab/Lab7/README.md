# Lab 7: Searching File Contents with `grep`

## Objective

The objective of this lab is to learn how to search for specific words and patterns within text files using the `grep` command. This skill is essential for analyzing log files, configuration files, and system outputs during cybersecurity investigations.

## Learning Outcomes

By completing this lab, I learned how to:

* Search for specific words within a file.
* Search for multiple occurrences of a word or phrase.
* Perform case-insensitive searches.
* Display line numbers with search results.
* Search for patterns across multiple files.

## Commands Used

### Search for a Word in a File

```bash id="pl6r8d"
grep "Failed" auth.log
```

Searches the file `auth.log` and displays all lines containing the word **Failed**.

---

### Perform a Case-Insensitive Search

```bash id="ndjv10"
grep -i "failed" auth.log
```

Searches for the word **failed** regardless of uppercase or lowercase letters.

---

### Display Line Numbers

```bash id="4gf0l0"
grep -n "Failed" auth.log
```

Displays matching lines along with their line numbers.

---

### Count Matching Lines

```bash id="qhkptv"
grep -c "Failed" auth.log
```

Counts the number of lines containing the word **Failed**.

---

### Search Across Multiple Files

```bash id="ag1kdm"
grep "login" *.log
```

Searches all `.log` files in the current directory for the word **login**.

## Observations

* The `grep` command quickly located matching text within files.
* The `-i` option ignored letter case during searches.
* The `-n` option displayed line numbers, making it easier to locate matching entries.
* The `-c` option counted matching lines without displaying the actual content.
* Searching multiple files at once made it easier to analyze related log files.

## Security Insight

The `grep` command is one of the most frequently used tools in cybersecurity. Security analysts use it to search authentication logs, web server logs, firewall logs, and application logs for failed login attempts, suspicious IP addresses, error messages, and indicators of compromise. Efficient use of `grep` significantly speeds up incident response and forensic investigations.

## Summary

This lab introduced the Linux `grep` command for searching text within files. By practicing different search options, I developed the ability to quickly locate relevant information inside log files and text documents, an essential skill for Linux administration and cybersecurity investigations.
