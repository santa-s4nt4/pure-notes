# pure-notes

[pure](https://github.com/santa-s4nt4/pure-editor) から明示的に公開した記事だけを保存するリポジトリです。
[poin7s.com](https://poin7s.com/) が公開用の `index.json` と Markdown を読み込みます。

- `posts/<タイトル>--<記事ID>.md`: 公開記事の本文。名前が変わっても記事 ID とサイト URL は維持します。
- `assets/<SHA-256>.webp`: 公開記事から参照される画像だけ。
- `index.json`: 公開記事の一覧と、公開設定の世代情報。非公開に戻した記事は一覧・本文・未使用画像から取り下げます。

非公開記事の本文・タイトル、pure の同期インデックス、認証情報は保存しません。
以前に公開した内容の Git 履歴と、第三者が保存したコピーは取り下げ後も残り得ます。
公開設定の世代情報には、取り下げ済みの記事 ID と設定 ID だけが残ります。

記事は pure の「この記事を公開する」「この記事を非公開にする」から管理してください。
GitHub で本文や index.json を直接編集すると pure 側の内容と競合する場合があります。

接続手順: [GitHub 公開の設定](https://github.com/santa-s4nt4/pure-editor/blob/main/docs/github-publishing.md)
