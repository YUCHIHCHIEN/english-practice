# 英語練習室 English Desk

單字、文法、聽力、口說四類英語練習網站。整個網站只有一個 `index.html`，不需要伺服器或資料庫。

## 功能
- **單字**：拍照或上傳圖片，辨識英文單字，做成可翻面的單字卡（音標、中英詞性、中文意思、例句、發音）。也可手動輸入。
- **文法**：21 題附中文解析的選擇題，可依主題練習。
- **聽力**：聽寫（逐字比對）與理解（選擇題），可慢速、可切換美式／英式。
- **口說**：跟讀並用語音辨識打分數，標出唸錯的字。

## 使用的免費服務
| 功能 | 服務 | 備註 |
|---|---|---|
| 圖片文字辨識 | [Tesseract.js](https://github.com/naptha/tesseract.js) | 在使用者裝置上執行，第一次需下載約 10 MB 辨識資料 |
| 音標、詞性、例句 | [Free Dictionary API](https://dictionaryapi.dev/) | 免金鑰；部分單字沒有例句 |
| 中文翻譯 | [MyMemory](https://mymemory.translated.net/) | 免金鑰，匿名每日約 5000 字元 |
| 發音 | 瀏覽器內建 Web Speech API | 聲音依裝置而異 |
| 語音辨識 | 瀏覽器內建 SpeechRecognition | Chrome（電腦、Android）支援最好；iPhone Safari 支援有限 |

## 上架到 GitHub Pages（免費）
1. 登入 [github.com](https://github.com)，右上角 **+ → New repository**。
2. Repository name 輸入 `english-practice`，選 **Public**，按 **Create repository**。
3. 在新 repo 頁面按 **uploading an existing file**，把 `index.html`（和這份 README.md）拖進去，按 **Commit changes**。
4. 進入 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 `main`、資料夾 `/ (root)`，按 **Save**。
5. 等 1–2 分鐘，網址會是：`https://你的帳號.github.io/english-practice/`

之後要更新，只要再上傳新的 `index.html` 覆蓋即可。

## 加到手機主畫面
- **iPhone**：用 Safari 開網址 → 分享 → 加入主畫面。
- **Android**：用 Chrome 開網址 → 右上角選單 → 加到主畫面。

## 其他可用平台
- **Netlify Drop**（app.netlify.com/drop）：把資料夾拖進去就有網址。
- **Cloudflare Pages**、**Vercel**：連結 GitHub repo 後自動部署。
