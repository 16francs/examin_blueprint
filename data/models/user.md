## AuthUser
+ user
	+ id: 1 (number) - ユーザID
	+ `login_id`: `login_id` (string) - ログインID
	+ name: name (string) - 名前
	+ school: school (string) - 塾名
	+ role: 1 (number) - 権限
+ `api_key`
	+ `access_token`: `access_token` (string) - アクセストークン
	+ `expires_at`: `2018-01-01 00:00:00` - トークン有効期限

## User
+ user
	+ id: 1 (number) - ユーザID
	+ `login_id`: `login_id` (string) - ログインID
	+ name: name (string) - 名前
	+ school: school (string) - 塾名
	+ role: 1 (number) - 権限
	+ `created_at`: `2018-01-01 00:00:00` (string) - 登録日時
	+ `updated_at`: `2018-01-01 00:00:00` (string) - 更新日時
	
## LoginForm
+ `login_id`: `login_id` (string, required) - ログインID
+ password: password (string, required) - パスワード

## UserForm
+ user
	+ `login_id`: `login_id` (string, required) - ログインID
	+ name: name (string, required) - 名前
	+ school: school (string, required) - 塾名
