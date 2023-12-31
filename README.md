# liberary_for_misken

個人的なweb練習。図書館の蔵書検索機能、貸出機能＋ユーザーによるおすすめ機能、感想投稿等の実装を目指す。

## 開発環境

- Docker (Docker Compose)
  - Nginx
  - MySQL (db)
  - Go (back)
  - React (front)

## 開発形態

- ブランチモデル
  - production (本番環境)
  - development (ステージング環境)
  - feat/xxx (機能追加)
  - fix/xxx (バグ修正)
  - hotfix/xxx (緊急バグ修正)

## 開発手順

### 最初

1. リポジトリをクローンする `git clone https://github.com/saitamau-maximum/maxitter.git`
2. `cd maxitter`でフォルダに移動
3. `cp .env.example .env`で.envファイルを作成
4. `.env`ファイルを自分の好きな名前やパスワードに書き換え
5. `./scripts/setup.sh` でビルドしてコンテナを起動する

### 停止

`./scripts/stop.sh` でコンテナを停止する

### 再開

`./scripts/start.sh` でコンテナを再開する

### DBデータの削除

`./scripts/reset-db.sh` でDBデータを削除する

### デプロイ

`./scripts/deploy.sh` で本番環境にデプロイする
（マイグレーションなど特別なオペレーションが必要な場合もある）


