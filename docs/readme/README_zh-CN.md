<div align="center">

<a href="https://blog.dei3c.com/2026/09/reboot-master.html" target="_blank" rel="noopener noreferrer">
  <img src="https://github.com/user-attachments/assets/2830eb70-512c-4ddb-87ec-5213a6e465b1" alt="得翼科技 | 重启大师 (Reboot Master)" height="70" />
</a>

<br /><br />

[繁體中文](../../README.md) · **简体中文** · [English](README_en.md)

# 重启大师 (Reboot Master)

### 轻量、安全且功能强大的 Windows 电源与启动管理工具
专为日常使用、电脑维护与 WinPE 维护环境打造

[![Platform](https://img.shields.io/badge/Platform-Windows%207%20%7C%208%20%7C%2010%20%7C%2011%20%7C%20WinPE-blue?style=flat-square&logo=windows)](https://github.com/robert820/reboot_master)
[![Type](https://img.shields.io/badge/Type-Freeware%20%7C%20Portable-success?style=flat-square)](#-下载与使用说明)
[![UI](https://img.shields.io/badge/GUI-Modern%20Responsive%20UI-blueviolet?style=flat-square)](#)
[![Download](https://img.shields.io/badge/Download-GitHub%20Releases-blue?style=flat-square&logo=github)](https://github.com/robert820/reboot_master/releases)

**告别狂按键盘、告别安全模式卡死无限循环。一键搞定 Windows 电源与开机设置。**

[功能介绍](#-功能介绍) · [下载与使用说明](#-下载与使用说明) · [救援指令](#-紧急救援指令-cli) · [系统需求](#-系统兼容性与需求) · [常见问答](#-常见问题-faq) · [问题反馈](#-问题反馈与支持)

</div>

---

## 📖 软件简介

在日常使用电脑、系统维护或重装时，您是否遇过这些困扰？
- 想进 BIOS/UEFI 设置启动顺序，开机时按键狂按 Delete 或 F2 却总是错过时机？
- 想进安全模式排查故障，却因为系统卡死或键盘失灵，陷入了**安全模式无限重启循环**的噩梦？
- 想要安装特殊硬件驱动或测试工具，却找不到哪里可以关闭驱动强制签名与内存完整性？
- 在维护 U 盘 (WinPE) 环境下，找不到方便好用的工具快速切换启动盘或重启？

**重启大师 (Reboot Master)** 是专为彻底解决这些繁琐痛点设计的绿色实用工具。免安装、无广告、开箱即用，让复杂的 Windows 启动设置变得直觉又简单！

---

## ✨ 功能介绍

### 1. ⚡ 一键重启进入 BIOS / UEFI
- 免狂按键盘、免猜不同主板快捷键，点击按钮即可让电脑于重启时自动加载 BIOS/UEFI 设置画面。
- 内置智能兼容性检测，若是传统 Legacy BIOS (MBR) 模式会贴心提供防呆提醒。

### 2. 🛡️ 一次性安全模式（防卡死设计）
- **拒绝安全模式无限循环**：传统方式进安全模式容易因设置被锁定而无法回到正常桌面。
- **单次引导保护机制**：仅在“下一次重启”进入安全模式，**排查完毕后只要再次手动重启，系统立即自动恢复进入正常模式**，干净无痕！
- 支持“最小化安全模式”与“含网络连接的安全模式”。

### 3. 🛠️ 一键进入高级启动选项 (WinRE)
- 快速重启至 Windows 高级疑难解答菜单，方便进行系统还原、启动修复或命令提示符操作。

### 4. 🚀 U 盘快速开机 (USB Boot)
- 自动扫描并枚举本机连接的 USB 启动盘与外接磁盘。
- 允许用户快速指定由特定的 USB 闪存盘重启，省去手动进 BIOS 调整启动顺序的麻烦。

### 5. 🔐 驱动强制签名与核心安全防护
- **测试模式 (Test Mode)**：一键开启或关闭 Windows 测试模式。
- **禁用驱动程序强制签名**：方便安装未获微软数字签名的硬件驱动程序或测试版软件。
- **内存完整性 (核心隔离)**：直觉切换核心隔离保护，排除特殊性能调优工具与外接设备的兼容性冲突。

### 6. 🔌 原生极速关机与重启
- 采用系统原生指令，极速响应，杜绝程序假死或重启卡顿现象。

### 7. 💽 深度支持 WinPE 维护环境
- 完美兼容各类装机维护 U 盘（WinPE），能在 U 盘环境下自动定位物理系统盘，维修装机超省心。
- 内置显示兼容性优化，在任何 PE 急救盘中均能稳定流畅显示。

### 8. 🌐 完整支持 31 种语言与现代化界面
- **全球 31 种语言完整支持**：软件启动时自动检测 Windows 系统语言，亦可随时在界面设置中自由切换。全数原生内置支持，绝无遗漏：
  | 地区分类             | 支持语言列表 (共 31 种)                                                                                                              |
  | :------------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
  | **东亚语系**         | 繁體中文、简体中文、日本語、한국어                                                                                                   |
  | **欧洲语系**         | English、Français、Deutsch、Español、Italiano、Português、Русский、Українська、Polski、Svenska、Magyar、Ελληνικά、Català、Беларуская |
  | **中东与西亚语系**   | العربية (Arabic)、فارسی (Persian)、עברית (Hebrew)、Türkçe、Kurdî                                                                     |
  | **东南亚与其他地区** | ไทย (Thai)、Bahasa Indonesia、Azərbaycanca、Српски (Ћирилица)、Srpski (Latinica)、Тоҷикӣ、Ўзбекча、Oʻzbekcha                         |
- **现代美观主题**：支持深色模式 (Dark Mode)、浅色模式 (Light Mode) 与跟随系统外观自动切换。
- **透明实时日志**：内置操作记录窗口，清楚呈现每一步执行状态，方便掌握与问题反馈。

---

## 📦 下载与使用说明

### 下载方式
1. 前往本项目的 [Releases 页面](https://github.com/robert820/reboot_master/releases) 下载最新版本的 `reboot_master.exe`。
2. 本程序为**单执行文件免安装绿色版**，无需安装额外运行库，下载后可直接存放于桌面或 U 盘随身携带。

### 使用步骤
1. 左键双击 `reboot_master.exe`执行。
2. 在主界面中点击您想执行的功能卡片（如：重启进入 BIOS、一次性安全模式、U 盘启动等）。
3. 阅读确认对话框中的说明后点击「确认」，程序即会自动执行并在实时日志窗口中显示执行进度。

---

## 🖥️ 系统兼容性与需求

- **操作系统**：Windows 11 / 10 / 8.1 / 8 / 7 (SP1) 及 Windows PE 维护环境
- **架构支持**：64 位 (x64) 与 32 位 (x86)
- **运行权限**：需要以管理员身份运行

---

## ❓ 常见问题 (FAQ)

<details>
<summary><b>Q1: 为什么程序启动时必须要求「管理员权限」？</b></summary>
A: 本工具执行的功能（如指示下次开机进入 BIOS、调整开机启动设置、关机控制）均属于 Windows 系统层级的核心权限，操作系统规定必须以管理员身份才能执行。
</details>

<details>
<summary><b>Q2: 为什么点击「重启进入 BIOS」会提示不支持？</b></summary>
A: 此功能需主板与操作系统支持 UEFI 规范。如果您的电脑引导方式为传统的 Legacy BIOS (MBR) 模式，硬件层级本身不支持由软件发出重启进 BIOS 的指令，此时请在开机时手动按键（如 Del 或 F2）进入。
</details>

<details>
<summary><b>Q3: 一次性安全模式进入后，真的只要再次重启就会回到正常模式吗？</b></summary>
A: 是的！本工具采用单次引导设计，原始系统的默认开机项目从始至终均未被更改。排查完毕后，只要随时手动重新启动，就会直接回到您原本熟悉的正常 Windows。
</details>

<details>
<summary><b>Q4: 为什么杀毒软件有时会出现警示或误报？</b></summary>
A: 本工具为纯绿色免安装软件，绝无任何恶意联网后门、广告插件或窃取隐私行为。但因为程序需调整 Windows 开机引导与执行底层电源控制，此类系统级操作容易被部分启发式杀毒软件（Heuristics）以较严格的标准判定。若遇误报，请放心将 <code>reboot_master.exe</code> 加入信任名单。
</details>

---

## 💬 问题反馈与支持

如果您在日常使用或系统维护过程中遇到任何问题、Bug，或是对新功能有建议：
1. 请至本项目的 [Issues 页面](https://github.com/robert820/reboot_master/issues) 提交反馈。
2. 提交时建议附上操作系统版本（如 Win10 22H2、WinPE 等）以及程序内日志窗口中显示的具体错误信息，这将有助于我们快速为您排查与修复！

---

## 📄 软件授权与免责声明

- **免费使用**：本软件为免费实用工具（Freeware），任何人均可免费下载、个人使用或于商业维护环境中使用。
- **免责声明**：本软件已针对各种系统环境进行严密测试与防呆保护（例如引导项自动还原、Legacy BIOS 识别等）。但修改系统底层开机引导仍属系统级高级操作，用户应自行评估并承担使用本软件时可能衍生之系统风险。
