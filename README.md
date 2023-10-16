# Meister Online

---

About
-----

[旧Meister Online](https://meister.ne.jp)に代わる新たなブログシステム

markdownファイルはhugoによって変換され、静的なwebサイトとしてサーバーで公開される。

Project layout
--------------

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

Usage
-----

ビルドする方法

```shell
$ cd /path/to/MeisterOnline
$ yarn
$ hugo server
```