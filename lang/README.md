# 🌐 Reboot Master 多語系語言包與字體庫 (Language Packs & Fonts)

[English](#english) | [繁體中文](#繁體中文)

---

## 繁體中文

本目錄收錄 **重啟大師 (Reboot Master)** 的外部擴充語言包與伴隨字庫。
為了確保主程式極致輕量（單一執行檔僅約 4.3 MB），繁體中文、簡體中文與英文已直接內嵌於主程式核心，其餘 28 種語言則模組化放置於此，供社群自由下載、修改與自訂！

### 📂 目錄結構

```text
lang/
├── template.pot          # 官方翻譯範本檔 (供翻譯新語言或比對最新詞條)
├── de/                   # 語言代碼 (以德文為例)
│   ├── reboot_master.po  # 德文 Gettext 翻譯檔案 (可自由編輯)
│   └── font.ttf          # 德文伴隨精簡字庫 (確保任何 WinPE 環境下均能正常顯示)
├── ja/
│   ├── reboot_master.po
│   └── font.ttf
└── ... (共 28 種語言)
```

### 🚀 如何使用外部語言包？

1. 下載您所需語言的資料夾（例如 `lang/de/`）或整個 `lang/` 資料夾。
2. 將 `lang/` 資料夾放置於 `reboot_master.exe` 的**同級目錄**下：
   ```text
   工作目錄：
   ├── reboot_master.exe
   └── lang/
       └── de/
           ├── reboot_master.po
           └── font.ttf
   ```
3. 啟動 `reboot_master.exe`，進入「設定」選擇該語言，軟體將**自動動態載入**自訂翻譯與伴隨字庫！
4. **自適應視窗排版**：軟體引擎會自動計算該語言關鍵標題的視覺寬度，自動切換至標準視窗 (920px) 或寬視窗 (1048px)，絕不截斷或折行。

### ✍️ 如何自行修改或貢獻翻譯？

1. **修改現有語言**：
   - 使用免費的 [Poedit](https://poedit.net/) 或任何純文字編輯器（如 VS Code、Notepad++）打開對應語言的 `reboot_master.po`。
   - 搜尋想修改的詞條（`msgid`），修改其對應的譯文（`msgstr`）後存檔即可！
2. **新增全新語言**：
   - 複製 `template.pot` 為 `新語言代碼/reboot_master.po`。
   - 完成翻譯後提交 Pull Request，我們將為您自動生成伴隨字庫並整合進官方清單！

---

## English

This directory contains external language packs and companion font subsets for **Reboot Master**.
To keep the universal executable ultra-compact (~4.3 MB), Traditional Chinese, Simplified Chinese, and English are built into the core binary. The remaining 28 languages are modularized here for community download, customization, and contribution!

### 📂 Directory Structure

```text
lang/
├── template.pot          # Official translation template
├── de/                   # Language code (e.g. German)
│   ├── reboot_master.po  # Gettext PO translation file
│   └── font.ttf          # Companion minimal font subset
└── ... (28 languages)
```

### 🚀 How to Use an External Language Pack?

1. Download the specific language directory (e.g. `lang/de/`) or the entire `lang/` folder.
2. Place the `lang/` folder in the same directory as `reboot_master.exe`:
   ```text
   Working Directory:
   ├── reboot_master.exe
   └── lang/
       └── de/
           ├── reboot_master.po
           └── font.ttf
   ```
3. Run `reboot_master.exe` and select your language in Settings. The app will dynamically load your PO catalog and register the companion font into memory.
4. **Adaptive Window Layout**: The UI dynamically measures the visual width of key titles to expand to wide mode (1048px) or stay in standard compact mode (920px) automatically.

### ✍️ How to Customize or Contribute?

1. Open `reboot_master.po` with [Poedit](https://poedit.net/) or any text editor.
2. Edit `msgstr` translations, save, and reopen the app.
3. Submit a Pull Request to contribute improved translations back to the community!
