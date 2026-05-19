# 📰 Tech News 朝刊

技術ニュース & セキュリティニュースのデイリーポータル。

**[k02miu.github.io/tech-news](https://k02miu.github.io/tech-news/)**

## 構成

```
.
├── index.html              # ポータル
├── tech/                   # 🔧 技術ニュース (毎朝 9:00 JST)
│   ├── index.html          #   一覧
│   └── YYYY-MM-DD.html     #   日別アーカイブ
├── security/               # 🛡️ セキュリティニュース (毎朝 8:00 JST)
│   ├── index.html          #   一覧
│   └── YYYY-MM-DD.html     #   日別アーカイブ
├── css/style.css           # スタイルシート
└── README.md
```

## 仕組み

[OpenClaw](https://github.com/openclaw) の cron ジョブにより毎朝自動生成:

1. SearXNG で対象スタックの最新情報を検索
2. 一次情報を `web_fetch` で確認
3. Discord チャンネルに配信
4. HTML を生成してこのリポジトリにプッシュ
5. GitHub Pages で自動公開

## 対象スタック

`web / Next.js / Java / Python / Django / Hono / GCP / AWS / Azure / React / SpringBoot / OpenClaw / Claude`

## リンク

- [curation.exe.xyz](https://curation.exe.xyz/) — 技術情報キュレーション（プライベート）
