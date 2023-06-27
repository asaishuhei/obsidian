

[PHP](PHP.md)において、`echo "Hellow World";`などの出力を[バッファリング](バッファリング.md)機能をONにして保持することができる。

`ob_get_contents`で出力したデータを取得、これを変数に入れるなどしてバッファリングを外で使う。

最後に`ob_end_clean`でバッファリングを終了する。

サンプル
```php
// 出力バッファリングを開始
ob_start(); 

// イメージを出力バッファに保存
imagepng($new_image);

// 出力バッファの内容を取得
$image_data = ob_get_contents(); 

ob_end_clean(); // 出力バッファリングを終了
```
上記のコードは[imagepng](imagepng.md)してしまうと画像をその場で出力してしまうので、それを防ぐことができる。