

指定されたRGBにもとに[インデックスカラー](インデックスカラー.md)を作成する[GDライブラリ](GDライブラリ.md)の関数の一つ。

allocateの意味は、「割り当てる」

サンプルコード
```php
$colorIndex = imagecolorallocate($image, 255, 0, 0);
```