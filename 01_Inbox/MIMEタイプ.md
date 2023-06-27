 
MIMEタイプとは、インターネット上でデータの種類や形式を識別するためのラベル。

MIMEタイプを指定しなければ、MIMEタイプはデフォルトで以下のように決まる。

- HTMLであれば`text/html`
- [Javascript](Javascript.md)であれば`application/json`
- 画像ファイル（PNG,JPEG）であれば`image/png`と`image/jpeg`

なので、[GDライブラリ](GDライブラリ.md)をつかって画像データを送信したいときはMIMEタイプを画像タイプに設定する必要がある。

[Cakephp](Cakephp.md)2であれば
```php
$this->response->type('image/png');
```
のようにして設定できる。