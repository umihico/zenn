# Zenn CLI

* [📘 How to use](https://zenn.dev/zenn/articles/zenn-cli-guide)

> 以下のコマンドによりmarkdownファイルを簡単に作成できます。

```bash
$ npx zenn new:article
```

## 画像

[参照](https://zenn.dev/zenn/articles/deploy-github-images#%E7%94%BB%E5%83%8F%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AE%E9%85%8D%E7%BD%AE%E3%83%AB%E3%83%BC%E3%83%AB)

画像ファイルはリポジトリ直下の /images ディレクトリに配置します。 /images ディレクトリの中の構造に制限はありませんが、拡張子だけはチェック対象となります。

```
.
├─ articles
│  └── example-article-1.md
└─ images
   ├── example-image1.png
   └── example-article-1
```

画像の参照方法
画像は、記事の本文や、本のチャプターの本文から参照することができます。参照するには、画像埋め込み記法の URL 部分に /images/ から始まる絶対パスを指定します。相対パスで指定しないようご注意ください。

```markdown
![](/images/example-image1.png)
![](/images/example-article-1/image1.png)
```
