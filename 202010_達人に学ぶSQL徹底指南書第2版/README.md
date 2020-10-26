# SQL実行までの手順

```bash
docker network create shared-network
cd rdbms
docker-compose up -d --build
cd -
cd jupyter
docker-compose up -d --build
cd -
```

localhost:28888を開くとjupyterが起動する。
work/以下のノートブックを開いて演習を実施する。

手元からDBに繋ぐ場合は

```bash
psql -U root -h localhost -p 25432 -d sandbox
```

sqlファイルを実行する場合は

```bash
psql -f hoge.sql -U root -h localhost -p 25432 -d sandbox
```