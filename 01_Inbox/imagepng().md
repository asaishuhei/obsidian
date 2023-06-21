 #php #GD #function 

画像データを出力できる[PHP](PHP.md)の関数。

パスで指定した画像を出力したい場合は、[imagecreatefrompng 関数](imagecreatefrompng%20関数.md)で[画像リソース](画像リソース.md)上に確保し、[MIMEタイプ](MIMEタイプ.md)を`image/png`にしておく必要がある。

### 引数の内容

```php
imagepng ( resource $image [, string $filename [, int $quality ]] )
```
- $image:画像リソースを指定
- $filename:ファイルに保存したい時に、ファイル名を指定する
- $quality:品質レベルを1~9(高品質~低品質)で指定できる