# making-game-while-eating-out-with-claude-20260718

スマホで一人・オフラインで遊べる簡単なゲーム集。

## 2048

[`index.html`](./index.html) — 単一ファイルのHTMLゲーム。

- **遊び方**: タイルをスワイプ（PCは矢印キー / WASD）。同じ数字がぶつかると合体し、`2048` を目指します。
- **オフライン対応**: 外部リソース・通信は一切なし。ファイルをブラウザで開くだけで動きます。
- **スマホ最適化**: 片手でのスワイプ操作、レスポンシブなレイアウト、画面拡大の抑制。
- **データ保存**: ベストスコアは端末の `localStorage` に保存されます。

## GitHub Pages で公開する

このリポジトリには自動デプロイ用のワークフロー（`.github/workflows/pages.yml`）が含まれています。

1. GitHubでこのリポジトリの **Settings → Pages** を開く
2. **Build and deployment → Source** を **「GitHub Actions」** に設定
3. 対象ブランチ（`claude/mobile-offline-game-ideas-w6irjx` または `main`）にpushされると自動でデプロイされます

公開後のURL:

```
https://reikashiwabara.github.io/making-game-while-eating-out-with-claude-20260718/
```

スマホのブラウザでこのURLを開くだけで遊べます（初回読み込み後はオフラインでもプレイ可能）。

### ローカルで開く場合

`index.html` をダウンロードして、スマホの「ファイル」アプリなどからタップして開くだけでも動きます。インストール不要です。
