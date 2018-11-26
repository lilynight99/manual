## Atom について

### 1. 入れるべきパッケージ
・`tag` html で``</``を打ち込むと勝手に補完してくれる  
・`japanese-menu` メニューの日本語化  
・`linter` スペルミスとかエラー出してくれる  
・`linter-htmlhint`  linter の html 版  
・`linter-php` linter の php 版  
linter-php の setting の PFP Excututable Path に php のパスを記述する必要あり．  
xampp の場合 `C:\xampp/php/php.exe` でいける．  
・`linter-python-pep8` linter の python 版 pep8 に対応  
・`highlight-selected` ダブルクリックした単語と同じ単語を表示してくれる  
・`minimap` 右側にコードのミニマップ表示  
・`file-icons` file のアイコンを GUI っぽく表示   
・`atom-beautify` きれいなコードに変換してくれる   
右クリックから beautify editer contents を選ぶか `Ctrl+Alt+B` でできる.  
htmm,javascript,css などは atom-beautify をインストールするだけで使用できるが，PHP などに関しては設定が必要.  
● PHP の設定方法(windows)  
1. [ここ](https://github.com/FriendsOfPHP/PHP-CS-Fixer) の Installation にある  Locally の Download the php-cs-fixer.phar file から php-cs-fixer.phar をダウンロード(いまは php-cs-fixer-v-2.phar らしい)  
1. php-cs-fixer.phar を任意の場所にコピー．`C:\xampp\php\php-cs-fixer.phar` など
1. atom-beautify の設定から Executables を選択し Executables 内の PHP の Binary/Script Path に PHP へのパスを入力し，PHP-CS-Fixer の Binary/Script Path に先ほどコピーした php-cs-fixer-v2.phar へのパスを入力する．  
```
例)
PHP Binary/Script Path : C:\xampp\php\php.exe
PHP-CS-Fixer Binary/Script Path : C:\xampp\php\php-cs-fixer.phar
```


・`git-puls`  使わないほうがよさそう．使ったら conflict 起きた．使うにしても下のターミナル開いてコマンド打てばよさそう．用勉強  
・`Platformio Ide Terminal`  Atom 上でターミナルを開ける．``Ctrl+Shift+` ``で開ける．何も設定しなかったら windows の場合デフォルトが Power Shell になっている．   
`cmd` にする場合，パッケージ設定の shell override に `C:\Windows\System32\cmd.exe` を記述したらコマンドプロンプトが使える．  
`Anaconda prompt` にする場合はパッケージ設定の shell override に `C:\Windows\System32\cmd.exe` を Core に `C:\Anaconda3\Scripts\activate.bat root` を記述したらアナコンダプロンプトが使える．仮想環境を使わない場合は root を，仮想環境を指定する場合はその名前にする．

### 2. 変えるべき setting   
setting からタブの可視化，インデントのライン揃えをオンにしたほうがみやすい

### 3. Atom コマンド集
Atom のコマンド集．一部 Atom 以外のコマンドも使えるものはのせる．  
随時更新

・ Editer 系コマンド． Atom 以外でも使えるものが多い  
`Ctrl+A` 全行選択  
`Ctrl+N` 新しくファイルを作成  
`Ctrl+O` ファイルを開く  
`Ctrl+Shift+O` フォルダを開く  
`Ctrl+S` ファイル保存
`Ctrl+Shift+S` 名前をつけてファイル保存  
`Ctrl+Z` 戻る  
`Ctrl+Shift+Z` 戻しを進める  
`Ctrl+Y` 戻しを進める  
`Ctrl+↑` カーソルがある行を一行上と交換  
`Ctrl+↓` カーソルがある行を一行下と交換  
`Ctrl+←` 文字のまとまり単位で左にカーソル移動  
`Ctrl+→` 文字のまとまり単位で右にカーソル移動  
`Shift+↑` カーソルがある行の一行上まで選択  
`Shift+↓` カーソルがある行の一行下まで選択  
`Shift+←` 左選択  
`Shift+→` 右選択  
`Ctrl+Shift+→` 文字のまとまり単位で右選択  
`Ctrl+Shift+←` 文字のまとまり単位で左選択  
`Ctrl+L` カーソル行選択  
`Ctrl+Shift+K` カーソル行削除  
`Ctrl+/` 指定された行をコメントアウト

 ・その他のコマンド  
`Ctrl+Shift+P` Atom パレット表示  
``Ctrl+Shift+` `` ターミナルを開く  
`Ctrl+Alt+B` コード整形  
`Ctrl+Shift+M` markdown プレビュー  
`Ctrl+,` setting を開く

・ git 系コマンド  
いろいろあるらしいがターミナルでやったほうがコミット，プッシュ，プルあたりの間違い
がなくなるからよさそう．
