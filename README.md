# list-app

## MySql 接続 & データ作成

- MySql 接続

```
brew services start mysql@8.0
```

- MySql ログイン

```
mysql --user=root --password
```

- データベース作成

```
CREATE DATABASE list_app;
```

- 確認

```
SHOW DATABASES;
```

- データベース指定

```
USE list_app;
```

- テーブル作成

```
CREATE TABLE items (id INT AUTO_INCREMENT, name TEXT, PRIMARY KEY(id));
```

- 確認

```
SHOW TABLES;
```

- 確認

```
DESCRIBE items;
```

- 適当な値を挿入

```
INSERT INTO items (name) VALUES ('じゃがいも'), ('にんじん'), ('とまと');
```

- 値削除

```
DELETE FROM items WHERE id=<id>;
```

- テーブル削除

```
DROP TABLE items;
```

- データベース削除

```
DROP DATABASE list_app;
```

> データベースの変更を行う API は "redirect" を用いる

```
res.redirect(<path>);
```
