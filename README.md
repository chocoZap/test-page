# GitHub Pages 公開手順

このディレクトリは GitHub Pages でそのまま公開できる最小構成です。

## 方法1: GitHub の画面から公開

1. 新しい GitHub リポジトリを作成
2. このフォルダの中身をリポジトリ直下にアップロード
3. GitHub の `Settings` → `Pages` を開く
4. `Build and deployment` の `Source` で **Deploy from a branch** を選択
5. `Branch` は **main** / **/(root)** を選択して保存
6. 数分待つと公開URLが発行されます

公開URL例:
- `https://<GitHubユーザー名>.github.io/<リポジトリ名>/`

## 方法2: GitHub Actions で公開

同梱の `.github/workflows/deploy-pages.yml` を使う方法です。

1. このフォルダの中身を GitHub リポジトリに push
2. GitHub の `Settings` → `Pages` を開く
3. `Source` で **GitHub Actions** を選択
4. `main` ブランチに push すると自動で公開

## 注意点

- 今回の HTML は単体ページなので、`index.html` をそのまま公開できます。
- Notion の外部リンクや外部アイコン参照はそのまま残っています。
- 独自ドメインを使わない場合は追加設定は不要です。
