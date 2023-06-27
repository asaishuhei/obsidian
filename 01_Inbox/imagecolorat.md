

画像の特定のx,y座標の[インデックスカラー](インデックスカラー.md)を返す[GDライブラリ](GDライブラリ.md)の関数の一つ。

サンプルコード
```php
$pixelColor = imagecolorat($image, $x, $y);
```

imagecoloatは6桁の16進数を返す。
各RGB値にアクセスするには[ビットシフト](ビットシフト.md)と[ビットマスク](ビットマスク.md)を用いる。

サンプル
```php
$im = imagecreatefrompng("php.png");  
$rgba = imagecolorat($im, 10, 15, 23);  
$a = $rgb >> 24;  
$r = ($rgb >> 16) & 0xFF;  
$g = ($rgb >> 8) & 0xFF;  
$b = $rgb & 0xFF;
```