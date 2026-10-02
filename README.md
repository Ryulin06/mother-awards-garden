# 模範母親祝福花園｜GitHub Pages 版

此資料夾已經接好 Supabase 專案，可直接上傳 GitHub Repository。

## 檔案
- `index.html`：網站主程式
- `config.js`：Supabase 公開連線資訊
- `.nojekyll`：避免 GitHub Pages 套用 Jekyll

## GitHub Pages 上線方式
1. GitHub 建立新的 Repository
2. 把本資料夾內 3 個檔案上傳到 Repository 根目錄
3. 進入 Repository → Settings → Pages
4. Build and deployment：
   - Source：Deploy from a branch
   - Branch：main
   - Folder：/(root)
5. 按 Save
6. GitHub 會產生 `https://你的帳號.github.io/Repository名稱/`

## 測試
開兩個裝置或瀏覽器：
- 手機：使用「手機互動模式」送祝福
- 電腦 / 大螢幕：切到「大螢幕模式」

送出祝福後，大螢幕應透過 Supabase Realtime 即時更新。

## 正式活動前
目前 Supabase 內仍是 60 筆示範名單。
之後可直接把 `awards` 表換成正式獲獎者資料，不需要重做網站。

## 安全
`config.js` 內放的是 Supabase Publishable key，本來就是提供公開前端使用。
不要把 Supabase `service_role` 或 secret key 放進 GitHub Pages。

## 建議正式上線前再做
- 留言審核
- 敏感詞過濾
- 防止短時間重複留言
- 正式活動主視覺
- QR Code
- 大螢幕專用網址參數（例如 `?mode=screen`）
