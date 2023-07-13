## 一般的なGitコマンド

### リポジトリの管理

- git init: Gitの初期化・設定開始
- git status: ワークツリーのステータスを表示
- git config: 設定周りの確認・変更
- git log: ログを表示
- git diff: ファイルの差分を表示

### ステージングとコミット
- git add: ステージングエリアに追加
- git commit: コミットの実行
- git commit --amend --no-edit: コミットの修正

### ファイルの操作
- git checkout: ファイルの復元や過去コミットの復元（変更がステージングエリア内にある場合）
- git reset: コミットのリセット
- git revert: コミットの変更を打ち消すコミット
- git rm: ファイルの削除とインデックス情報の削除

### リモートリポジトリとの連携
- git clone: リポジトリをコピー
- git pull: リモートリポジトリの同期
- git push: 変更をアップロードする
- git request-pull: プルリクエスト（変更依頼）
- git remote: リモートリポジトリの設定
### ブランチの操作
- git branch: ブランチの作成
- git checkout: ブランチの切り替え
- git merge: ブランチの統合
- git push: 変更をアップロードする


## 一般的なGitフロー

### リポジトリの作成またはクローン
- git init（新規作成）
- git clone <repository URL>（既存のリポジトリをクローン）

### ブランチの作成
- git branch <branch>

### ブランチの切り替え
- git checkout <branch>

### コードの変更とコミット
- ファイルを編集し、git add <file>でステージングし、git commit -m 
"commit message"でコミットする

### リモートリポジトリへのプッシュ
- git push -u origin <branch>

### プルリクエストまたはマージリクエストの作成
- コードの変更を他の開発者に通知し、コードのレビューやマージを行う

### レビューと修正
- コードの変更に対するフィードバックを受け、必要な修正を行う

### マージ
- コードが承認されたら、マージを実行して変更を本番環境に統合する

### - メインブランチへのマージ
- 開発が安定し、テストが完了した場合は、メインブランチにマージする