# 🌐 Reboot Master 多語系語言包 (Language Packs)

[English](#english) | [繁體中文](#繁體中文)

---

## 繁體中文

本目錄收錄 **重啟大師 (Reboot Master)** 的外部擴充語言包與翻譯範本。
為了確保主程式極致輕量與安全，繁體中文、簡體中文、英文、日本語與韓語 5 大常用語言已直接內嵌於主程式核心，其餘 26 種語言則模組化放置於此，供社群自由下載、修改與自訂！

### 🔤 100% 純系統字體架構 (零外部字型依賴)

Reboot Master 採用**純 Windows 系統原生字體架構**：
- **完全零自帶字型**：倉庫與發行版**不攜帶、不下架、不打包任何字型檔** (`*.ttf`, `*.ttc`, `*.otf`)，外部語言包僅包含純文字 Gettext 翻譯檔案 (`reboot_master.po`)。
- **自動適配 Windows 原生 UI 字體**：軟體會根據使用者選擇的介面語言，自動偵測並選用 Windows 7、8、10、11 該語系慣用的系統字體（如微軟正黑體、Segoe UI、Yu Gothic UI / Meiryo、Malgun Gothic 等）。
- **缺字安全防護**：若在極簡環境（如極簡英文 WinPE）下選擇缺少字體的語言，系統會友善提示並安全保留當前語言，防止文字顯示為空白或亂碼方框。

### 📂 目錄結構

```text
lang/
├── template.pot          # 官方翻譯範本檔 (供翻譯新語言或比對最新詞條)
├── de/                   # 語言代碼 (以德文為例)
│   └── reboot_master.po  # 德文 Gettext 翻譯檔案 (純文字 PO，可自由編輯)
├── fr/
│   └── reboot_master.po  # 法文 Gettext 翻譯檔案
├── ru/
│   └── reboot_master.po  # 俄文 Gettext 翻譯檔案
└── ... (共 26+ 種語言擴充包)
```

### 🚀 如何使用外部語言包？

1. 下載您所需語言的資料夾（例如 `lang/de/`）或整個 `lang/` 資料夾。
2. 將 `lang/` 資料夾放置於 `reboot_master.exe` 的**同級目錄**下：
   ```text
   工作目錄：
   ├── reboot_master.exe
   └── lang/
       └── de/
           └── reboot_master.po
   ```
3. 啟動 `reboot_master.exe`，進入「語言設定」選擇該語言，軟體將**自動動態載入**自訂翻譯！
4. **自適應視窗排版**：軟體引擎會自動計算該語言關鍵標題的視覺寬度，自動切換至標準視窗 (920px) 或寬視窗 (1048px)，絕不截斷或折行。

### ✍️ 如何自行修改或貢獻翻譯？

1. **修改現有語言**：
   - 使用免費的 [Poedit](https://poedit.net/) 或任何純文字編輯器（如 VS Code、Notepad++）打開對應語言的 `reboot_master.po`。
   - 搜尋想修改的詞條（`msgid`），修改其對應的譯文（`msgstr`）後存檔即可！
2. **新增全新語言**：
   - 複製 `template.pot` 為 `新語言代碼/reboot_master.po`。
   - 完成翻譯後提交 Pull Request，我們審核後會整合進官方清單！

---

## English

This directory contains external language packs and the translation template for **Reboot Master**.
To keep the universal executable ultra-compact (~5 MB) and zero-dependency, 5 major languages (Traditional Chinese, Simplified Chinese, English, Japanese, and Korean) are built directly into the core binary. The remaining 26 languages are modularized here for community download, customization, and contribution!

### 🔤 100% Native System Font Architecture (Zero Font Bundling)

Reboot Master utilizes a **pure native Windows system font architecture**:
- **Zero Bundled Fonts**: The repository and distributed binaries **never bundle, embed, or download external font files** (`*.ttf`, `*.ttc`, `*.otf`). Language packs contain only plain-text Gettext PO files (`reboot_master.po`).
- **Dynamic System Font Adaptation**: The application dynamically detects and selects the idiomatic native UI fonts installed on Windows 7, 8, 10, and 11 for each language (such as Segoe UI, Microsoft JhengHei, Yu Gothic UI / Meiryo, Malgun Gothic, Tahoma, etc.).
- **Missing Glyph Protection**: In minimal environments (e.g. minimal English WinPE lacking CJK fonts), switching to an unsupported language is safely prevented with an informative message, avoiding broken squares (tofu) and preserving your language preferences.

### 📂 Directory Structure

```text
lang/
├── template.pot          # Official translation template
├── de/                   # Language code (e.g. German)
│   └── reboot_master.po  # Gettext PO translation file (plain text, easily editable)
├── fr/
│   └── reboot_master.po  # French translation file
├── ru/
│   └── reboot_master.po  # Russian translation file
└── ... (26+ languages)
```

### 🚀 How to Use an External Language Pack?

1. Download the specific language directory (e.g. `lang/de/`) or the entire `lang/` folder.
2. Place the `lang/` folder in the same directory as `reboot_master.exe`:
   ```text
   Working Directory:
   ├── reboot_master.exe
   └── lang/
       └── de/
           └── reboot_master.po
   ```
3. Run `reboot_master.exe` and select your language in the Language dropdown. The app will dynamically load your PO catalog with zero restarts required!
4. **Adaptive Window Layout**: The UI dynamically measures the visual width of key titles to expand to wide mode (1048px) or stay in standard compact mode (920px) automatically.

### ✍️ How to Customize or Contribute?

1. Open `reboot_master.po` with [Poedit](https://poedit.net/) or any text editor.
2. Edit `msgstr` translations, save, and reopen the app.
3. Submit a Pull Request to contribute improved translations back to the community!
