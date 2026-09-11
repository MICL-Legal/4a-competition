# 4a-competition

2026 4A 工作坊「部門 AI 化」競賽規章（對外發布頁）。

## 發給全公司的網址是 `/a/`，不是根目錄

**https://micl-legal.github.io/4a-competition/a/**

Notion 頁面「2026年 部門AI化競賽：浴火鳳凰Phoenix Rising」的「競賽規章」區塊連的就是這個網址，已發給 13 個部門主管。

## 四個網址都不能刪

`/`、`/a/`、`/b/`、`/c/` 是**同一份 v6 規章內容的四種視覺設計**，不是四個不同版本的草案。內容逐項相同（續燃期、火焰、績效加分、春酒、30 個加分池計數全部一致），只有排版與配色不同。

| 網址 | 設計 | 狀態 |
|---|---|---|
| `/a/` | 方案 A 烈焰 | **採用中，Notion 對外連結指這裡** |
| `/` | 基本版 | 保留 |
| `/b/` | 方案 B 神話典藏 | 保留 |
| `/c/` | 方案 C 極簡現代 | 保留 |

GitHub Pages 的網址就是路徑，**刪掉任何一個目錄就是讓那個網址 404，而且沒有 redirect**。2026-09-10 曾誤刪 a/b/c，導致 `/a/` 中斷約 12 小時，恰好落在主管回報參賽資料的截止日（9/11）。已於 2026-09-11 revert 復原，blob SHA 與刪除前一致。

## 內容源頭

單一真相源是私有 repo `MICL-Legal/4A--ideas` 的 `handout/`，手動同步到本 repo：

| 本 repo | 源頭 |
|---|---|
| `index.html` | `handout/regulations.html` |
| `a/index.html` | `handout/opt-a.html` |
| `b/index.html` | `handout/opt-b.html` |
| `c/index.html` | `handout/opt-c.html` |

改規章要改源頭再同步，兩邊都要 push。
