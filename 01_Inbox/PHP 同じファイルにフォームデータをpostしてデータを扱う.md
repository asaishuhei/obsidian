
 #php #form #post 

[PHP](PHP.md)
手順を以下に示す

## 1.フォームを作成
```php
<form action="" method="post">
        <input type="text" name="input_text">
        <input type="submit">
    </form>
```
このとき`action`は空にする

## 2.postされたデータを受け取る
```php
$user_input =  $_POST["input_text"];
```
これでデータを扱える