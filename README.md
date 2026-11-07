# Icon Atlas — Tabler Icons 繁體中文語意搜尋

[![License: MIT](https://img.shields.io/badge/Code%20License-MIT-blue.svg)](LICENSE) [![Tabler Icons](https://img.shields.io/badge/Tabler%20Icons-3.50.0-478fbb.svg)](https://github.com/tabler/tabler-icons)

**非官方、獨立的 Tabler Icons 中文搜尋工具**。讓使用者透過「蘋果、圖釘、訊號、鎖住、取用」等繁體中文名稱、動作及用途，尋找 Tabler Icons 中的 Outline／Filled SVG。

## 網址

部署 GitHub Pages 後，預計入口：

**https://yiminghu0125-svg.github.io/icon-atlas-zh/**

> 這個網址必須先建立公開 GitHub Repository、上傳檔案及啟用 GitHub Pages 才會生效。請勿在發布前視為已上線。

## 功能

- 完整列出 `@tabler/icons@3.50.0` 的官方索引及 Outline／Filled 圖示。
- 自訂繁體中文同義詞、常見英文單詞直譯、物件名稱、動作及用途搜尋。
- 官方英文名稱／Tags 搜尋、官方分類、用途分類、多詞 AND／OR、排序、分頁。
- 圖示預覽、複製名稱與 Vue 元件語法、複製／下載官方 SVG。
- 收藏清單、僅看收藏及收藏 CSV 匯出（儲存在本機瀏覽器）。
- 桌面與手機排版；捲動時縮小固定搜尋工具列；**沒有快速搜尋範例區塊**。

## 技術與執行方式

- 網站入口：**`index.html`**，沒有編譯、後端、資料庫、API Key 或 npm 安裝程序。
- 可直接雙擊 `index.html` 或使用一般靜態網站主機開啟。
- 官方圖示索引及 SVG 首次載入**需要網路**：jsDelivr CDN，索引失敗時嘗試 unpkg。
- 目前固定使用 `@tabler/icons@3.50.0`，不會自動切換最新版，避免新增／移除圖示使對照失準。
- 中文匹配採詞庫與規則式排序，**不是 LLM 即時語意推論，也不是官方逐筆中文翻譯**。

## 專案結構

```text
icon-atlas-zh/
├── index.html                         # GitHub Pages 網站首頁（原本的中文搜尋 HTML）
├── README.md                          # 使用與部署說明
├── LICENSE                            # 本網站程式 MIT License
├── THIRD_PARTY_NOTICES.md            # 第三方來源及聲明
├── licenses/
│   └── TABLER_ICONS_LICENSE.txt      # 官方 Tabler Icons MIT 授權原文
├── .nojekyll                          # 停用 GitHub Pages Jekyll 預處理
└── .gitignore
```

## 授權與歸屬

**本網站程式／自訂中文詞庫**採 [`MIT License`](LICENSE)；**Tabler Icons** 採其獨立的 MIT License，Copyright (c) 2020–2026 Paweł Kuna。完整聲明參見 [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md) 與 [`licenses/TABLER_ICONS_LICENSE.txt`](licenses/TABLER_ICONS_LICENSE.txt)。

本站未取得 Tabler Icons 官方背書，也不隸屬 Tabler；圖示及官方英文資料的著作權仍屬其原權利人。

## 隱私及維護注意

搜尋不需要登入；收藏僅存在瀏覽器儲存空間（清除瀏覽資料可能遺失）。第三方 CDN 仍會接收圖示相關的網路請求。未來更新官方圖庫版本時，應同步更新 `index.html` 的 `VERSION`、README 與第三方通知，並驗證載入數量及搜尋結果。
