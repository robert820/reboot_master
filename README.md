<div align="center">

<a href="https://blog.dei3c.com/2026/09/reboot-master.html" target="_blank" rel="noopener noreferrer">
  <img src="https://github.com/user-attachments/assets/2830eb70-512c-4ddb-87ec-5213a6e465b1" alt="得翼科技 | 重啟大師 (Reboot Master)" height="70" />
</a>

<br /><br />

**繁體中文** · [简体中文](docs/readme/README_zh-CN.md) · [English](docs/readme/README_en.md)

# 重啟大師 (Reboot Master)

### 輕量、安全且功能強大的 Windows 電源與啟動管理工具
專為日常使用、電腦維修與 WinPE 維護環境打造

[![Platform](https://img.shields.io/badge/Platform-Windows%207%20%7C%208%20%7C%2010%20%7C%2011%20%7C%20WinPE-blue?style=flat-square&logo=windows)](https://github.com/robert820/reboot_master)
[![Type](https://img.shields.io/badge/Type-Freeware%20%7C%20Portable-success?style=flat-square)](#-下載與使用說明)
[![UI](https://img.shields.io/badge/GUI-Modern%20Responsive%20UI-blueviolet?style=flat-square)](#)
[![Download](https://img.shields.io/badge/Download-GitHub%20Releases-blue?style=flat-square&logo=github)](https://github.com/robert820/reboot_master/releases)

**告別狂按鍵盤、告別安全模式卡死無限輪迴。一鍵搞定 Windows 電源與開機設定。**

[功能介紹](#-功能介紹) · [下載與使用說明](#-下載與使用說明) · [救援指令](#-緊急救援指令-cli) · [系統需求](#-系統相容性與需求) · [常見問題](#-常見問題-faq) · [問題反饋](#-問題反饋與支援)

</div>

---

## 📖 軟體簡介

在日常使用電腦、系統維護或重灌時，您是否遇過這些困擾？
- 想進 BIOS/UEFI 設定開機順序，開機時按鍵狂按 Delete 或 F2 卻總是錯過時機？
- 想進安全模式排查故障，卻因為系統卡死或鍵盤失靈，陷入了**安全模式無限重啟迴圈**的惡夢？
- 想要安裝特殊硬體驅動或測試工具，卻找不到哪裡可以關閉驅動強制簽章與記憶體完整性？
- 在維護隨身碟 (WinPE) 環境下，找不到方便好用的工具快速切換開機碟或重啟？

**重啟大師 (Reboot Master)** 是專為徹底解決這些繁瑣痛點設計的綠色實用工具。免安裝、無廣告、開箱即用，讓複雜的 Windows 啟動設定變得直覺又簡單！

---

## ✨ 功能介紹

### 1. ⚡ 一鍵重啟進入 BIOS / UEFI
- 免狂敲鍵盤、免猜不同主機板快捷鍵，點擊按鈕即可讓電腦於重開機時自動載入 BIOS/UEFI 設定畫面。
- 內建智慧相容性偵測，若是傳統 Legacy BIOS (MBR) 模式會貼心提供防呆提醒。

### 2. 🛡️ 一次性安全模式（防卡死設計）
- **拒絕安全模式無限迴圈**：傳統方式進安全模式容易因設定被鎖定而無法回到正常桌面。
- **單次引導保護機制**：僅在「下一次重啟」進入安全模式，**排查完畢後只要再次手動重開機，系統立即自動恢復進入正常模式**，乾淨無痕！
- 支援「最小化安全模式」與「含網路連線的安全模式」。

### 3. 🛠️ 一鍵進入進階開機選項 (WinRE)
- 快速重啟至 Windows 進階疑難排解選單，方便進行系統還原、啟動修復或命令提示字元操作。

### 4. 🚀 隨身碟快速開機 (USB Boot)
- 自動搜尋並枚舉本機連接的 USB 開機隨身碟與外接磁碟。
- 允許使用者快速指定由特定的 USB 隨身碟重啟，省去手動進 BIOS 調整開機順序的麻煩。

### 5. 🔐 驅動強制簽章與核心安全防護
- **測試模式 (Test Mode)**：一鍵開啟或關閉 Windows 測試模式。
- **停用驅動程式強制簽章**：方便安裝未經微軟數位簽章的硬體驅動程式或測試版軟體。
- **記憶體完整性 (核心隔離)**：直覺切換核心隔離保護，排除特殊效能調校工具與外接裝置的相容性衝突。

### 6. 🔌 原生極速關機與重啟
- 採用系統原生指令，極速響應，杜絕程序假死或重啟卡頓現象。

### 7. 💽 深度支援 WinPE 維護環境
- 完美相容各類裝機維護隨身碟（WinPE），能在隨身碟環境下自動定位實體系統碟，維修裝機超省心。
- 內建顯示相容性最佳化，在任何 PE 急救碟中均能穩定流暢顯示。

### 8. 🌐 完整支援 31 種語言與現代化介面
- **全球 31 種語言完整支援**：軟體啟動時自動偵測 Windows 系統語言，亦可隨時在介面設定中自由切換。核心內建繁中、簡中、英文，其餘 28 種語言收錄於 [lang/ 語言包目錄](lang/README.md)，支援社群自由編輯與自適應寬度排版：
  | 地區分類             | 支援語言列表 (共 31 種)                                                                                                              |
  | :------------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
  | **東亞語系**         | 繁體中文、简体中文、日本語、한국어                                                                                                   |
  | **歐洲語系**         | English、Français、Deutsch、Español、Italiano、Português、Русский、Українська、Polski、Svenska、Magyar、Ελληνικά、Català、Беларуская |
  | **中東與西亞語系**   | العربية (Arabic)、فارسی (Persian)、עברית (Hebrew)、Türkçe、Kurdî                                                                     |
  | **東南亞與其他地區** | ไทย (Thai)、Bahasa Indonesia、Azərbaycanca、Српски (Ћирилица)、Srpski (Latinica)、Тоҷикӣ、Ўзбекча、Oʻzbekcha                         |
- **現代美觀主題**：支援深色模式 (Dark Mode)、淺色模式 (Light Mode) 與跟隨系統外觀自動切換。
- **透明即時日誌**：內建操作紀錄視窗，清楚呈現每一步執行狀態，方便掌握與問題回報。

---

## 📦 下載與使用說明

### 下載方式
1. 前往本專案的 [Releases 頁面](https://github.com/robert820/reboot_master/releases) 下載最新版本的 `reboot_master.exe`。
2. 本程式為**單一免安裝綠色執行檔**，無須安裝額外執行庫，下載後可直接存放於桌面或隨身碟隨身攜帶。

### 使用步驟
1. 對 `reboot_master.exe` 連點左鍵兩下執行。
2. 在主介面中點選您想執行的功能卡片（如：重啟進入 BIOS、一次性安全模式、隨身碟啟動等）。
3. 閱讀確認對話框中的說明後點選「確認」，程式即會自動執行並在即時日誌視窗中呈現執行進度。

---

## 🖥️ 系統相容性與需求

- **作業系統**：Windows 11 / 10 / 8.1 / 8 / 7 (SP1) 及 Windows PE 維護環境
- **架構支援**：64 位元 (x64) 與 32 位元 (x86)
- **執行權限**：需具備系統管理員身分

---

## ❓ 常見問題 (FAQ)

<details>
<summary><b>Q1: 為什麼程式啟動時必須要求「系統管理員權限」？</b></summary>
A: 本工具執行的功能（如指示下次開機進入 BIOS、調整開機啟動設定、關機控制）皆屬於 Windows 系統層級的核心權限，作業系統規定必須以管理員身分才能執行。
</details>

<details>
<summary><b>Q2: 為什麼點擊「重啟進入 BIOS」會提示不支援？</b></summary>
A: 此功能需主機板與作業系統支援 UEFI 規範。如果您的電腦開機方式為傳統的 Legacy BIOS (MBR) 模式，硬體層級本身不支援由軟體發出重啟進 BIOS 的指令，此時請在開機時手動按鍵（如 Del 或 F2）進入。
</details>

<details>
<summary><b>Q3: 一次性安全模式進入後，真的只要再次重開機就會回到正常模式嗎？</b></summary>
A: 是的！本工具採用單次引導設計，原始系統的預設開機項目從頭到尾都沒有被更改。排查完畢後，只要隨時手動重新開機，就會直接回到您原本熟悉的正常 Windows。
</details>

<details>
<summary><b>Q4: 為什麼防毒軟體有時會出現警示或誤報？</b></summary>
A: 本工具為純綠色免安裝軟體，絕無任何惡意聯網後門、廣告插件或竊取隱私行為。但因為程式需調整 Windows 開機引導與執行底層電源控制，此類系統級操作容易被部分啟發式防毒軟體（Heuristics）以較嚴格的標準判定。若遇誤報，請安心將 <code>reboot_master.exe</code> 加入防毒軟體信任名單。
</details>

---

## 💬 問題反饋與支援

如果您在日常使用或系統維護過程中遇到任何問題、Bug，或是對新功能有建議：
1. 請至本專案的 [Issues 頁面](https://github.com/robert820/reboot_master/issues) 提交反饋。
2. 提交時建議附上作業系統版本（如 Win10 22H2、WinPE 等）以及程式內日誌視窗中顯示的具體錯誤訊息，這將有助於我們快速為您排查與修復！

---

## 📄 授權條款 (License)

本軟體採用專有免費軟體授權（Proprietary Freeware），完整授權規範、使用條款與免責聲明請參閱 [LICENSE](LICENSE) 檔案。
