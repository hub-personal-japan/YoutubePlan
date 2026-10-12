# YouTube Planner

動画案・台本・アナリティクス・ToDo・メモを管理する静的Webアプリ(index.html 1ファイルのみ)。

## GitHub Pagesで公開する手順
1. GitHubで新しいリポジトリを作成(例: `youtube-planner`)
2. `index.html` と `README.md` をリポジトリ直下にアップロード
3. Settings > Pages > Source を `Deploy from a branch`、Branch を `main` / `(root)` にして Save
4. 数分後、`https://<ユーザー名>.github.io/youtube-planner/` で開けます

## 台本のCSV書き出し
動画作成案 > 書き出し タブで、A列=話者名、B列=セリフのCSV(UTF-8)を保存できます。
ゆっくりムービーメーカー4 Lite の [ツール] > [台本編集] から読み込みます。

## アナリティクスの取得
- 再生回数・いいね: YouTube Data API v3 のAPIキーを画面の入力欄に入れ、動画URLまたは動画IDを入力して「取得」
  (APIキーはコードに書かず、入力欄から入れてください。ブラウザ内にのみ保存されます)
- 再生時間・収益: YouTube Studio で動画別データをCSVでエクスポートし「CSV取り込み」

## データ保存
入力内容はブラウザのlocalStorageに保存されます(端末間の同期はありません)。
