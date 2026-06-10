# Anlight OS 🛡️

A lightweight, elegant, **cybersecurity-focused Linux distro** by **Aegis Raid**.

Debian-based · XFCE + animated compositor · curated white-hat toolkit · one-command installs.

## ✨ What makes it Anlight
- **Beautiful & light** — XFCE tuned with `picom` (blur, rounded corners, fade & zoom animations) on a slim Debian base.
- **Powerful out of the box** — nmap, wireshark, aircrack-ng, john, hydra, hashcat, sqlmap, radare2, and more preinstalled.
- **Stupidly easy installs** — the `anlight-get` tool:
  ```bash
  anlight-get nmap                          # system package
  anlight-get pip:impacket                  # python tool
  anlight-get https://github.com/you/tool   # any github repo, auto-setup
  anlight-get metasploit                    # heavy tools, official installer
  ```

## 🏗️ How it's built
The ISO is built **in the cloud** by GitHub Actions (no big disk needed locally).
Every push to `main` triggers a build; the finished ISO is published as a **Release** download.

Manual trigger: **Actions → Build Anlight OS ISO → Run workflow**.

## 📦 Tool philosophy
The base image stays light. Massive frameworks (Metasploit, Burp, etc.) install **on demand**
via `anlight-get`, so you only carry the weight you actually use.

---
*v0.1 "Aurora" — a real, bootable foundation. Iterating toward the dream.* 🌌
