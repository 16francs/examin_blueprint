## Auth [/auth]
### ログイン情報取得 [GET]
+ Request (application/json)

	+ Headers

			access-token: 認証用のアクセストークン

+ Response 200 (application/json)
	+ Attributes (AuthUser)
		+ status: success

+ Response 401 (application/json)
	+ Attributes (ErrorUnauthorized)

### ログイン [POST]
+ Request (application/json)
	+ Attribute (LoginForm)

+ Response 200 (application/json)
	+ Attributes
		+ status: success
		+ access_token: 認証に使用するアクセストークン (string)
		+ user
			+ id (number)
			+ role (number)

+ Response 401 (application/json)
	+ Attributes (ErrorUnauthorized)

### ログアウト [DELETE]
+ Request (application/json)

	+ Headers

			access-token: 認証用のアクセストークン

+ Response 200 (application/json)
	+ Attributes
		+ status: success

+ Response 401 (application/json)
	+ Attributes (ErrorUnauthorized)
