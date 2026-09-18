# TDNA CIS

台灣數位遊牧者協會品牌識別系統 — https://cis.dna.org.tw

- `index.html` — 單頁手冊：品牌介紹、標誌（12 款組合 × 黑白）、色彩、字型、輔助圖形、數位介面 token、下載。
- `assets/tdna.css` — 與 `tdna-console`（console.dna.org.tw）共用的樣式來源；改色彩 token 時兩邊要同步。
- `assets/logo/*.svg` — 出自 `TDNA Brand Assets.ai`，命名 `<組合>-<black|white>.svg`。
- `assets/download/` — VI 2.1 PDF、Brand Assets ZIP、名片 PDF。

靜態站，nginx（`Dockerfile`）。Railway 從 `main` 自動部署。

本機預覽：`python3 -m http.server 8090` 後開 http://localhost:8090 。
