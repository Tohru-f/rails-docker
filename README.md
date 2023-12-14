# README
Railsのタスク管理アプリを立ち上げる方法
対象としたスペック： MAC M2チップ

1. git clone https://github.com/Tohru-f/rails-docker.git でローカルリポジトリに本アプリのリポジトリの内容をコピーしてくる。

2. docker-compose build でイメージファイルを作成する

3. docker-compose up で作成したイメージでコンテナを立ち上げる

4. docker-compose run web rake db:createでデータベースを生成

5. docker-compose run web rails db:migrateで生成したデータベースをマイグレーションする

6. ブラウザを起動してURL欄にlocalhost:3000を入力してタスク管理アプリを表示させる