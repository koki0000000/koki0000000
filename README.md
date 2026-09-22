# Koki.m

データアナリスト。Gmail・Notion・Discord をつないで、手入力をなくす仕組みを作っています。

## 動かしているもの

自分の家計の処理を自動化して、毎日動かしています。

| | |
|---|---|
| 記帳 | カード会社の利用通知メールを1分おきに読み、日付・店名・金額を取り出して家計簿へ |
| 訂正 | 分類が外れたら通知のボタンで直す。履歴が溜まった店は次から正しい分類に入る |
| 照合 | 明細CSVを台帳と1件ずつ突合。毎月3社、直近は漏れ0件 |
| 取得 | 各社サイトへログインして領収書と明細を取得。自動のものと手で起動するものがある |
| 監視 | 定期実行25本・常時起動8本の処理を台帳と毎日照合し、止まっていれば通知。監視も同じ機械の上で動く |

## 公開しているもの

- [ledger-starter](https://github.com/koki0000000/ledger-starter): 上の「記帳」を切り出したもの。Google Apps Script と Notion だけで動く。三井住友・楽天カード・ビューカード対応
- [Ledgermail](https://koki0000000.github.io/ledgermail/): 同じ仕組みを製品にしようとしたときのページ。デモ動画つき

## 使うもの

Python / TypeScript / Google Apps Script / SQL
Notion API / Cloudflare Workers + D1 / Discord Bot / Playwright
