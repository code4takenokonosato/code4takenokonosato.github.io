# Code for Takenoko no Sato

VRSNS「cluster」の居住地、フォレストヒルズ タケノコの里から始まるシビックテック・コミュニティのティザーサイトです。

## ローカルで見る

GitHub Pages の公開元を **Deploy from a branch / `/docs`** に設定して、そのまま配信できる構成です。ビルド工程はありません。

```sh
python3 -m http.server 8000 --directory docs
```

ブラウザで `http://localhost:8000` を開いてください。

## GitHub Pages 設定

リポジトリの **Settings → Pages → Build and deployment** で次のように設定します。

- Source: `Deploy from a branch`
- Branch: 公開対象のブランチ / `/docs`

`docs/.nojekyll` を含めているため、Jekyllによる変換を行わず静的ファイルがそのまま公開されます。
