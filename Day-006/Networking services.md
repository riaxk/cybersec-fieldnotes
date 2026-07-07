# Room Name: Network Services

**Platform:** TryHackMe

**Date:** 2026-07-06

**Difficulty:** Medium

---

## Objective

To understand, enumerate, and exploit common network services like SMB, Telnet, and FTP.

---

## Important Commands

### Nmap
```bash
nmap -sV <IP>
```
- Detects open ports and identifies running services.

### SMB
```bash
smbclient -L //<IP>/ -N
```
- Lists available SMB shares (anonymous login).

```bash
smbclient //<IP>/<ShareName>
```
- Connects to a specific SMB share.

### Enum4linux
```bash
enum4linux <IP>
```
- Enumerates SMB shares, users, groups, and OS information.

### Telnet
```bash
telnet <IP> <PORT>
```
Example:
```bash
telnet 10.10.10.10 23
```

### FTP
```bash
ftp <IP>
```
Example:
```bash
ftp 10.10.10.10
```

---

## Key Takeaways

- **SMB (Server Message Block)** is a Windows file-sharing protocol that typically runs on **TCP Port 445** (and older versions may also use **TCP Port 139**).
- SMB allows systems to share files, printers, and other network resources. Misconfigured SMB shares may expose sensitive data.
- Enumeration using tools like **enum4linux** and **smbclient** helps identify users, shares, operating system information, and possible attack vectors before exploitation.
- **Telnet** is a remote login protocol that runs on **TCP Port 23**. Since all communication, including usernames and passwords, is transmitted in plaintext, it is considered insecure and has largely been replaced by SSH.
- If weak or default credentials are enabled on a Telnet service, attackers may gain unauthorized remote access.
- **FTP (File Transfer Protocol)** is used for transferring files between systems and typically runs on **TCP Port 21** (control connection) and **TCP Port 20** (data connection in active mode).
- FTP does not encrypt traffic by default, making credentials vulnerable to interception. Anonymous FTP access or poor server configurations can also expose sensitive files.
- Proper enumeration is a critical step in penetration testing, as understanding the exposed services and their configurations helps identify potential vulnerabilities before attempting exploitation.

---

## Common Ports

| Service | Port |
|----------|------|
| SMB | 445/TCP (139/TCP legacy) |
| Telnet | 23/TCP |
| FTP | 21/TCP (20/TCP data transfer) |

---

## Challenges Faced

None

---

## Time Taken
1 hour