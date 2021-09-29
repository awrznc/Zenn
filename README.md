Zenn
===

Zennのコンテンツを管理するためのリポジトリです。<br>
https://zenn.dev/awrznc


## Zenn CLI

以下の記事を参考に環境構築・及び執筆を行います。

* [📘 How to install](https://zenn.dev/zenn/articles/install-zenn-cli)
* [📘 How to use](https://zenn.dev/zenn/articles/zenn-cli-guide)


## 環境構築

Dockerを利用した環境構築を以下に示します。

```bash
# Linux or macOS
docker run --rm -it -v "$(pwd):/opt" --workdir="/opt" -p "8000:8000" node:16 bash -c "npm install && npx zenn preview"

# Windows (Git Bash)
powershell 'docker run --rm -it -v "$(pwd):/opt" --workdir="/opt" -p "8000:8000" node:16 bash -c "npm install && npx zenn preview"'

# => http://localhost:8000
```
