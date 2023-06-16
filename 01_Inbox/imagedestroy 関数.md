 #php #GD #function 

[メモリ](メモリ.md)上に確保した[画像リソース](画像リソース.md)を破棄する[PHP](PHP.md)の関数

[imagecreatefrompng 関数](imagecreatefrompng%20関数.md)などで画像リソースを確保したら、適切に破棄しないと[メモリ](メモリ.md)の使用量が増えて圧迫する可能性がある。

引数の詳細
```php
imagedestroy ( resource $image )
```