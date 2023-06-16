 #php #server #variable 

### $\_SERVERとは
- [PHP](PHP.md)における[スーパーグローバル変数](スーパーグローバル変数.md)の一つ
- ヘッダ情報、パス情報、スクリプトの位置を取得できる。

### 各サーバー変数
- `$_SERVER['PHP_SELF']`は` /test.php/foo.bar`のような現在実行しているスクリプトルートを取得できる。脆弱性があるらしい。
- `$_SERVER['REQUEST_TIME']`はリクエスト開始時のタイムスタンプを取得できる。