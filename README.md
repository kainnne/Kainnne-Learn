# Kain³e Academy

課程、文章與未來影片教學的公開入口，連到 WikiNB 和 Kain³e AI。沿用主頁的粉紅、薰衣草、淡藍、薄荷、玻璃材質與深淺色。

## 維護

- `content.json`：真實內容的名稱、中英標題、分類、標籤與網址。`video` 可放影片或播放清單的公開網址；不放私人教材或題庫。
- `site.json`：正式網址、主頁、AI 及 GitHub。正式網址為 https://academy.kainnne.com/，由 GitHub Pages 部署。
- `index.template.html`、`styles.css`、`app.js`：版面、樣式、搜尋、分類、語言與主題。
- `npm run build && npm run check`：產生並檢查 `dist/`。無第三方建置依賴。
- `.github/workflows/pages.yml`：推送 main 後部署 GitHub Pages。

影片尚未加入時，影片分類如實顯示空狀態；沒有虛構影片、片長或完成紀錄。內容清單先使用已有的公開 WikiNB 課程與文章，文章正文維持在 WikiNB。

## 網址變更

日後變更子網域時，更新 `site.json` 的 `url`，同步 Pages 的自訂網域與 DNS，並在建置輸出加入對應 CNAME。主頁 `Me/src/projects.json` 的教學卡片網址也要一起更新。目前 CNAME 為 academy.kainnne.com。
