# 教學足跡｜年度評鑑佐證中心

不需建置的靜態網站，可部署至 GitHub Pages。預設 115 學年度，透過 Google 表單上傳附件，由已安裝的 Google Apps Script 依年度與評鑑項目歸檔。

## 架站

1. 將本資料夾內容放在 GitHub 儲存庫根目錄（index.html 必須在根目錄）。
2. 開啟 Settings → Pages。
3. Source 選 Deploy from a branch，Branch 選 main，資料夾選 / (root)，儲存。
4. 等待 GitHub 顯示正式網站網址。

GitHub Free 可由公開儲存庫發布 Pages；私人儲存庫是否可使用 Pages 取決於方案。一般 Pages 網站對外公開，即使原始碼儲存庫是私人也不代表網站是私人。

## 使用

1. 輸入評鑑學年度（例如 115）。
2. 搜尋或選擇教學、研究、輔導與服務項目。
3. 按上傳，網站會把年度與項目帶入 Google 表單。
4. 填寫佐證名稱、成果日期及附件後提交。
5. 開啟雲端資料夾確認歸檔結果。

新年度、面向及項目資料夾會於第一次提交時自動建立。每次提交有獨立 EV_編號資料夾，保留檔案及佐證資訊.json。網站只提供分類與上傳入口，不讀取實際附件數量或計算評鑑分數。

## Google 設定

config.json 保存表單網址、資料夾網址、預填欄位代碼。這些是連結與表單欄位代碼，不是密碼或存取權杖。Google 的表單／雲端硬碟權限獨立管理；公開 GitHub 不會自動公開其中的佐證檔案。

現有表單、自動化程式及 Google 雲端硬碟均已在原帳號建立，不需要因網站搬遷而重新安裝。請不要將佐證檔案、原始評鑑 Excel 或帳號憑證上傳到 GitHub。

rules.json 的教學與服務 63 個分類取自「教師評鑑 Agent MVP.xlsx」中的「113評鑑規則」；研究僅設待分類收件項目。這些不代表 115 學年度的正式規則，正式分類修訂時須同步更新網站與 Google 表單／歸檔程式。

技術參考：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
