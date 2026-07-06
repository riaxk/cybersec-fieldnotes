# Room Name: 1.DNS in detail & 2.HTTP in detail

**Platform:** TryHackMe 

**Date:** 2026-07-06

**Difficulty:** Easy 

---

## Objective

- To understand Domain Name System(DNS)
- To understand Hypertext Transfer Protocol(Http)

---

## Tools Used

- Kali linux attackbox provided by THM for practical

---

## Important Commands

HTTP:
- GET: to get information from the server
- POST: to add some information on the server
- PUT: to update some info on the server
- DELETE: to delete some information from the server

---

## Key Takeaways

DNS:
- Domain Name System is used to assign unique names to use instead of ip address numbers
- Top level domain (TLD) consists of gTLD and ccTLD
- gTLD is generic TLD like .com, .edu, .org
- ccTLD is country code TLD like .in(INDIA), .ca(Canada), .us(USA)
- Second level domain is the name eg.tryhackme and .com is TLD
- Subdomain is when a single org hosts multiple websites (max length 63, max domain name length 253)
- DNS Record types are A(for IPv4), AAAA(for IPv6), CNAME, MX(for email), TXT(for text based data)

HTTP:
- HyperText Transfer Protocol is used to communicate with website servers
- HTTPS is http secure for important and safe communication
- Uniform Resource Locator(URL) is made up of all desired information needed to be retrived or posted on a website including, scheme->user->domain name->port->path->query string->fragments
- HTTP has various status codes given as a response from the server depicting current status of request
- Headers are use to specify request or response
- Cookies are the information of a user activity on a website

---

## Time Taken

DNS: 15 mins
Http: 30 mins