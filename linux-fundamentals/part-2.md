# Linux Fundamentals Part-2

**Platform:** TryHackMe

**Date:** 2026-07-02

**Difficulty:** Easy 

---

## Objective

- To learn to deploy your linux machine using SSH 
- To understand flags & switches
- To learn more file navigation commands
- To understand Permissions of a directory/file
- To understand common directories
---

## Important Commands

- "-a": this is used with ls to list all files (including hidden)
- "--help": This command can be used with any other command to understand what all arguments can be used with the command.
- "man": This command is used with other commands to understand all options of the command. man stands for manual
- "su": This is used to switch between users on the machine
- "touch": it is used to create a file
- "mkdir": used to create a directory/folder
- "cp": used to copy a file or folder
- "mv": used to move a file or folder to a new location
- "rm": used to remove a file or folder
- "file": used to determine the file type
---

## Key Takeaways

- Secure Shell protocol can be used to establish connection of a device using ssh hostname@ip
- Permissions can be granted using rwxrwxrwx where first set of rwx is for owner, second set for group and third set for others.
r: read
w: write
x: execute
- Common directories store all important information regarding the device.
/root: home directory of the root user (the filesystem root is /)
/etc: stores system-wide configuration files (including account information in /etc/passwd; password hashes are typically in /etc/shadow)
/var: stores logs
/tmp: stores temporary files; it is not a recycle bin.

---

---

> **Scope:** Notes from authorized TryHackMe training rooms. These notes summarize learning and example commands; they are not independent vulnerability disclosures or proof of exploitation.

## Original Lab Screenshots

![Linux command su](../assets/Day-002/Linux%20command%20su.png)

