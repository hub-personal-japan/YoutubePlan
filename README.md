# YouTube案作成表

動画案・台本・アナリティクスを管理する静的Webアプリ(index.html 1ファイルのみ)。

## GitHub Pagesで公開する手順
1. GitHubで新しいリポジトリを作成(例: `youtube-planner`)
2. `index.html` と `README.md` をリポジトリ直下にアップロード
3. Settings → Pages → Source を `Deploy from a branch`、Branch を `main` / `(root)` にして Save
4. 数分後、`https://<ユーザー名>.github.io/youtube-planner/` で開けます

## アナリティクスの取得
- **再生回数・いいね**: Google Cloud Consoleで「YouTube Data API v3」を有効化し、APIキーを発行 → アプリのAPIキー欄に入力 → 動画URLまたは動画IDを入れて「取得」
  (APIキーは公開リポジトリのコードに書かず、アプリの入力欄から入れてください。ブラウザ内にのみ保存されます)
- **再生時間・収益**: YouTube Studioのアナリティクスから動画別データをCSVでエクスポート → 「CSV取り込み」

## データ保存
入力内容はブラウザのlocalStorageに保存されます(端末間の同期はありません)。
