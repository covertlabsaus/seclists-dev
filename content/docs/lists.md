+++
title = 'Wordlist Categories'
date = '2025-09-26T21:03:00+10:00'
draft = false
+++

SecLists groups files by the type of assessment they support. Highlights include:

## Discovery

- `Discovery/DNS/` — subdomain, zone transfer, and record enumeration.
- `Discovery/Web-Content/` — common directories, files, and backup artefacts for web applications.
- `Discovery/Infrastructure/` — network services, SNMP, and IoT enumeration.

## Fuzzing

Payloads for XSS, SQL injection, command injection, SSRF, template injection, and more. Ideal for Burp, ffuf, and custom fuzzers.

## Passwords & Credentials

- `Passwords/Common-Credentials/` — curated lists of default usernames and passwords.
- `Passwords/Leaked-Databases/` — top passwords extracted from public breaches.
- `Passwords/Permutations/` — generated combos for targeted attacks.

## Usernames

Common usernames for brute-force or credential stuffing exercises.

## Payloads & Pattern Matching

- `Payloads/` — exploit strings, SSRF URLs, XML payloads, etc.
- `Pattern-Matching/` — regex signatures for sensitive data (AWS keys, RSA headers, credit cards).

## Web Shells

Reference implementations of PHP, ASPX, JSP, and other web shells to test upload filters and detection.

Explore the repository tree on GitHub for a complete breakdown, or pull the repo locally and grep for relevant keywords.
