

ピクセル(画像の特定のx,y座標)のRGBA値を取得する[GDライブラリ](GDライブラリ.md)の関数の一つ。

各RGBA値に対して[ビットシフト](ビットシフト.md)と[ビットマスク](ビットマスク.md)を行う必要がないので、コードを短縮できる。

各RGBA値にアクセスするサンプル。

```php
// 画像をオープンします  
$im = imagecreatefrompng('nexen.png');  
  
// 色を取得します  
$start_x = 40;  
$start_y = 50;  
$color_index = imagecolorat($im, $start_x, $start_y);  
  
// 可読形式にします  
$color_tran = imagecolorsforindex($im, $color_index);

//各RGB値にアクセス
$alpha = $color_tran['alpha'];
$red = $color_rtan['red']
$green = $color_rtan['green']
$blue = $color_rtan['blue']
```

$color_tranの中身
```php
Array
(
   [red] => 226
   [green] => 222
   [blue] => 252
   [alpha] => 0
)
```