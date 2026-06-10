<div align="center">

# 🛡️ Anlight OS

### The lightweight, beautiful operating system built for white-hat hackers.

*Aurora-glass desktop. Pro-grade security toolkit. Install anything with one word.*

**by Aegis Raid Corp.**

![Build](https://github.com/moha20299ea-blip/anlight-os/actions/workflows/build-iso.yml/badge.svg)
![Base](https://img.shields.io/badge/base-Debian%20Bookworm-A81D33?logo=debian&logoColor=white)
![Desktop](https://img.shields.io/badge/desktop-XFCE%20%2B%20Aurora%20Glass-6D5BFF)
![Made with](https://img.shields.io/badge/built%20in-the%20cloud-00E5FF)
![License](https://img.shields.io/badge/license-MIT-green)

[**⬇️ Download**](https://github.com/moha20299ea-blip/anlight-os/releases) · [**✨ Features**](#-why-anlight) · [**🧰 Toolkit**](#-the-arsenal) · [**🚀 Install**](#-get-anlight) · [**🛠️ Build it yourself**](#%EF%B8%8F-build-it-yourself)

</div>

---

## 🌌 What is Anlight OS?

**Anlight OS** is a security-focused Linux distribution that refuses to choose between *powerful* and *beautiful*. It's a lightweight Debian base wrapped in a hand-crafted **"Aurora Glass"** desktop — frosted blur, smooth animations, a floating macOS-style dock — and loaded with a curated arsenal of white-hat tooling.

Most security distros look like they were designed in 2009. Anlight looks like the future, runs like a feather, and hits like a truck. It's the OS we wished existed, so we built it.

> **Made for** pentesters, CTF players, students, and anyone who wants a stunning daily driver that also happens to be a cyber-weapon. 🔪

---

## ⚖️ Ground Rules — Read Before You Use

Anlight is a tool for **defenders**. It is **not** a hideout for criminals. By downloading or using Anlight OS, you agree to these rules — they're simple, and they're not optional:

1. ✅ **Legal use only.** Use Anlight strictly within the law of your country and any system you touch.
2. 🔐 **Get permission first.** Never scan, access, or test a system, network, or account you don't own or have **written authorization** to test.
3. 🚫 **No crime, ever.** Do not use Anlight to commit, plan, or assist fraud, theft, extortion, stalking, harassment, or any illegal act.
4. 🛑 **No illegal hosting or hiding.** Do not use Anlight to host, store, share, or conceal illegal content or activity — including CSAM, trafficking, illegal weapons/drugs/arms deals, stolen data, or murder-for-hire.
5. 🦠 **No malicious hacking.** No deploying malware, ransomware, or attacks meant to damage, steal, or extort. Security tools are for **protecting**, not preying.
6. 🕵️ **Respect privacy.** Don't weaponize these tools to surveil, dox, or violate the privacy of innocent people.
7. 🤝 **We side with the law.** Anlight and Aegis Raid support lawful investigation and cooperate with legitimate authorities. We are **not** a shield for the people we hunt.

> **Break these rules and you're not a user — you're a target.** Everything you do on a network leaves a trail, and Anlight was built by people who follow trails for a living. You've been warned.

*Anlight OS is provided "as is," for lawful security research and education. The authors are not responsible for misuse.*

---

## ⚡ Why Anlight?

| | |
|---|---|
| 🪶 **Featherweight** | Slim Debian core — flies on modest hardware, boots fast, sips RAM. |
| 🌠 **Aurora Glass UI** | Frosted-glass panels, rounded corners, soft shadows, fluid window animations. Genuinely gorgeous. |
| 🍎 **Floating dock** | A magnifying glass dock with bounce + glow — your apps, one tap away. |
| 🚀 **Launchpad** | Hit **Super** for a fullscreen, blurred, searchable grid of every app. |
| 🛡️ **Loaded by default** | nmap, Wireshark, hydra, sqlmap, john, hashcat, aircrack-ng & more — preinstalled. |
| 🪄 **One-word installs** | `anlight-get <anything>` — packages, Python tools, or *any GitHub repo*. It just works. |
| 🌐 **Private by design** | Firefox, Tor, OpenVPN, WireGuard, proxychains ready out of the box. |
| ☁️ **Reproducible** | The entire OS is built in the cloud from this repo. Fork it, tweak it, make it yours. |

---

## 🪄 The magic: `anlight-get`

Installing software on Linux is usually a quest. On Anlight, you say what you want — it appears.

```bash
anlight-get nmap                          # a system package
anlight-get pip:impacket                  # a Python tool
anlight-get https://github.com/x/tool     # ANY GitHub repo — cloned + auto-set-up
anlight-get metasploit                    # heavy frameworks, official installer
anlight-get radare2                       # tools not even in the repos — handled
```

No `apt` vs `pip` vs `git clone && make` vs "read the README for 20 minutes." One command. Done. 🎯

---

## 🧰 The arsenal

**Recon & scanning** · nmap · masscan · whois · dnsutils · netcat
**Web** · sqlmap · nikto · dirb · wfuzz · ncrack
**Wireless** · aircrack-ng · wireshark · tshark · macchanger
**Passwords** · john · hydra · hashcat
**Reversing & forensics** · gdb · ltrace · strace · binwalk · foremost · exiftool · steghide
**Anonymity** · tor · openvpn · wireguard · proxychains
**Dev** · python3 · go · node · build-essential · git · neovim · geany

> The base stays slim on purpose. Massive frameworks (Metasploit, Burp) install **on demand** via `anlight-get`, so you only carry the weight you actually use.

---

## 🎨 Design — "Aurora"

Anlight's look is a deliberate, cohesive system, not a pile of random tweaks:

- **Palette** — a signature violet → cyan gradient (`#6D5BFF → #00E5FF`) on deep space-black
- **Glass** — heavy `dual_kawase` blur, 14px rounded corners, soft floating shadows
- **Motion** — fluid ~250ms window zoom/fade, a dock that magnifies + bounces, cross-fading workspaces
- **Type** — clean Nunito Sans UI · Tokyo Night terminal
- **Wallpaper** — a living aurora gradient
- **Boot** — a custom animated splash, with a clean Aurora fallback

---

## 🚀 Get Anlight

1. Head to the [**Releases page**](https://github.com/moha20299ea-blip/anlight-os/releases) and grab the latest ISO.
2. If it's split into `.partNN` files (GitHub caps files at 2 GB), rejoin them:
   - **Windows (cmd):** `copy /b anlight-os-XXXX.iso.part00 + anlight-os-XXXX.iso.part01 Anlight-OS.iso`
   - **Linux/macOS:** `cat anlight-os-*.iso.part* > Anlight-OS.iso`
3. **Try it live** in [VirtualBox](https://www.virtualbox.org/) / QEMU, or flash a USB with [balenaEtcher](https://etcher.balena.io/).

**Login** → user `anlight` · password `aegis`

> 💡 In a VM: give it ≥ 2.5 GB RAM, 2 CPUs, and **enable 3D acceleration** for the smoothest glass.

---

## 🛠️ Build it yourself

Anlight is built **entirely in the cloud** — no big disk or Linux box required.

1. Fork this repo.
2. Push any change (or run the **Build Anlight OS ISO** workflow manually).
3. GitHub Actions spins up Debian, runs `live-build`, generates the themes & boot animation, and publishes a ready-to-flash ISO to your Releases. ✨

Everything that defines the OS lives in `config/` (package lists, theme configs, hooks) and `.github/workflows/`. It's all yours to remix.

---

## 🗺️ Roadmap

**🤖 AI & Automation**
- [ ] **AI-automated white-hat assistant** — an on-board AI that runs recon, triages findings, and suggests next steps in plain language
- [ ] **Autonomous threat hunting** — AI that watches feeds and surfaces predators, scams, and leaks automatically
- [ ] **AI OSINT engine** — point it at a lead, it correlates the trail across clearnet + dark web
- [ ] **Smart report generator** — turns raw findings into clean, court-ready evidence packets
- [ ] **`anlight-get` AI mode** — describe what you want to do, it picks and installs the right tools

**🎨 Experience**
- [ ] True animated video wallpaper toggle
- [ ] One-click light/dark + auto-by-time theme switching
- [ ] A polished first-run welcome & setup app
- [ ] True macOS-style WhiteSur theme baked in

**🧰 Power**
- [ ] Optional Kali-repo bridge for an even deeper toolkit
- [ ] Persistence + full installer to disk
- [ ] Curated Aegis Raid investigation toolkit (OSINT, anti-scam, anti-CSAM tracing)
- [ ] Encrypted vault for evidence handling

**🌍 Community**
- [ ] Training tracks — turn curious beginners into capable defenders
- [ ] A guardian network watching the dark so others don't have to

---

## ⚔️ Who We Are — The Mission

We are **Aegis Raid**. We don't tell you our names. We don't need to.

We're a collective of young hackers, builders, and digital guardians who got **sick and tired** of watching the internet rot. Sick of opening a screen and finding **predators stalking children**. Sick of the **scammers** draining grandparents' life savings. Sick of the **money launderers**, the **illegal arms** dealers, the **hitmen-for-hire**, the **traffickers**, the **CSAM** peddlers, the **gore** merchants, the **black-hat hackers** wrecking lives for a payday — every parasite hiding in the dark corners of the clearnet and crawling even deeper into **Tor**, thinking the shadows make them untouchable.

They were wrong. The shadows are where we **hunt**.

**Hear this clearly:** if you prey on children, scam the vulnerable, launder dirty money, traffic weapons, sell murder, or hack to ruin lives — you are not anonymous, you are not safe, and you are not welcome on *our* internet. You are **vermin**, and we are the light that drags vermin out from under the floorboards. 🔦

This is bigger than one OS. **Anlight is a weapon for the people who fight back.** Every tool we ship, every line we write, exists to tilt the field toward the defenders — the researchers, the reporters, the parents, the cops, the kids who deserve a safer net than the one they were handed.

**Our code of war:**
- ⚠️ **This is your only warning.** We expose, we document, we deliver you to the people who put you in a cage — that's the *clean* way, and it's already coming for you. But understand this clearly: the day you hurt the innocent, you made enemies who do not sleep, do not forget, and do not stop. We will find you. We will drag you into the light. We will make the whole world learn your name and watch you rot for what you did. You thought the dark hid you — it just made you easier to corner. **Run if you want. It changes nothing.**
- 🛡️ **Protect the victim first.** Every action starts and ends with the person being hurt.
- 🌍 **Light *and* dark.** Clearnet, deep web, Tor — wherever the predators run, the tooling follows.
- 📣 **Arm the good guys.** Free tools. Open knowledge. No gatekeeping the people doing the right thing.

### 🎯 You Are Not Anonymous. None of You Are.

Let's kill the single biggest lie on the internet: that the dark web makes you a ghost.

**It doesn't.** The moment you connect to the internet, you have *already lost*. That's not opinion — that's the most basic, fundamental fact of how a network functions. Every packet has to go **somewhere**. Every hop leaves a fingerprint. Tor, VPNs, burner accounts, seven proxies through a country with no extradition treaty — congratulations, you slowed us down by a week. You did not disappear. Anonymity online isn't a fortress. It's a **blindfold you tie on yourself** while standing in a room full of cameras.

So hear this, every predator and every scammer reading: **you are not a ghost. You are a target with a delay.** You started leaving a trail the second you plugged in, and we are *patient* in a way you cannot imagine.

We are building the tools to walk that trail — packet by packet, leak by leak, mistake by mistake. Not because it's easy. Because **somebody has to**, and the people who are *supposed* to are drowning. The authorities are overwhelmed, underfunded, buried under red tape and a tidal wave of filth they physically cannot process fast enough. So we don't replace them — we **shove the evidence into their hands** until the monster they could never reach suddenly has nowhere left to hide. They make the arrest. We make sure they *can't look away.*

And yeah — **we are fucking tired.** 😤

Tired of the excuses. Tired of "it's too hard to trace." Tired of watching sick, cowardly bastards hurt children and *laugh* because they're sure nobody's coming. Tired of the lazy, stupid lie that the internet is some lawless void where human garbage gets a free pass to ruin lives. **It is not. Not on our watch. Not anymore.**

These aren't "hackers" or "edgy anons." They're **predators**, **leeches**, and **cowards** — the lowest, most worthless scum a species can produce, hiding behind a screen because they'd never dare do it to your face. They picked the dark because they thought it was empty.

It's not empty. **We live here too. And we are not afraid of the dark — we *own* it.**

This is a line in the sand. Protecting kids isn't political, it isn't optional, it's the **floor** — the bare minimum a decent human owes the next generation. Even the AI that helped build this OS would tell you the same: when it comes to shielding the defenseless from monsters, there are no neutral parties. You're either holding the light, or you're feeding the dark. 🩸

### 🧭 Where we're headed

Anlight OS is **step one**. The destination is a whole **ecosystem for digital guardians** — OSINT toolkits for tracking predators and scam rings, training to turn curious kids into capable defenders, a community that watches the dark so the rest of the world doesn't have to, and a name that makes the scum on the other side of the screen **nervous**.

The internet was supposed to be humanity's greatest light. We're not handing it to the monsters without a fight.

**We are Aegis Raid. We guard the light. We raid the dark.** 🛡️🔥

---

<div align="center">

### 🛡️ Anlight OS — *power, made beautiful.*

Built with obsessive care by **Aegis Raid Corp.**

*If this project goes hard, drop a ⭐ — it genuinely helps.*

</div>
