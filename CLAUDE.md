# CLAUDE.md

此檔案提供 Claude Code（claude.ai/code）在此專案中操作時所需的指引。

## 專案概述

本專案為元智大學「資訊與人工智慧概論」課程的教材儲存庫，修課對象為工業工程與管理系學生。所有內容以 **繁體中文（台灣用語）** 撰寫。

本專案無建置系統、測試套件或 CI/CD 流程，僅包含 Markdown 文件與 Jupyter 筆記本。

## 內容架構

| 檔案 | 說明 |
|------|------|
| `00-Course-Introduction.md` | 課程介紹、評分方式、出席規定、考試規則 |
| `01-History-of-Computer.md` | 計算機歷史、二進位系統、數位化、網路起源、AI 概覽 |
| `02-Computer-Structure.md` | 計算機結構（工業工程導向）、作業系統、應用軟體 |
| `03-Computer-Program.md` | 程式設計概念、資料結構、演算法（工業工程導向） |
| `04-Networks-and-Internet.md` | 分三篇：網路（硬體、拓樸、無線與行動通訊、物聯網）、網際網路（TCP/IP、WWW、DNS、網路服務與資安）、整合觀點（智慧製造網路架構） |
| `05-Information-Systems-and-Database.md` | 資訊系統、資料庫（ERP/MES/SCM 等企業應用系統的權威章節） |
| `06-Data-Science-AI-and-Smart-Manufacturing.md` | 資料科學、人工智慧與智慧製造（**全課程終點**）：串接計算機→程式→網路→資訊系統→AI 的技術演進主線，並在最後以工業4.0智慧工廠案例收束全課程。機器學習／深度學習原理、AI 發展史，以及工業4.0（定義、九大支柱、數位轉型、數位孿生）的權威章節 |
| `notebooks/Computer-Program-Examples.ipynb` | Python Jupyter 筆記本，對應 `03-Computer-Program.md` 的實作範例 |
| `notebooks/Computer-Structure-Examples.ipynb` | Python Jupyter 筆記本，對應 `02-Computer-Structure.md`〈四、數字系統與進位轉換〉與〈五、浮點數與 IEEE 754〉的練習題完整詳解 |

各章節另有對應的 Marp 投影片版本 `0X-XXX.slides.md`（目前涵蓋 00–06 章）。

### 檔案夾

| 資料夾 | 說明 |
|------|------|
| `reference/` | 教材撰寫規範與骨架範本，**格式規則的唯一權威來源**。內容刻意與課程脫鉤，換一門課可整個資料夾複製沿用 |
| `temp-reference/` | 生成教材用的暫存參考素材（非規範文件） |
| `images/` | Markdown 文件引用的圖片，依所屬文章分子資料夾 |
| `notebooks/` | 所有課程練習用的 Jupyter 筆記本，集中放置於此資料夾 |
| `.claude/skills/` | Claude Code 技能（skill），每個技能自成一個資料夾，資料夾內含 `SKILL.md` 與其相依檔案 |

## 教材撰寫規範

格式規則一律以 `reference/` 的規範文件為準，本檔不重述。動筆前先讀對應的規範，再複製骨架檔開始寫：

| 要做的事 | 先讀規範 | 再複製骨架 |
|------|------|------|
| 新增或修改章節正文 `0X-XXX.md` | `reference/chapter-writing-guide.md` | `reference/chapter-template.md` |
| 新增或修改投影片 `0X-XXX.slides.md` | `reference/slides-design-template.md` | `reference/slides-template.slides.md` |
| 新增或修改練習筆記本 `notebooks/*.ipynb` | `reference/notebook-guide.md` | — |

分工是：**怎麼寫** 在 `reference/`，**寫什麼** 在下一節。兩邊若有衝突，格式規則以規範文件為準。

即使只做小幅修改、來不及讀完規範，以下三條一律適用：

- 繁體中文、台灣習慣用語，技術名詞首次出現時附上英文全名
- 粗體 `**` 貼著中文字或英數字時，標記外側補一個半形空白
- 授權無法確認的外部圖片不可收錄

## 本課程專屬設定

規範文件中凡標示「由 `CLAUDE.md` 指定」的占位項目，實際值如下。

- **章節標題副標**：各章正文以 `# {章節標題}——工業工程管理導向` 開頭。
- **讀者程度**：大一新生、工業工程與管理系、無程式設計背景。
- **應用範例取材**：一律取自製造業與工業工程場域。
- **學習重點總結的固定引言**：「讀完本章後，你應該能夠理解以下核心概念，並將其應用於工業場域的思考與決策：」。範本見 `04-Networks-and-Internet.md`〈二十五、學習重點總結〉。
- **銜接提示對象**：01–05 章一律前指 `06-Data-Science-AI-and-Smart-Manufacturing.md`；06 章為全課程終點，不需銜接提示。跨章連結的實際寫法範本見 `02-Computer-Structure.md`〈二十三、專業工業應用軟體〉。
- **參考文獻取材**：經典教科書取 Tanenbaum、Silberschatz、Cormen 等公認課本，原典取 Turing 1936、Codd 1970、Cerf & Kahn 1974、Vaswani 2017 等里程碑論文；份量與 `06-Data-Science-AI-and-Smart-Manufacturing.md` 看齊。
- **趣味小知識**：各章適時穿插 `> **趣味小知識**：…` 的 blockquote，補充名詞由來、歷史八卦或老師的親身經驗，讓大一新生對枯燥的技術名詞產生記憶點。這是本教材的既有特色，新增章節時應延續。
- **延伸閱讀連結**：正文大量附上中文維基百科連結，此慣例對學生的說明見 `README.md`〈🔗 延伸閱讀連結說明〉。
- **生成新內容的素材來源**：先找 `temp-reference/`，再上網搜尋。
- **專案架構**：資料夾架構不寫進 `README.md`。

### 權威章節清單

各主題的完整介紹只寫在下列章節，其他章節提到時一兩句話帶過並連結過去：

| 主題 | 權威章節 |
|------|------|
| ERP／MES／SCM 等企業應用系統的定義與功能 | `05-Information-Systems-and-Database.md`〈三、企業應用系統〉 |
| 資料庫、SQL、NoSQL、大數據特性（5V） | `05-Information-Systems-and-Database.md` |
| 機器學習／深度學習原理、AI 發展史 | `06-Data-Science-AI-and-Smart-Manufacturing.md` |
| 工業4.0（定義、九大支柱、數位轉型、數位孿生）與智慧工廠整合案例 | `06-Data-Science-AI-and-Smart-Manufacturing.md`〈五、工業4.0與智慧製造〉 |
| 智慧工廠的分層架構 | `04-Networks-and-Internet.md`〈二十三、智慧製造網路架構（概念性）〉 |

智慧工廠分層架構以該節的 **四層模型**（現場層／控制層／管理層／雲端層）為全專案唯一標準。IoT 文獻常見的「感知層／網路層／應用層」三層說法，僅能出現在該節的對照 blockquote 中，其他地方不得用三層講智慧工廠架構。

新增趣味小知識或範例前，務必先全專案搜尋該主題是否已在他章出現過（例如 SQL／SEQUEL 的由來、大數據 3V 的來歷都已在 05 章）。

## Claude Code 技能（`.claude/skills/`）

- **一個技能一個資料夾**：每個 skill 都自成一個獨立資料夾（如 `.claude/skills/speak-human-tw/`），該技能所有相依檔案（`references/`、`evals/` 等）一律收在此資料夾內，不散落於專案根目錄；`SKILL.md` 內的相對連結也必須指向資料夾內部，確保技能可獨立搬移。
- **技能授權例外**：移植自外部專案的技能，依其原始授權條款使用，不適用本專案 README 所宣告的 CC BY-NC-SA 授權。移植時須在技能資料夾內保留原始 `LICENSE`，`SKILL.md` frontmatter 保留原作者標示，並在 `README.md`〈📄 授權與使用聲明〉的例外項目中列明來源與授權。
- 現有技能：`speak-human-tw`（繁體中文去 AI 味改寫，移植自 [Raymond Hou 的 speak-human-tw](https://github.com/Raymondhou0917/speak-human-tw)，MIT 授權）。
