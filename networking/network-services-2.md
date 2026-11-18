# Network Services 2

**Platform:** TryHackMe

**Date:** 2026-07-07

**Difficulty:** Medium

---

## Objective

To understand, enumerate, and exploit common network services like NFS, SMTP, and MySQL.

---

## Important Commands

### Nmap
```bash
nmap -sV <IP>
```
- Detects open ports and identifies running services.

### NFS
```bash
showmount -e <IP>
```
- Lists exported NFS shares.

```bash
sudo mount -t nfs <IP>:/<share> /mnt/nfs
```
- Mounts the NFS share locally.

### SMTP
```bash
smtp-user-enum -M VRFY -U users.txt -t <IP>
```
- Enumerates valid SMTP usernames.

```bash
telnet <IP> 25
```
- Connects to the SMTP service manually.

### MySQL
```bash
mysql -h <IP> -u <username> -p
```
- Connects to the MySQL server.

---

## Key Takeaways

- **NFS (Network File System)** allows files and directories to be shared over a network and typically runs on **TCP/UDP Port 2049**.
- Misconfigured NFS shares may allow unauthorized users to access or modify files if proper permissions are not enforced.
- **SMTP (Simple Mail Transfer Protocol)** is used to send emails and commonly runs on **TCP Port 25**. User enumeration through SMTP commands can reveal valid usernames.
- **MySQL** is a relational database management system that usually runs on **TCP Port 3306**. Weak credentials or misconfigurations may allow unauthorized database access.
- Enumeration is essential for identifying exposed services, gathering information, and discovering potential attack vectors before exploitation.

---

## Common Ports

| Service | Port |
|----------|------|
| NFS | 2049/TCP, UDP |
| SMTP | 25/TCP |
| MySQL | 3306/TCP |

---

## Challenges Faced

None

---

## Time Taken
1 hour

---

> **Scope:** Notes from authorized TryHackMe training rooms. These notes summarize learning and example commands; they are not independent vulnerability disclosures or proof of exploitation.
