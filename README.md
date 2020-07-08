## 手順
1. Dockerが入っている環境でこのリポジトリを `git clone` する
1. `docker-compose build` でdockerイメージを作成
1. `docker-compose up -d` でコンテナを立ち上げる
1. `docker-compose exec app rails webpacker:install` でappコンテナにwebpackerをインストール
1. `docker-compose exec app rails db:create`でDBを作成する
1. [http://localhost/](http://localhost/)にアクセスしてアプリが立ち上がっていることを確認する。以上。

## 参考文献
- [【Rails6】Docker+Rails6+puma+nginx+mysql【環境構築＊初心者必見】](https://qiita.com/kohki4115/items/c37ff8550b01bbc75df2)