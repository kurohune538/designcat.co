# designcat.co

株式会社DesignCat のコーポレートサイト。HTML/CSS のみの静的サイトで、GitHub Pages で公開しています。

- `index.html` / `styles.css` — サイト本体（`main` ブランチに push すると自動で反映）
- `assets/` — ロゴ（公式データ `Design Cat inc完.ai` から抽出した SVG）、favicon、OGP画像
- `CNAME` — カスタムドメイン `designcat.co`

ブランドカラー: 濃緑 `#066839` / 緑 `#39B54A` / 墨 `#333132`

## DNS（お名前.com）

1. お名前.com Navi →「ネームサーバーの設定」→ designcat.co を「お名前.comのネームサーバーを使う」に変更（以前は AWS Route 53 の NS が入っていたが、ゾーンが削除されていて名前解決できない状態だった）
2. 「DNS関連機能の設定」→「DNSレコード設定を利用する」で下記5件を追加
3. 反映後（数時間〜最大72時間）、GitHub の Settings → Pages で「Enforce HTTPS」をオンにする

| ホスト | タイプ | 値 |
| --- | --- | --- |
| （空欄） | A | 185.199.108.153 |
| （空欄） | A | 185.199.109.153 |
| （空欄） | A | 185.199.110.153 |
| （空欄） | A | 185.199.111.153 |
| www | CNAME | kurohune538.github.io |
