# MySQLのインストール手順
## MacOS
1. インストール
```terminal
brew install mysql
mysql --version
echo 'export PATH="/usr/local/opt/mysql/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
mysql --version
```

2. パスワード登録
```terminal
brew services start mysql@5.7
mysql -u root

mysql> update mysql.user set password=password('PassWord12345!') where user = 'root';
mysql> flush privileges;
mysql> exit;
```

3. パスワード登録確認
```terminal
mysql --user=root --password
mysql> exit;

brew services stop mysql@5.7
```


