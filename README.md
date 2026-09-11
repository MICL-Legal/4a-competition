# 4a-competition

2026 4A 工作坊「部門 AI 化」競賽規章（對外發布頁）。

## 發給全公司的網址是 `/a/`，不是根目錄

**https://micl-legal.github.io/4a-competition/a/**

Notion 頁面「2026年 部門AI化競賽：浴火鳳凰Phoenix Rising」的「競賽規章」區塊連的就是這個網址，已發給 13 個部門主管。

## 現有兩個路徑，都不可刪

| 網址 | 設計 | 狀態 |
|---|---|---|
| `/a/` | 方案 A 烈焰 | **採用中，Notion 對外連結指這裡** |
| `/` | D 青金典雅（主網址） | 保留 |

GitHub Pages 的網址就是路徑，**刪掉目錄就是讓那個網址 404，而且沒有 redirect**。

2026-09-10 曾誤刪 `a/ b/ c/`，導致 `/a/` 中斷約 12 小時，恰好落在主管回報參賽資料的截止日（9/11）。已於 2026-09-11 revert 復原，blob SHA 與刪除前一致。事故與防範見記憶 `00_刪除上線資源前必查實際發布通路`。

## 已下架的設計

`/b/`（方案 B 神話典藏）與 `/c/`（方案 C 極簡現代）於 2026-09-11 依 Ever 指示下架。下架前已查證零引用：Notion 全workspace 搜尋只連 `/a/`、GitHub code search 全帳號 0 筆、本機 `~/repo` `~/Documents` `~/Desktop` 0 筆、頁面之間無互連。

設計原稿仍在私有 repo `MICL-Legal/4A--ideas` 的 `handout/opt-b.html`、`handout/opt-c.html`，要回復隨時可以。

## 內容源頭

單一真相源是私有 repo `MICL-Legal/4A--ideas` 的 `handout/`：

| 本 repo | 源頭 |
|---|---|
| `index.html` | `handout/regulations.html` |
| `a/index.html` | `handout/opt-a.html` |

改規章要改源頭再同步，兩邊都要 push。原本的四版同步腳本 `gen_variants.py` / `_publish.py` 放在 job 暫存目錄、已隨目錄清除，現在是兩份手動同步。
