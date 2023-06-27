


指定したRGB値とアルファ値（透明度）を持つRGBA値に対する色IDを作成することができる[GDライブラリ](GDライブラリ.md)の関数の一つ。

[imagecolorallocate](imagecolorallocate.md)のアルファを追加した関数。



### サンプルコード
```php
imagecolorallocatealpha($image, $red, $green, $blue, $alpha);
```

```php
$newRGB = imagecolorallocatealpha($image, 255, 255, 3, 3);

//$newRGBの16進数の返り値
//11 11111111 11111111 00000011
```