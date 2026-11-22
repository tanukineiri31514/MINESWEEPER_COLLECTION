# MINESWEEPER COLLECTION

ゲーム選択画面と24版・POLYGON版のセットです。

## このZIPのままGitHub Pagesで公開する場合

ルートの `index.html` がゲーム選択画面です。

- 選択画面 → `24SWEEP/index.html` / `POLY/index.html`
- ゲーム → ヘッダーの「← ゲーム選択」から `../index.html`

それぞれの `index.html`, `style.css`, `script.js` はゲームごとのフォルダにあります。
元のゲームのルール、JS、表示演出は変更していません。

## ゲームを別々のGitHubリポジトリで公開する場合

各ゲームの `index.html` に追加したリンク先を、ゲーム選択ページの実際の公開URLに変えてください。

```html
<a class="ghost-button collection-link" href="https://ユーザー名.github.io/コレクションのリポジトリ名/">← ゲーム選択</a>
```

この例のURLはプレースホルダーです。実際に使うURLに置き換えてください。
各ゲームの `style.css` 末尾にもリンク用のCSSを追加しているので、ゲームを個別更新する際には **HTMLとCSSの両方** をコピーしてください。

ゲーム選択ページの `index.html` の2つのカードの `href` も、各ゲームの公開URLに変更してください。

## 変更点

- 24版／POLYGON版それぞれのヘッダーに「← ゲーム選択」を追加
- リンクの見た目を既存のボタンに統一
- スマホではヘッダーボタンが収まるように折り返す
- ゲームロジックのJavaScriptは変更なし
