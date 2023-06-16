 #php #GD #function 

`imagecreatefrompng`とは、指定したpng画像を[画像リソース](画像リソース.md)に確保する[PHP](PHP.md)の[GDライブラリ](GDライブラリ.md)の関数である。

画像を加工したいときに利用する。

### サンプルコード
```php
// コンテンツがPNG画像であることをブラウザーにお知らせ
header ('Content-Type: image/png');

// ファイルを画像リソースを確保
$img = imagecreatefrompng('sakura.png');

// 画像リソースからPNGファイルを出力
imagepng($img);

// 画像リソースを破棄
imagedestroy($img);
```

- 最初に[PHP](PHP.md)ファイルではなく、画像を表示するために[MIMEタイプ](MIMEタイプ.md)を指定する。
- [画像リソース](画像リソース.md)を取得する
- [imagepng 関数](imagepng%20関数.md)で画像を出力
- [imagedestroy 関数](imagedestroy%20関数.md)で[メモリ](メモリ.md)のお掃除