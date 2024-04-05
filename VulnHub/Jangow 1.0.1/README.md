# Jangow: 1.0.1 Walkthrough

## Author Information

- **Name:** Mikhail Wilson
- **GitHub:** <https://github.com/meekthephreak>
- **Twitter:** <https://twitter.com/meekthephreak>
- **LinkedIn:** <https://www.linkedin.com>
- **Website:** <https://www.thecyberphreak.com>

## TL;DR Summary

- Retrieved user.txt and proof.txt (root flag) on the jangow 1.0.1 box.
- Key vulnerabilities exploited:
  - Insecure FTP server
  - Vulnerable Apache Web Server
  - Old Kernel Version (4.1.3 generic)

- Tools and techniques used:
  - Nmap
  - Gobuster
  - Searchsploit
  - ExploitDB
  - LinPEAS

- Major Findings:
  - Web server allowed for execution within an unsecure URL parameter
  - Exposed credentials in config.php
  - Unsecure FTP server

- Recommendations:
  - Avoid using FTP; use SFTP instead
  - Disable anonymous user file upload/retrieval
  - Keep kernel updated to the latest version

## Introduction

- **Box Name:** Jangow 1.0.1
- **Platform:** VulnHub
- **Difficulty:** Beginner
- **Objectives:** Capture the user and root flags
- **Tools Used:** Nmap, Gobuster, Searchsploit, ExploitDB, LinPEAS
