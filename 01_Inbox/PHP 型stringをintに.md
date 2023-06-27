 

[PHP](PHP.md)において[cakephp2 コントローラでPostされたデータを受け取る](cakephp2%20コントローラでPostされたデータを受け取る.md)や[cakephp2 FormHelperの使い方](cakephp2%20FormHelperの使い方.md)でtextやtextereaでpostされたデータは入力された値が半角数字であっても`string`型になる。

対策として
```php
intval(対象)
```
でint型にすることができる