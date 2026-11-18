# Cybersecurity Lab Notes

A curated portfolio of **hands-on cybersecurity learning notes** from authorized [TryHackMe](https://tryhackme.com/) training rooms. The notes cover Linux administration, network fundamentals, web protocols, and introductory network-service enumeration.

This repository began as a short daily learning challenge in July 2026. It is now organized by topic so the work is easier to navigate and maintain. It is **not** a claim of 100 completed labs, independent vulnerability research, or professional penetration-testing engagements.

## Explore the notes

| Area | Lab | Topics |
|---|---|---|
| Linux | [Fundamentals — Part 1](linux-fundamentals/part-1.md) | Navigation, file inspection, shell operators |
| Linux | [Fundamentals — Part 2](linux-fundamentals/part-2.md) | SSH, permissions, users, directories |
| Linux | [Fundamentals — Part 3](linux-fundamentals/part-3.md) | Processes, cron, package management, logs |
| Networking | [What Is Networking?](networking/networking-basics.md) | IP, MAC, ICMP, ping |
| Networking | [DNS and HTTP](networking/dns-and-http.md) | DNS records, URLs, HTTP methods and status codes |
| Service enumeration | [Network Services](networking/network-services-1.md) | SMB, Telnet, FTP, Nmap, enum4linux |
| Service enumeration | [Network Services 2](networking/network-services-2.md) | NFS, SMTP, MySQL, showmount, smtp-user-enum |

## Tools and concepts practiced

`Linux CLI` · `SSH` · `Nmap` · `smbclient` · `enum4linux` · `Telnet` · `FTP` · `NFS` · `SMTP` · `MySQL` · `DNS` · `HTTP`

## Featured technical notes

- **[Network Services](networking/network-services-1.md):** Introductory commands for enumerating SMB shares and connecting to Telnet and FTP services.
- **[Network Services 2](networking/network-services-2.md):** Introductory enumeration of NFS exports and SMTP users, plus MySQL connectivity.

These are concise educational notes with example commands and key takeaways—not full exploitation walkthroughs or independently validated vulnerability findings.

## Evidence and responsible use

The `assets/` directory preserves screenshots from the original lab notes. Example IP addresses and commands are for authorized training environments only. Some room solutions may be restricted by their creators; check the room's rules before publishing spoilers or flags.

## Future writeups

New notes can use the [writeup template](templates/lab-writeup.md), with observations, evidence, security implications, and mitigations added **only where actually supported by completed work**.
