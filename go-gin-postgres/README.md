# Go と postgresql を Docker で構築する

1. docker をビルドする。

```bash
$ docker compose build
```

2. docker を起動する。(`-d`はバックグラウンドで起動するオプションなのでお好み)

```bash
$ docker compose up -d
```

3. コンテナ内部に接続する。

```bash
$ docker exec -it <container_name> /bin/bash
```
