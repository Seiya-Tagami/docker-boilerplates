# Go と postgresql を Docker で構築する。

### 基本操作

1. コンテナをビルドする。

```bash
$ docker compose build
```

2. コンテナを起動する。(`-d`はバックグラウンドで起動するオプション)

```bash
$ docker compose up -d
```

3. コンテナ内部に接続する。

```bash
$ docker exec -it <container_name> /bin/bash
```

### Go の起動について

- `go run main.go`で基本的には動作します。ただ、ホットリロードツールの Air も導入しているので、単に`air`と打つだけでも動作するようになっています。

### 注意

- 必要に応じて、各種の名前や設定を変更してください。
