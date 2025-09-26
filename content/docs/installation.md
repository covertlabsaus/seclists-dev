+++
title = 'Installation'
date = '2025-09-26T21:03:00+10:00'
draft = false
+++

SecLists is a large repository. Choose the option that fits your workflow and bandwidth.

## Download a ZIP

```bash
wget -c https://github.com/danielmiessler/SecLists/archive/master.zip -O SecLists.zip
unzip SecLists.zip
rm SecLists.zip
```

## Clone with Git

Shallow clone (faster, no history):

```bash
git clone --depth 1 https://github.com/danielmiessler/SecLists.git
```

Full clone with history:

```bash
git clone https://github.com/danielmiessler/SecLists.git
```

## Install via package manager

- **Kali Linux** — `sudo apt -y install seclists`
- **BlackArch** — `sudo pacman -S seclists`

After installation the wordlists live under `/usr/share/seclists/`.

## Verify integrity

SecLists is safe to store locally, but antivirus tools often flag the repository because it contains payloads and patterns used during testing. Whitelist the folder on sensitive systems.
