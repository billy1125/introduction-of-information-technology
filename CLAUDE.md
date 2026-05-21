# CLAUDE.md

此檔案提供 Claude Code（claude.ai/code）在此專案中操作時所需的指引。

## 專案概述

本專案為元智大學「資訊與人工智慧概論」課程的教材儲存庫，修課對象為工業工程與管理系學生。所有內容以**繁體中文（台灣用語）**撰寫。

本專案無建置系統、測試套件或 CI/CD 流程，僅包含 Markdown 文件與 Jupyter 筆記本。

## 內容架構

| 檔案 | 說明 |
|------|------|
| `00-Course-Introduction.md` | 課程介紹、評分方式、出席規定、考試規則 |
| `01-History-of-Computer.md` | 計算機歷史、二進位系統、數位化、網路起源、AI 概覽 |
| `02-Computer-Structure.md` | 計算機結構（工業工程導向）、作業系統、應用軟體、工業4.0 |
| `03-Computer-Program.md` | 程式設計概念、資料結構、演算法（工業工程導向） |
| `04-Networks-and-Internet.md` | 網路基礎、網際網路協定、物聯網、智慧製造 |
| `05-Information-Systems-and-Database.md` | 資訊系統、資料庫 |
| `06-Data-Science-and-AI.md` | 資料科學與人工智慧，串接所有課程主線的整合章節 |
| `Computer-Program-Examples.ipynb` | Python Jupyter 筆記本，對應 `03-Computer-Program.md` 的實作範例 |

### 檔案夾
| `temp-reference/` | 用於生成教材的參考資料 |
| `images/` | Markdown 文件引用的圖片 |

## 內容撰寫規範

- **語言**：所有內容必須以繁體中文、台灣習慣的工程與資訊用語撰寫。技術名詞首次出現時附上英文，格式為「中央處理器（CPU）」。
- **工業情境**：每個技術概念都應搭配製造業或工業工程的實際應用範例，延續現有教材的寫作風格。
- **讀者程度**：大一新生、無程式設計背景，說明技術概念時避免未加解釋的專業術語。
- **Markdown 格式**：教材預計透過 GitPrint.com 等工具轉換為 PDF，請使用標準 CommonMark 語法，避免 HTML 或不通用的延伸語法。
- **圖片**：圖片統一放於 `images/` 資料夾，以相對路徑引用，例如 `![說明文字](images/檔名.png)`。
- **參考資料**：如果要生成新內容，優先找`temp-reference/`中的內容，再透過網路找尋適合的資料。

## Jupyter 筆記本（`Computer-Program-Examples.ipynb`）

- 每組 Cell 對應 `03-Computer-Program.md` 的章節內容。
- 變數名稱使用中文（如 `總產量`、`良率`），與教材撰寫風格一致。
- 僅使用 Python 標準函式庫，不引入外部套件。
- 每個程式碼 Cell 必須有可見的輸出，方便學生對照執行結果。
- 筆記本設計為由上往下依序執行，後面的 Cell 會依賴前面 Cell 的定義。
