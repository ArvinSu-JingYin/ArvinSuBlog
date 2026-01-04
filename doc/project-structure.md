
# 專案目錄結構說明

以下為專案目錄結構樹狀圖：

+```
ArvinSuBlog/
├── _config.yml
├── _config.next.yml
├── _config.landscape.yml
├── package.json
├── README.md
├── db.json
├── LICENSE
├── CONTENT-LICENSE.md
├── source/           # 原始內容資料夾（Markdown 文章與靜態頁面）
│   ├── _posts/       # 部落格文章（Markdown）
│   ├── about/        # 關於頁面內容
│   ├── categories/   # 分類頁面內容
│   └── tags/         # 標籤頁面內容
├── public/           # Hexo 產生的靜態網站檔案（勿手動修改）
│   ├── atom.xml
│   ├── index.html
│   ├── search.xml
│   ├── sitemap.xml
│   ├── 2026/         # 依年份歸檔的文章靜態檔
│   ├── about/        # 關於頁面靜態檔
│   ├── archives/     # 歸檔頁面靜態檔
│   ├── categories/   # 分類頁面靜態檔
│   ├── css/          # 靜態樣式檔
│   ├── images/       # 靜態圖片檔
│   ├── js/           # 靜態 JavaScript 檔
│   └── tags/         # 標籤頁面靜態檔
├── css/              # 全站樣式檔
├── images/           # 全站圖片資源
├── js/               # 全站 JavaScript 程式碼
│   └── third-party/  # 第三方 JS 外掛
│       ├── analytics/    # 分析工具
│       ├── chat/         # 聊天外掛
│       ├── comments/     # 留言外掛
│       ├── math/         # 數學公式外掛
│       ├── search/       # 搜尋外掛
│       ├── statistics/   # 統計外掛
│       └── tags/         # 標籤相關外掛
├── scaffolds/         # 文章、頁面、草稿模板
│   ├── draft.md
│   ├── page.md
│   └── post.md
├── themes/            # Hexo 主題資料夾
└── doc/               # 專案說明文件
  └── project-structure.md
```

本文件說明本專案的主要目錄與檔案結構，方便新成員快速了解專案架構。

## 根目錄
- `_config.yml` / `_config.next.yml` / `_config.landscape.yml`：Hexo 部署與主題設定檔。
- `package.json`：Node.js 專案描述與依賴管理。
- `README.md`：專案說明文件。
- `db.json`：Hexo 生成的資料庫檔案。
- `LICENSE` / `CONTENT-LICENSE.md`：授權條款。

## 內容與文章
- `source/`：原始內容資料夾。
  - `_posts/`：Markdown 格式的部落格文章。
  - `about/`、`categories/`、`tags/`：靜態頁面內容。
- `public/`：Hexo 產生的靜態網站檔案（勿手動修改）。

## 佈景主題與樣式
- `themes/`：Hexo 主題資料夾。
- `css/`、`images/`、`js/`：靜態資源（樣式、圖片、JavaScript）。
  - `js/third-party/`：第三方 JS 外掛。

## 其他
- `scaffolds/`：文章、頁面、草稿模板。
- `archives/`、`categories/`、`tags/`：分類、標籤、歸檔頁面。

---

如需詳細說明，請參閱各資料夾下的 README 或聯絡專案維護者。