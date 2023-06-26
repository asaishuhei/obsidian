 #php #GD #function 

画像の[アルファチャンネル](アルファチャンネル.md)(透明度)を保持するかどうかを`true`か`false`で指定する[GDライブラリ](GDライブラリ.md)の関数の一つ。

透明部分がある[画像リソース](画像リソース.md)を扱う際、`imagesavealpha`関数を`true`に指定しないとデォルトで`false`となっているため、透明部分が黒く塗りつぶされる。

### サンプルコード
```php
imagesavealpha($image, true)
```