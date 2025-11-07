# ge--mu

このリポジトリの簡単な説明と、アプリアイコンの使い方を記載します。

## 追加したファイル

- `icons/icon.svg` — ページ内のアイコンおよびファビコンに使うシンプルな SVG。
- `index.html` — クリック可能なアイコンを表示するサンプルページ（ファビコン設定を含む）。

## アイコンをクリックしてサイトに移動させる方法

`index.html` の中でアイコンは以下のように定義されています。

```html
<a class="app-icon" href="https://example.com" target="_blank" rel="noopener noreferrer">
  <img src="icons/icon.svg" alt="App icon">
</a>
```

リンク先を変更するには、`href` の値を目的の URL に書き換えてください（例: `https://your-site.example`）。

## 参考: PWA/ホーム画面に追加したい場合

将来的に「ホーム画面に追加」などの PWA 機能を使いたい場合は、以下の追加が必要です。

- `manifest.json`（アイコンの複数サイズ、名前、開始 URL などを定義）
- サービスワーカーの登録（オフライン対応など）

必要なら、PWA 用の `manifest.json` と簡単なサービスワーカーのひな形を追加します。
