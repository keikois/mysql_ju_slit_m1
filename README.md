# mysql_ju_slit_m1

## M1Mac対応版
jupyterlabとMySQL&amp;phpMyAdminとstreamlitがセットになったdocker-composeのディレクトリです。

## 使い方
```
mysql_ju_slit
├── db => (MySQLのデータ保存場所)
├── work => （jupyterlabのコードを保存する場所）
├── struns => (streamlitを実行するapp.pyを入れる場所。必要に応じ、requirements.txtも、ここにおいてください。)       
└── docker-compose.yml
```
- ターミナルで下記のコードを実行
```
git clone git@github.com:keikois/mysql_ju_slit_m1.git
```
```
cd mysql_ju_slit　
```
```
docker-compose up -d
```

- localhost:8888でjupyterlabが起動
- localhost:8080でphpMyAdminが起動
- streamlit run <app.pyのパス> でstreamlitが起動

- streamlitはcontrol + C で終了します。
- docker-compose down　でdocker-composeを終了できます。

## git cloneが終ったら
git cloneが終ったら、リモートリポジトリを削除するコマンドを使ってください。

Git のリモートリポジトリを削除するコマンド
```
git remote rm origin 
```
Gitのリモートリポジトリを確認するコマンド
- 何も書かれていないことを確認してください。
```
git remote -v 
```
