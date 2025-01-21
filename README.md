# Meister Online

---

## About

[旧Meister Online](https://meister.ne.jp/index2.html)に代わる新たなブログシステム

markdownファイルはgithub actionsを通じてhugoによって変換され、静的なwebサイトとしてサーバーで公開される。

[新Meister Online](https://meister.ne.jp)にて公開されるほか、サーバーダウンなどに備え[この組織のgithub pages](https://titechmeister.github.io/)によっても同様のサイトが公開されている。

## Project layout


    ├─ archtypes/       default Markdown
    ├─ public/
    ├─ asset            esbuildによりバンドルされるファイル群
    │  ├─ js/           script群
    │  └─ sass/         scss/sass群
    ├─ static           baseurl直下に配置されるファイル群
    │  ├─ js/           script群
    │  ├─ img/          トップページの背景
    │  └─ css/          css群
    ├─ content/         投稿されたMarkfile群
    ├─ layouts          htmlに変換するときのテンプレート
    │  ├─ _default/     Markdownを変換するときのテンプレート
    │  ├─ _shortcodes/  ショートコード
    │  └─ partial/      各componentのテンプレート
    └─ resources/       esbuildから出力されたファイル群

## Usage

ビルドする方法

```shell
$ cd /path/to/MeisterOnline
$ yarn
$ hugo server
```

記事の更新

```shell
$ cd /path/to/MeisterOnline
$ hugo new post/{year}/{month}/{day}/index.md
```

1日に複数の記事を更新したい場合

```shell
$ hugo new post/{year}/{month}/{day}/{ArticleNum}/index.md
```
