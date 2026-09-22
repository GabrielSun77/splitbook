
# 三人分帳簿 — GitHub Pages 架設說明

https://gabrielsun77.github.io/splitbook/

這個資料夾就是完整的網頁 App（PWA）。放到 GitHub Pages 後，iPhone / Android 都能免登入開啟，
並可「加入主畫面」變成獨立 App，離線也能用，資料存在各自手機裡。

## 一、上傳到 GitHub（約 10 分鐘，全部在瀏覽器操作）

1. 到 https://github.com 註冊免費帳號（已有就直接登入）。
2. 右上角「+」→「New repository」。
   - Repository name 填：`splitbook`
   - 選 **Public**（Pages 免費方案必須是公開 repo）
   - 其他不用勾，按「Create repository」。
3. 在新 repo 頁面點「uploading an existing file」。
   把這個資料夾裡的所有東西（`index.html`、`manifest.webmanifest`、`sw.js`、`icons` 資料夾）
   一起拖進去。※ 拖「資料夾裡的內容」，不是拖整個 splitbook 資料夾。
   下方按「Commit changes」。
4. 進 repo 的「Settings」→ 左側「Pages」。
   - Source 選「Deploy from a branch」
   - Branch 選 `main`，資料夾選 `/ (root)`，按 Save。
5. 等 1～3 分鐘，重新整理 Pages 頁面，上方會出現網址：
   `https://你的帳號.github.io/splitbook/`
   用手機打開這個網址即可。

## 二、加到手機主畫面

- **iPhone**：用 Safari 開網址 → 底部「分享」→「加入主畫面」→ 加入。
  之後從主畫面點開是全螢幕、無網址列的獨立視窗。
- **Android**：用 Chrome 開網址 → 右上角選單 →「安裝應用程式」或「加到主畫面」。

## 三、之後怎麼更新

把新的 `index.html` 上傳到 repo 覆蓋舊檔（Add file → Upload files → Commit）。
手機下次連網開啟時會自動抓到新版本；資料不受影響。

## 四、三個人怎麼共用

每個人各自把網址加到主畫面，帳存在各自手機。
需要同步時，在 App 的「備份」分頁產生備份碼傳到群組，對方貼上匯入即可。
