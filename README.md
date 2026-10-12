# YouTube Planner

動画案・台本・アナリティクス・メモを管理する静的Webアプリ(index.html 1ファイルのみ)。

## GitHub Pagesで公開する手順
1. GitHubで新しいリポジトリを作成(例: `youtube-planner`)
2. `index.html` と `README.md` をリポジトリ直下にアップロード
3. Settings > Pages > Source を `Deploy from a branch`、Branch を `main` / `(root)` にして Save
4. 数分後、`https://<ユーザー名>.github.io/youtube-planner/` で開けます

## 機能
- アナリティクス: 動画のリンクから再生回数・いいね・題名・長さ・投稿日を取得。投稿日の新しい順で表示し、列ごとのフィルター・並び替えが可能
- 動画作成案: 台本(話者・内容・コピー)、構成・概要、案ごとのToDo、CSV書き出し(ゆっくりムービーメーカー4 Lite用)。並び替えと、投稿予定日までの残り日数表示
- 設定: APIキー、登録者数・目標、動画種別、話者の追加・編集・削除

## API設定
Google Cloud Consoleで「YouTube Data API v3」を有効化してAPIキーを発行し、設定タブに入力します。
キーはコードに書かず、画面から入力してください(ブラウザ内にのみ保存されます)。

## データ保存
入力内容はブラウザのlocalStorageに保存されます(端末間の同期はありません)。
