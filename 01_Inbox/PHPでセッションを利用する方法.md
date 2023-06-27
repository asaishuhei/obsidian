 

[PHP](PHP.md)で[セッション](セッション.md)を利用する手順を以下に記す
1. `session_start();`
	- セッションデータを初期化
	- セッションIDを発行、IDが残っているなら読み込む
	- [PHP $SESSION](PHP%20$SESSION.md)を読み込む
2. `$_SESSION['セッションkey'] = 登録する値;`
	- 変数をセッションに登録する
3. 登録されたセッションを使う
	- `echo $_SESSION['登録されたkey']`で使える