# このアプリについて
[pyscript](https://pyscript.net/) の学習を目的としたものです。


# 環境について
webapp のバンドラーに [parcel](https://ja.parceljs.org/) を使用しています。

| 環境                                          | バージョン | 備考               |
| --------------------------------------------- | ---------- | ------------------ |
| [pyscript](https://pyscript.net/)             | alpha      |                    |
| [parcel](https://ja.parceljs.org/)            | v1.12.5    | package.json から  |

# pyscript について
下記のように CDN を利用しています。

```
<link rel="stylesheet" href="https://pyscript.net/alpha/pyscript.css" />
<script defer src="https://pyscript.net/alpha/pyscript.js"></script>
```

Download から下記のように指定しようと思ったのですが、

```
<link rel="stylesheet" href="path/to/pyscript.css" />
<script defer src="path/to/pyscript.js"></script>
```

`pyscript.css` や `pyscript.ks` がダウンロードした資産にみつからなかったので諦めました。


# 起動
次の手順で実行してください。

## 1. package.json で管理しているプラグインのインストール

```zsh
$ npm i
```

## 2. アプリ起動

```zsh
$ npm run dev

> pyscript-work@1.0.0 dev /Users/ksh-fthr/workspace/pyscript-work
> parcel index.html

Server running at http://localhost:1234
✨  Built in 211ms.
```

アクセス http://localhost:1234 にブラウザからアクセスすると pyscript で作成した web アプリの挙動が試せます。

