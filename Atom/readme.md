## Atom について

### 1. 入れるべきパッケージ
・`tag` html で``</``を打ち込むと勝手に補完してくれる  
・`japanese-menu` メニューの日本語化  
・`linter` スペルミスとかエラー出してくれる  
・`linter-htmlhint`  linter の html 版  
・`linter-php` linter の php 版   
linter-php は設定が必要で git からファイルとってきたりいろいろめんどい．
いつかやりかたまとめるつもり  
・`linter-python-pep8` linter の python 版 pep8 に対応  
・`highlight-selected` ダブルクリックした単語と同じ単語を表示してくれる  
・`minimap` 右側にコードのミニマップ表示  
・`file-icons` file のアイコンを GUI っぽく表示   
・`atom-beautify` きれいなコードに変換してくれる   
右クリックから beautify editer contents を選ぶか `Ctrl+Alt+B` でできる  
・`git-puls`  使わないほうがよさそう．使ったら conflict 起きた．使うにしても下のターミナル開いてコマンド打てばよさそう．用勉強  
・`Platformio Ide Terminal`  Atom 上でターミナルを開ける．`Ctrl+Shift+\``で開ける．何も設定しなかったら windows の場合デフォルトが Power Shell になっている．   
`cmd` にする場合，パッケージ設定の shell override に `C:\Windows\System32\cmd.exe` を記述したらコマンドプロンプトが使える．  
`Anaconda prompt` にする場合はパッケージ設定の shell override に `C:\Windows\System32\cmd.exe` を Core に `C:\Anaconda3\Scripts\activate.bat root` を記述したらアナコンダプロンプトが使える．仮想環境を使わない場合は root を，仮想環境を指定する場合はその名前にする．


### 2. 変えるべき setting   
setting からタブの可視化，インデントのライン揃えをオンにしたほうがみやすい

### 3. Atom コマンド集
Atom のコマンド集．一部 Atom 以外のコマンドも使えるものはのせる．  
`Ctrl+Shift+A` 全行選択  
`Ctrl+/` 指定された行をコメントアウト  
`Ctrl+Shift+P` Atom コマンド表示  
`Ctrl+Shift+\`` ターミナルを開く  
`Ctrl+Alt+B` コード整形    
