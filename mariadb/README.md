###起動の仕方
```java
docker compose up -d
```
<font color="blue" >compose.yamlのディレクトリで実行すること</font>

| 環境変数             | 意味                     | 
| -------------------- | :----------------------- | 
| MARIADB_ROOTPASSWORD | ルートユーザのパスワード | 
| MARIADB_DATABASE     | データベース名           | 
| MARIADB_USER         | データベースのユーザ名   | 
| MARIADB_PASSWORD     | データベースのパスワード | 
[DockerHub:mariadb](https://hub.docker.com/_/mariadb)
###　コンテナの中に入る
```
docker compose exec /bin/bash
```

### データベースへログインする
```
mariadb -u testuser -D testdb -p
```