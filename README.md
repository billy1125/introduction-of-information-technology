# 資訊與人工智慧概論 教材 — Introduction to Information Technology & AI

> **元智大學「資訊與人工智慧概論」課程教材**（呂卓勲老師負責部分），修課對象為工業工程與管理系學生。全文以**繁體中文（台灣用語）**撰寫，技術名詞首次出現時附上英文原文，並搭配製造業／工業工程的實際應用範例。

**關鍵字 Keywords**：資訊科技概論、計算機概論、人工智慧、資料科學、工業工程、元智大學、大學課程教材。

> **閱讀建議**：本教材包含大量文字、表格與架構圖，少部分程式碼，建議使用**電腦或平板**開啟，手機螢幕過窄會導致排版跑掉，閱讀體驗不佳。

---

## 📚 教材清單

| 檔案 | 主題 | 說明 |
|------|------|------|
| [00-Course-Introduction.md](00-Course-Introduction.md) | 課程介紹 | 課程概要、評分方式、考試規定、出席規範、請假規定 |
| [01-History-of-Computer.md](01-History-of-Computer.md) | 計算機歷史 | 計算工具演進、二進位系統、數位化、網路起源、AI 發展簡史 |
| [02-Computer-Structure.md](02-Computer-Structure.md) | 電腦架構 | CPU、記憶體、儲存裝置、作業系統、應用軟體、工業4.0 |
| [03-Computer-Program.md](03-Computer-Program.md) | 程式設計概念 | 演算法、程式語言、資料結構、工業工程應用 |
| [04-Networks-and-Internet.md](04-Networks-and-Internet.md) | 網路與網際網路 | 網路基礎、TCP/IP、雲端運算、物聯網、智慧製造 |
| [05-Information-Systems-and-Database.md](05-Information-Systems-and-Database.md) | 資訊系統與資料庫 | 資訊系統類型（TPS/MIS/DSS/EIS）、ERP/MES/CRM、關聯式資料庫、SQL、NoSQL、大數據、電子商務 |
| [06-Data-Science-and-AI.md](06-Data-Science-and-AI.md) | 資料科學與人工智慧 | 從計算機歷史到 AI 的完整脈絡、機器學習、深度學習、生成式 AI、AI 代理人 |

## 💻 程式範例與練習筆記本

所有練習用 Jupyter 筆記本統一放在 [`notebooks/`](notebooks/) 資料夾：

| 檔案 | 說明 |
|------|------|
| [notebooks/Computer-Program-Examples.ipynb](notebooks/Computer-Program-Examples.ipynb) | Python Jupyter 筆記本，對應 `03-Computer-Program.md` 的實作範例，可在 Google Colab 或 JupyterLab 執行 |
| [notebooks/Computer-Structure-Examples.ipynb](notebooks/Computer-Structure-Examples.ipynb) | Python Jupyter 筆記本，對應 `02-Computer-Structure.md` 進位轉換與 IEEE 754 練習題的完整計算過程與程式驗證 |

---

## 📖 如何使用這份教材

1. **直接在 GitHub 上閱讀**：點選上方各檔案連結即可線上閱覽 Markdown 內容
2. **轉為投影片或 PDF**：部分章節提供對應的 Marp 投影片版本（檔名為 `0X-XXX.slides.md`），可使用 [Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode) 或 [Marp CLI](https://github.com/marp-team/marp-cli) 開啟並匯出為簡報或 PDF，方便上課簡報或列印
3. **搭配 AI 工具延伸學習**：每份教材都可以直接貼給生成式 AI（如 ChatGPT、Claude）請它幫你整理重點、出練習題或解釋不懂的段落

---

## 🧭 閱讀順序建議

```
00 課程介紹
    ↓
01 計算機歷史（理解電腦從哪裡來）
    ↓
02 電腦架構（理解電腦如何運作）
    ↓
03 程式設計概念（理解電腦如何被控制）
    ↓
04 網路與網際網路（理解電腦如何連結）
    ↓
05 資訊系統與資料庫（理解企業如何運用電腦）
    ↓
06 資料科學與人工智慧（理解 AI 如何從資料中學習）
```

---

## 🤖 AI 協作聲明

本教材內容除作者自行撰寫外，部分段落與圖片透過生成式 AI（如 ChatGPT、Claude）協作產生，並由作者審閱與編修。惟 AI 生成內容仍可能存在錯誤或過時資訊，雖作者盡力糾正與編輯，若您仍發現內容有誤，歡迎透過 Issue 回報。

若圖片為 AI 生成，會在圖片下方以圖說標註（例如「圖片來源：作者自製或 ChatGPT 生成」）；引用自外部來源（如維基百科）的圖片，則會標註原始出處與連結，該等圖片仍依其原始授權條款使用，版權歸屬原作者或原出處所有，不適用下方之整體授權聲明。

---

## 📄 授權與使用聲明

本教材（不含下述例外項目）採用 [CC BY-NC-SA 4.0（姓名標示－非商業性－相同方式分享）](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh-hant) 授權釋出。你可以自由**分享**（重製、散布）與**改作**（修改、轉化、部分引用）本教材內容，但須符合以下條件：

- **姓名標示**：需註明原作者（Cho-Hsun Lu）與本專案連結
- **非商業性**：不得用於商業目的
- **相同方式分享**：若對本教材進行改作，需以相同授權條款釋出

**例外項目（不適用上述授權）**：

- 引用自維基百科等外部來源的圖片，依其原始授權條款使用，版權歸屬原作者或原出處，詳見各圖片下方的來源標註
- 內容中提及之特定廠商、品牌或產品名稱（如 Google、Microsoft、IBM、OpenAI、Apple 等），其名稱、商標與相關權利均屬各該公司或商標權人所有，本教材與其並無隸屬或合作關係

**免責聲明**：本教材以現狀（AS IS）提供，作者已盡力確保內容正確，但不保證內容完全正確、完整或適用於特定情境，使用者應自行判斷並承擔使用風險。

© 2026 Cho-Hsun Lu
