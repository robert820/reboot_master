<div align="center">

<a href="https://blog.dei3c.com/2026/09/reboot-master.html" target="_blank" rel="noopener noreferrer">
  <img src="https://github.com/user-attachments/assets/2830eb70-512c-4ddb-87ec-5213a6e465b1" alt="DEI3C | Reboot Master" height="70" />
</a>

<br /><br />

[繁體中文](../../README.md) · [简体中文](README_zh-CN.md) · **English**

# Reboot Master

### Lightweight, Secure & Powerful Windows Power and Boot Management Utility
Designed for Daily Use, PC Maintenance, and WinPE Rescue Environments

[![Platform](https://img.shields.io/badge/Platform-Windows%207%20%7C%208%20%7C%2010%20%7C%2011%20%7C%20WinPE-blue?style=flat-square&logo=windows)](https://github.com/robert820/reboot_master)
[![Type](https://img.shields.io/badge/Type-Freeware%20%7C%20Portable-success?style=flat-square)](#-download--usage)
[![UI](https://img.shields.io/badge/GUI-Modern%20Responsive%20UI-blueviolet?style=flat-square)](#)
[![Download](https://img.shields.io/badge/Download-GitHub%20Releases-blue?style=flat-square&logo=github)](https://github.com/robert820/reboot_master/releases)

**Stop smashing keys. Stop getting stuck in infinite Safe Mode loops. One click for all Windows boot actions.**

[Features](#-features) · [Download & Usage](#-download--usage) · [Emergency CLI](#-emergency-rescue-cli) · [Requirements](#-system-compatibility--requirements) · [FAQ](#-frequently-asked-questions-faq) · [Feedback](#-issues--feedback)

</div>

---

## 📖 Overview

Have you ever struggled with these common Windows startup headaches?
- Repeatedly mashing Delete or F2 upon rebooting, yet missing the brief window to enter BIOS/UEFI Setup?
- Booting into Safe Mode to troubleshoot, only to find yourself trapped in an **infinite Safe Mode reboot loop** due to keyboard driver issues or corrupted settings?
- Searching endlessly for menus just to temporarily disable Driver Signature Enforcement or Memory Integrity when testing custom drivers?
- Needing a quick and reliable way to switch boot media inside a WinPE maintenance flash drive?

**Reboot Master** was created to eliminate all these hassles. Portable, zero-install, and ad-free, it makes complex Windows power and boot configurations simple and intuitive.

---

## ✨ Features

### 1. ⚡ One-Click Reboot to BIOS / UEFI
- No more key-mashing or guessing motherboard shortcut keys. Click one button and your PC will automatically boot straight into BIOS/UEFI Setup on restart.
- Built-in hardware check: gracefully detects Legacy BIOS (MBR) and provides clear guidance.

### 2. 🛡️ One-Time Safe Mode (Loop-Proof Design)
- **Eliminate Infinite Safe Mode Loops**: Traditional tools can lock Windows into Safe Mode, preventing a return to normal desktop mode.
- **Single-Boot Protection**: Safe Mode is applied strictly to the *next restart only*. **Once you finish troubleshooting, simply restart your PC normally and you'll return straight to your standard Windows desktop seamlessly!**
- Supports both "Minimal Safe Mode" and "Safe Mode with Networking".

### 3. 🛠️ One-Click Advanced Boot Options (WinRE)
- Quickly restart directly into the Windows Advanced Troubleshooting Menu to perform System Restore, Startup Repair, or open Command Prompt.

### 4. 🚀 Quick USB Boot
- Automatically scans connected bootable USB drives and external storage.
- Allows you to reboot straight from a designated USB flash drive without having to modify BIOS boot priority orders manually.

### 5. 🔐 Driver Signature & Core Security Controls
- **Test Mode**: Easily toggle Windows Test Mode on or off.
- **Disable Driver Signature Enforcement**: Convenient for installing uncertified hardware drivers or development software.
- **Memory Integrity (Core Isolation)**: Toggle core isolation protection easily to eliminate compatibility issues with specialized performance tools.

### 6. 🔌 Fast Native Shutdown & Reboot
- Instantaneous power execution, preventing hanging processes or unresponsive shutdowns.

### 7. 💽 Full WinPE Native Support
- Fully compatible with system maintenance USB drives (WinPE), automatically detecting physical OS drives for hassle-free repairs.
- Display compatibility fallback ensures reliable rendering in any rescue environment.

### 8. 🌐 Complete 31-Language Support & Modern UI
- **Native Support for 31 Languages Worldwide**: Automatically detects Windows display language or can be changed anytime in settings:
  | Region                      | Supported Languages (All 31 Included)                                                                                                                                                                                                                                       |
  | :-------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  | **East Asia**               | 繁體中文 (Traditional Chinese), 简体中文 (Simplified Chinese), 日本語 (Japanese), 한국어 (Korean)                                                                                                                                                                           |
  | **Europe**                  | English, Français (French), Deutsch (German), Español (Spanish), Italiano (Italian), Português (Portuguese), Русский (Russian), Українська (Ukrainian), Polski (Polish), Svenska (Swedish), Magyar (Hungarian), Ελληνικά (Greek), Català (Catalan), Беларуская (Belarusian) |
  | **Middle East & West Asia** | العربية (Arabic), فارسی (Persian), עברית (Hebrew), Türkçe (Turkish), Kurdî (Kurdish)                                                                                                                                                                                        |
  | **Southeast Asia & Others** | ไทย (Thai), Bahasa Indonesia (Indonesian), Azərbaycanca (Azerbaijani), Српски (Serbian Cyrillic), Srpski (Serbian Latin), Тоҷикӣ (Tajik), Ўзбекча (Uzbek Cyrillic), Oʻzbekcha (Uzbek Latin)                                                                                 |
- **Modern Themes**: Seamless Dark Mode, Light Mode, and System Theme following.
- **Live Operation Log**: Complete transparency with real-time in-app logging.

---

## 📦 Download & Usage

### How to Download
1. Download the latest `reboot_master.exe` from [GitHub Releases](https://github.com/robert820/reboot_master/releases).
2. The application is a **single portable standalone executable** requiring zero installation or dependencies.

### How to Run
1. Double left-click `reboot_master.exe` to execute.
2. Click any action card on the dashboard (e.g. Reboot to BIOS, Safe Mode, USB Boot).
3. Confirm the action in the prompt dialog.

---

## 🖥️ System Compatibility & Requirements

- **Operating System**: Windows 11 / 10 / 8.1 / 8 / 7 (SP1) & Windows PE
- **Architecture**: 64-bit (x64) and 32-bit (x86)
- **Privilege**: Requires Administrator privileges

---

## ❓ Frequently Asked Questions (FAQ)

<details>
<summary><b>Q1: Why does Reboot Master require Administrator privileges?</b></summary>
A: Modifying boot sequence settings, scheduling UEFI BIOS reboots, and invoking system power management are kernel-level operations that Windows restricts to Administrator accounts.
</details>

<details>
<summary><b>Q2: Why does "Reboot to BIOS" display an unsupported notice on my machine?</b></summary>
A: This feature requires motherboard and OS support for UEFI specifications. If your machine boots under traditional Legacy BIOS (MBR) mode, hardware APIs cannot trigger a software reboot into BIOS. In this case, please use the motherboard's key (Del / F2) during startup.
</details>

<details>
<summary><b>Q3: Am I guaranteed to return to normal mode after entering Safe Mode?</b></summary>
A: Yes! Reboot Master uses a single-boot design that leaves your original default bootloader untouched. Once troubleshooting is done, simply restarting your PC will return you straight to normal Windows.
</details>

<details>
<summary><b>Q4: Why might antivirus software trigger an alert or false positive?</b></summary>
A: Reboot Master is 100% clean, portable software with zero malware or adware. Because it configures system boot entries and invokes low-level power commands, heuristic anti-malware scanners may occasionally flag it. Please add <code>reboot_master.exe</code> to your antivirus whitelist.
</details>

---

## 💬 Issues & Feedback

If you encounter any issues, bugs, or have feature requests during system maintenance:
1. Please report them on our [GitHub Issues](https://github.com/robert820/reboot_master/issues) page.
2. Including your Windows version (e.g. Win10 22H2, WinPE) and log messages from the app will help us fix problems quickly.

---

## 📄 License

This software is released under the [Proprietary Freeware License](../../LICENSE). For the complete terms, usage guidelines, and disclaimers, please refer to the [LICENSE](../../LICENSE) file.
