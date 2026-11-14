# Third-Party Notices / 第三方元件授權聲明

This software is distributed as a closed-source freeware executable and includes the third-party components below. They are licensed under their own terms, which are reproduced here or in [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md). The proprietary freeware [LICENSE](LICENSE) of this project does not apply to them.

本軟體為閉源免費執行檔，內含下列第三方元件。各元件依其原授權條款提供，授權全文見本檔或 [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md)。本專案之 [LICENSE](LICENSE) 專有免費軟體授權不適用於這些元件。

---

## 1. Slint (GUI toolkit)

- Project / 專案：https://slint.dev
- License elected / 採用授權：**Slint Royalty-free Desktop, Mobile, and Web Applications License 2.0**
  (Slint is offered under GPL-3.0 / Royalty-free / Commercial; this software uses the Royalty-free option. / Slint 提供 GPLv3、免費授權、商業授權三選一，本軟體採用免費授權。)
- Use / 使用方式：This is a desktop application for general-purpose Windows PCs. It is not an embedded system and does not expose Slint APIs. The Slint toolkit is only distributed as part of this application. / 本軟體為一般 Windows 電腦上的桌面應用程式，非嵌入式系統，亦不對外暴露 Slint API，Slint 僅隨本應用程式一併散布。
- Modifications / 修改：A locally patched copy of some `i-slint-*` crates is used; original license notices are kept unchanged. / 部分 `i-slint-*` 套件使用本地修補版，原始授權聲明均未更動。
- Attribution (required by Section 2 of the license) / 授權要求之標示：

<a href="https://slint.dev"><picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/slint-ui/slint/master/logo/MadeWithSlint-logo-dark.png">
  <img src="https://raw.githubusercontent.com/slint-ui/slint/master/logo/MadeWithSlint-logo-light.png" alt="Made with Slint" width="180">
</picture></a>

Full license text: see [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md#slint-royalty-free-license-20).

---

## 2. YY-Thunks

- Project / 專案：https://github.com/Chuyu-Team/YY-Thunks
- Usage / 用途：Statically linked compatibility layer that lets the executable run on older Windows versions (e.g. Windows 7) / 以靜態連結方式提供舊版 Windows（如 Windows 7）API 相容層
- License / 授權：MIT License

```
MIT License

Copyright (c) 2018 Chuyu-Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 3. Rust standard library and Rust crates / Rust 標準函式庫與套件

The executable is written in Rust and statically links the Rust standard library (MIT OR Apache-2.0) and the open-source crates listed in [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) (MIT, Apache-2.0, BSD, ISC, Zlib, Unicode-3.0, BSL-1.0 and similar permissive licenses), together with their license texts and copyright notices.

本執行檔以 Rust 撰寫，靜態連結 Rust 標準函式庫（MIT OR Apache-2.0）與 [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) 所列開源套件（MIT、Apache-2.0、BSD、ISC、Zlib、Unicode-3.0、BSL-1.0 等寬鬆授權），其授權全文與版權聲明均已收錄於該檔。
