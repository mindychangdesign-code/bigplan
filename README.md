# Mindy Chang — 作品集網站

一個乾淨、響應式的靜態作品集網站,以純 HTML / CSS / JavaScript 打造,不需要任何建置工具。

原本希望直接從 [mindychang.webflow.io](https://mindychang.webflow.io/) 匯入內容,但此環境的網路政策無法連線到該網域,因此這個版本是依照常見作品集網站版面重新設計的起點,**內容多為預留文字(標記 `TODO`),請替換成真實資訊**。

## 結構

```
index.html            主頁面(Hero / 關於我 / 作品集 / 專長 / 聯絡方式)
assets/css/styles.css 樣式(含淺色 / 深色模式)
assets/js/main.js     行動選單、年份等互動
assets/img/           放置實際作品圖片的資料夾(目前為空,作品卡片先以色塊呈現)
```

## 待你替換的內容

在 `index.html` 中搜尋 `TODO` 可以快速找到所有需要更新的地方,包含:

- Hero 自我介紹文字
- 關於我的段落與經歷、所在地
- 四個作品卡片的標題、分類、描述與連結(可替換 `assets/img/` 底下的真實截圖,並把 `.work-thumb` 換成 `<img>`)
- 聯絡方式(Email、LinkedIn、Instagram 等連結)

## 本機預覽

不需要安裝任何套件,直接用瀏覽器開啟 `index.html`,或用簡易伺服器:

```bash
python3 -m http.server 8000
# 開啟 http://localhost:8000
```

## 部署到 GitHub Pages

1. 到 repo 的 **Settings → Pages**
2. Source 選擇欲發布的分支(例如 `main`)與根目錄 `/`
3. 儲存後,網站會發布在 `https://<你的帳號>.github.io/<repo 名稱>/`

如需自訂網域,可在 Pages 設定中加入 Custom domain,並在 DNS 設定對應的 CNAME 記錄。
