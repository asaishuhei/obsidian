 

```php
$this->Form->create('モデル名', array('action' => 'アクション名'));
```
モデルを使わない場合は`'モデル名'`の部分を`false`にする

```php
$this->Form->text('モデル名', array('属性' => '10'));
```

```php
$this->Form->submit('ボタン表記名');
```

```php
 $this->Form->end();
```

これらを使うときは`<?php echo $this->Html->pre($data); ?>`の通りに`echo`をつける

