 #cakephp2 #form #post 

postされたデータをコントローラで受け取るとき、
`$this->request->data`で受け取ると配列になる
例
```php
array(1) {

  ["exel_data"]=>

  string(9) "ｗｗｗ"

}
```

対策として`$this->request->data('exel_data')`のように要素を指定することで文字列になる