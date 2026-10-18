# MyDrive 網站

MyDrive 的公開首頁、隱私權政策與服務條款。此 repo 只放靜態網站；桌面程式的原始碼由維護者另外管理。

| 頁面 | 網址 |
| --- | --- |
| 首頁 | https://bos-tw.github.io/mydrive-site/ |
| 隱私權政策 | https://bos-tw.github.io/mydrive-site/privacy.html |
| 服務條款 | https://bos-tw.github.io/mydrive-site/terms.html |

## GitHub Pages 設定

Settings → Pages → Deploy from a branch → `main` → `/ (root)`。

網頁為原生 HTML／CSS，沒有編譯步驟、外部字型、分析或追蹤指令碼。根目錄的 `.nojekyll` 讓 GitHub 直接發布靜態檔案。

## Google Search Console

網站發布成功後，在 Search Console 選「網址前置字元」資源，填入首頁網址。使用 Google 為你的帳戶提供的 HTML 驗證檔或 `<meta name="google-site-verification">` 標記；HTML 檔放在 repo 根目錄，meta 標記放在 `index.html` 的 `<head>`。保持檔名與內容不變，再 commit、push，等待部署成功後完成 Google 驗證。

此 repo 未填入假的驗證碼。Search Console 驗證成功不保證 OAuth 品牌審核或授權網域檢查通過，須以 Google 的實際結果為準。Google 登入仍由 MyDrive 桌面程式接收本機回呼，此網站不處理權杖。

原創網站程式碼採 MIT 授權，見 [LICENSE.txt](LICENSE.txt)。
