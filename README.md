# 我的個人品牌｜三頁式網站作業

這是一份可部署到 GitHub Pages 的靜態網站，包含：
- `index.html`：首頁
- `about.html`：公司介紹
- `contact.html`：聯絡我們（姓名、電話、Email、聯絡內容）
- `style.css`：科技黑色風格與手機版排版

## 重要：寄信如何運作
GitHub Pages 只負責託管靜態網頁，不會直接替 HTML 寄信。本作業的聯絡表單使用 FormSubmit（第三方表單轉寄服務），表單提交到 `https://formsubmit.co/zxcv50408@gmail.com`。

首次使用時，FormSubmit 通常會先寄一封啟用確認信到收件地址。請登入 `zxcv50408@gmail.com`，找到 FormSubmit 的確認信並按下啟用連結。若沒看到，檢查垃圾郵件/促銷內容。尚未完成啟用前，表單可能不會正常轉寄。

## A. 在電腦上先預覽
1. 將 ZIP 解壓縮。
2. 打開資料夾，雙擊 `index.html`，用瀏覽器預覽。
3. 點上方「公司介紹」「聯絡我們」確認頁面互相連得起來。
4. 本機預覽只能檢查版面；要驗證寄信，建議部署到 GitHub Pages 後測試。

## B. 上傳到 GitHub Pages
1. 登入 https://github.com/ 或建立帳號。
2. 右上角 `+` → `New repository`。
3. Repository name 建議輸入 `my-personal-brand`。
4. 選擇 `Public`，勾選 `Add a README file` 可選，按 `Create repository`。
5. 在新 repository 頁面按 `Add file` → `Upload files`。
6. 把解壓縮後的 **五個檔案**（`index.html`、`about.html`、`contact.html`、`style.css`、`README.md`）拖進上傳區。若 GitHub 已自動建立 README，可略過本包的 README 或覆蓋前先確認。
7. 在下方按 `Commit changes`。
8. 進入 repository 的 `Settings` → 左側 `Pages`。
9. 在 `Build and deployment` 中，Source 選 `Deploy from a branch`；Branch 選 `main`，資料夾選 `/(root)`，按 `Save`。
10. 等待部署完成。網址通常會是 `https://你的GitHub帳號.github.io/my-personal-brand/`。以 Settings → Pages 實際顯示的網址為準。

## C. 啟用 FormSubmit 收件信箱
1. 網站部署後，開啟 `contact.html` 的公開網址。
2. 用自己的資料填寫四個欄位，先送出一封測試表單。
3. 登入 `zxcv50408@gmail.com`，查看收件匣、垃圾郵件及促銷內容。
4. 若收到 FormSubmit 的啟用確認信，按信中的確認/啟用連結。
5. 回到網站再次送出一筆測試資料。
6. 確認信箱收到標題類似「【我的個人品牌】收到新的聯絡表單」的郵件，並檢查姓名、電話、Email、聯絡內容是否正確。
7. 只有實際收到測試郵件，才可向老師展示已完成。

## D. 常見問題
- **沒收到啟用信**：檢查垃圾郵件，確認 HTML 的 `action` Email 拼字正確，稍等後再測。
- **送出後出現錯誤或驗證頁**：依頁面指示操作；FormSubmit 可能要求驗證。不要用真實客戶的敏感資料測試。
- **GitHub Pages 404**：確認檔名是小寫 `index.html`，檔案放在 repository 根目錄，且 Pages 設為 `main` / `/(root)`。
- **修改後網站沒更新**：確認已按 `Commit changes`，再稍等並重新整理。
- **不想讓信箱公開**：目前頁面上會顯示收件 Email；若不想公開，可從 `contact.html` 的聯絡資訊區移除該文字，但表單的 `action` 仍要保留收件地址。
- **隱私與垃圾信**：這是第三方服務，寄送會經過 FormSubmit。避免收集密碼、身分證字號或其他敏感資料。正式商用前請先閱讀服務條款與隱私政策。

## E. 如何修改
- 改網站名稱：在三個 HTML 中搜尋 `我的個人品牌`，換成你的名稱。
- 改收件 Email：在 `contact.html` 找到 `form action="https://formsubmit.co/zxcv50408@gmail.com"`，換成新的地址。
- 改公司介紹：編輯 `about.html` 中「關於我的個人品牌」等段落，換成真實資訊。
- 改外觀：調整 `style.css` 中的顏色變數（最上方 `:root`）。
