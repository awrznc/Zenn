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


## LICENSE

基本的には[こちら](LICENSE)のライセンスがこのプロジェクトのライセンスです。

上記とは異なる `LICENSE` ファイルが存在しているディレクトリがあった場合は、そのファイルが存在しているディレクトリ以下のコンテンツにはその `LICENSE` の内容が適用されます。

また、コンテンツの文章内にライセンスが記述されている場合は、文章内で明記した範囲に記述したライセンスの内容が適用されます。


### ライセンスの適用例

以下のようなディレクトリ構成だった場合の適用例を示します。

```bash
./
├── contents.md
├── LICENSE
└── sub/
    ├── sub/
    |   └── contents.md
    ├── contents.md
    └── LICENSE
```

`./contents.md` には `./LICENSE` の内容が適用されます。

`./sub/contents.md` 及び `./sub/sub/contents.md` には `./sub/LICENSE` の内容が適用されます。
