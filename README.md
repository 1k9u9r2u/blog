## App URL

### **https://guarded-temple-00608.herokuapp.com/users/2**


<p>アプリ名・ブログアプリ</p>

<p>機能・ログイン、ログアウト、新規投稿、編集、削除</p>

<p>開発環境</p>
html css/ruby on rails

テスト用アカウント等
メールアドレス: sample@gmail.com
ユーザー名:山田太郎
パスワード: buyer123
https://gyazo.com/de3f1bb5ca6855bb7782e6e97223e44f

## usersテーブル
|Column|Type|Options|
|------|----|-------|
|email|string|null: false|
|password|string|null: false|
|nickname|string|null: false|
### Association
- has_many :posts


## postsテーブル
|Column|Type|Options|
|------|----|-------|
|text|text|null: false|
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user
