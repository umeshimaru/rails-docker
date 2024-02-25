# 作成する環境
- ruby 3.2.2
- Rails:7.0.6
- Postgres:version12系


# 環境構築方法

①ローカル環境で任意のディレクトリを作成。
```
mkdir  rails-docker
```
②、①で作成したディレクトリでgit cloneコマンド実行
```
git clone https://github.com/umeshimaru/rails-docker.git
```
③コンテナ作成起動
```
docker compose up
```
④初めて起動する場合下記２つのコマンド実行(データベース作成)
1つ目
```
docker-compose run web rake db:create
```
２つ目
```
docker-compose run web rails db:migrate
```

⑤localhost:3000にアクセスし「Task」,「New task」と表示されていたら完成
```
http://localhost:3000
```
