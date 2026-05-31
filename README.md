# 🗣️ 族語翻譯互動學習 — Klokah Translator

> 串接 **族語E樂園** (klokah.tw) 公開 API 的台灣原住民族語翻譯互動學習頁面。

![preview](https://web.klokah.tw/image/og-image.jpg)

## ✨ 功能特色

- **16 種族語 × 42 種方言** 完整收錄（阿美語、泰雅語、布農語、排灣語…）
- **36 類單詞分類**（身體部位、動物、植物、顏色、飲食、親屬稱謂…）
- **🃏 卡片模式** — 大字顯示族語、中文、英文對照
- **📋 列表模式** — 整頁瀏覽，快速掃讀
- **🔊 點擊發音** — 播放原住民語真人錄音
- **🔍 即時搜尋** — 輸入中文或族語關鍵字即刻過濾
- **⌨️ 鍵盤快捷** — 左右方向鍵翻頁，空白鍵播放發音

## 🚀 快速開始

### 本機執行

```bash
# 任何靜態檔案伺服器均可
python3 -m http.server 8080
# 或
npx serve .
```

### Zeabur 部署

1. Fork 或 clone 此專案到你的 GitHub
2. 登入 [Zeabur](https://zeabur.com)
3. 點擊 **New Project** → **Deploy from GitHub**
4. 選擇此 repo → Zeabur 自動偵測為靜態網站
5. 部署完成 ✅

## 🏗️ 專案結構

```
klokah-translate/
├── index.html       # 主頁（完整 SPA 應用）
├── README.md        # 專案文件
├── package.json     # Zeabur 靜態網站設定
└── .gitignore       # Git 忽略規則
```

## 🔌 API 來源

資料來自 [族語E樂園](https://web.klokah.tw)（原住民族語言研究發展基金會）

| API | 說明 |
|------|------|
| `php/getWords.php?did={方言ID}&cate={分類}` | 取得單詞列表 |
| `audio/word/{方言ID}/{編號}.wav` | 單詞發音音檔 |

## 📜 授權

本專案為非官方獨立開發，資料版權歸 **財團法人原住民族語言研究發展基金會** 所有。
