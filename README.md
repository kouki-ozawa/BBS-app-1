##概要
開発中の掲示板アプリ

## 構成

- **backend**: Ruby on Rails + SQLite  
  - Railsの設定でSQLiteのDBファイルは通常ファイルシステム上に作成されます。
  - Docker Composeでは、ホストとのボリュームマウントは行っていませんが、必要に応じて設定できます。

- **frontend**: Next.js  
  - frontendフォルダ内はNext.jsプロジェクトとして構築されています。
  - npm run devで開発サーバが起動します。

## 起動方法

1. プロジェクトルートで以下を実行
    ```bash
    docker-compose up --build
    ```
2. backendはポート3002、frontendはポート3001でアクセス可能です。

---
