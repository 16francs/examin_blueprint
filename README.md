# Examin (仕様書)

[仕様書: API Blueprint](https://github.com/nishikawatadashi/examin_blueprint)     
[フロントエンド: Vue.js](https://github.com/nishikawatadashi/examin_vue)     
[バックエンド: Rails API](https://github.com/nishikawatadashi/examin)     

## 導入方法

* 必要なライブラリのインストール(Mac OS)

> $ brew install node     
> $ npm install -g aglio

####  (インストール時エラーが出る場合)

* nodeのバージョンが高すぎるのが原因の場合

参考: [nodebrewでnodeのバージョンを切り替える方法](https://qiita.com/kuriya/items/36ae29366df0b7c95dec)

1. 今まで使っていた ```node``` のアンインストール

    > $ brew uninstall --ignore-dependencies node

2. ```nodebrew``` のインストール

    > $ brew install nodebrew

3. ```nodebrew``` のセットアップ

    > $ nodebrew setup

4. バージョンを指定してインストール

    > $ nodebrew ls-remote     
      $ nodebrew install-binary 'node version'

(補足)

* 安定板: ```$ nodebrew install-binary stable```
* 最新版: ```$ nodebrew install-binary latest```

* パスの通し方
    * bash
    > export PATH=$HOME/.nodebrew/current/bin:$PATH

    * fish
    > set -U fish_user_paths "$HOME/.nodebrew/current/bin/" $fish_user_paths


## HTMLファイルの生成方法

* 以下のコマンドを実行して起動する

> $ aglio -i examin.apib -o examin.html


* 上記コマンドを実行後, ```examin.html``` を開くとHTML形式で閲覧できる

## サーバーを起動して確認する場合

* 以下のコマンドを実行して起動する

> $ aglio -i examin.apib --server

* 表示されるURLにアクセス(デフォルトの場合，以下のリンクにアクセス)

> http://localhost:3000

