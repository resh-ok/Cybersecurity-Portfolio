# Lab 12: Archiving and Compressing Files

## Objective

The objective of this lab is to learn how to archive and compress files and directories using Linux commands. Archiving is commonly used to back up data, preserve evidence, and transfer files efficiently in system administration and cybersecurity.

## Learning Outcomes

By completing this lab, I learned how to:

* Create an archive using the `tar` command.
* Compress an archive using `gzip`.
* Extract archived files.
* List the contents of an archive without extracting it.
* Verify archived and extracted files.

## Commands Used

### Create a Tar Archive

```bash id="n8q5xw"
tar -cvf backup.tar reports/
```

Creates an archive named `backup.tar` containing the `reports` directory.

---

### Create a Compressed Tar Archive

```bash id="g4m7zr"
tar -czvf backup.tar.gz reports/
```

Creates a compressed archive named `backup.tar.gz` using `gzip`.

---

### List Archive Contents

```bash id="j3v9pk"
tar -tvf backup.tar
```

Displays the contents of the archive without extracting it.

---

### Extract an Archive

```bash id="r6w1yt"
tar -xvf backup.tar
```

Extracts the contents of `backup.tar` into the current directory.

---

### Extract a Compressed Archive

```bash id="f2n8mq"
tar -xzvf backup.tar.gz
```

Extracts the contents of the compressed archive.

## Observations

* The `tar` command combined multiple files and directories into a single archive.
* Using the `-z` option compressed the archive with `gzip`, reducing its file size.
* The `-t` option displayed archive contents without extracting them.
* Extracting archives restored the original files and directory structure.

## Security Insight

Archiving is widely used in cybersecurity to preserve log files, forensic evidence, and system backups. Compressing files reduces storage space and simplifies file transfers while maintaining the integrity of collected data. Security professionals often archive investigation artifacts before sharing or storing them for long-term retention.

## Summary

This lab introduced the Linux `tar` command for archiving and compressing files and directories. By practicing archive creation, compression, and extraction, I developed essential file management skills used for backups, data preservation, and cybersecurity investigations.
