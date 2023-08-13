# 環境構築の方法

1. 任意のディレクトリでgit cloneを行いローカルで開発できるようにする。
    ```
    git clone <リポジトリ名>
    ```
2. docker compose upでdockerを起動する。
   ```
   docker compose up -d
   ```
3. dockerのコンテナ内に入る
    ```
    docker compose exec web bash
    ```
4. データベースを作り、migrateする
    ```
      rails db:create
      rails db:migrate
    ```
5. サーバーを起動する
    ```
    rails s -b 0.0.0.0
    ```
