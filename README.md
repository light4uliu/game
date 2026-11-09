# 神殿遊戲室

埃及風的原創網頁小遊戲網站，純靜態網頁（HTML、CSS、JavaScript），不需要建置工具。

## 內容

- **聖符守衛戰**：墓穴迷宮射擊遊戲，共 8 關。（`shengfu/`）
- **神殿五子棋**：15×15 五子棋，可對電腦（學徒、祭司、法老）或雙人同機。（`wuzi/`）
- 關於、隱私權政策、聯絡頁。

遊戲的畫面、音樂與音效皆由程式即時繪製、合成，沒有使用外部圖片或音檔。

## 檔案結構

```
index.html        首頁
about.html        關於
privacy.html      隱私權政策
contact.html      聯絡
404.html          找不到頁面
style.css         共用樣式
favicon.svg       網站圖示
robots.txt        搜尋引擎設定
shengfu/          聖符守衛戰（index.html 說明頁、game.html 遊戲本體）
wuzi/             神殿五子棋（index.html 說明頁、game.html 遊戲本體）
```

## 用 GitHub Pages 架站

1. 到 repo 的 **Settings → Pages**。
2. Source 選 **Deploy from a branch**，Branch 選 `main`，資料夾選 `/ (root)`，按 Save。
3. 等一兩分鐘，網址會顯示在同一頁。

所有連結都是相對路徑，放在子路徑（例如 `帳號.github.io/game/`）或自己的網域底下都能正常運作。

## 之後綁定自己的網域

1. 在 Pages 設定的 **Custom domain** 填入網域，GitHub 會自動建立 `CNAME` 檔。
2. 到網域商設定 DNS 指向 GitHub Pages（依 GitHub 官方說明）。
3. 勾選 **Enforce HTTPS**。
4. 網域確定後，補上 `sitemap.xml`，並在 `robots.txt` 加一行 `Sitemap: https://你的網域/sitemap.xml`。
5. 若日後使用 Google AdSense，通過後把 `ads.txt` 放在根目錄，並同步更新 `privacy.html` 中的廣告說明。

## 授權

版權所有 © 2026 四月老師。未經同意，請勿轉載、重製或將遊戲放到其他網站。
