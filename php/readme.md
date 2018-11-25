## PHP について

### 1．インストール(環境造り)

web サーバ系の環境は LAMP 環境が一般的(linux,apache,mysql,php)．ただ windows じゃ使えないから windows 含めて全部のプラットフォームで使える環境を作ろうというのが xampp 環境(x(マルチプラットフォーム),apache,mysql,php)

とりあえず xampp つかっとけば OK な感じ．インストールも公式サイトからダウンロードしてインストールするだけだからめっちゃ簡単．

使い方は `xampp control panel` 開いて apache,mysql とかの start,stop 押すだけでできる．ただGUIベースでしかできないからコマンドでやる場合は個別に入れるのがいいかも．一応 php と mysql は xampp の path を追加するだけでコマンドが使える．
環境変数の path に
```
C:\xampp/php
C:\xampp/mysql/bin
```
を追加するだけ．

ちなみに mysql の操作は phpmyadmin が使われている．xampp の phpmyadmin には apache,mysql を start してから以下の URL で入れる．
[`http://localhost/phpmyadmin/index.php`](http://localhost/phpmyadmin/index.php)

用語説明  
・`Apache` 開発用の無料のレンタルサーバ  
・`mysql` データベース作成のためのツール．基本はコマンドでやる  
・`phpmyadmin` コマンドでやるのがめんどい人向け．GUI で mysql ができる．git でいう sourcetree みたいなもの．

apacheの入り方は xampp の start 押して[`http://localhost/`](http://localhost/)で入れるがこれだと初期の dashbourd が表示される．初期状態では`C:/xampp/htdocs`が読み込まれてるのでそのディレクトリに`C:/xampp/htdocs/php/index.php`を作って[`http://localhost/php/index.php`](http://localhost/php/index.php)に入るか初期ディレクトリの設定を変えるかすること．

### 2.phpの使い方

●コマンド  
`php -v`
でバージョン確認  
`php index.php` で php の実行

●php のビルトイン web サーバの使い方  
`php -S 192.168.0.19:8000` でサーバを立てて[`http://192.168.0.19:8000/hoge.php`](http://192.168.0.19:8000/hoge.php)から入れる．
`192.168.0.19`の部分が ip アドレスで`8000`の部分がポート番号

`http://192.168.0.19:8000/hoge.php`の`hoge.php`部分が使いたい phpファイル.なにも指定しなかったら同ディレクトリの`index.php`が勝手に読み込まれる．サーバを立てる時に使いたい php があるディレクトリからコマンドを打つこと．ip が知りたい場合は`ipconfig`とかのコマンド使う．まあ apache 使うならビルトインサーバの使用場面はほとんどなさそうだけど．．．
