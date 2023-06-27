 

[メモリ](メモリ.md)上に確保した[画像リソース](画像リソース.md)を破棄する[PHP](PHP.md)の関数

[imagecreatefrompng](imagecreatefrompng.md)などで画像リソースを確保したら、適切に破棄しないと[メモリ](メモリ.md)の使用量が増えて圧迫する可能性がある。

引数の詳細
```php
imagedestroy ( resource $image )
```

注意点として、一つのリソースIDを複数の変数で管理している場合、被っているIDすべてが削除される。

なので`if (get_resource_type($new_image) === 'gd')`でまだ消されていないリソースをあぶりだす必要がある。