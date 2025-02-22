# YelpCamp(Udemy)：キャンプ場サイト

## 開発環境
- Windows 11 WSL2
- VScode

## サーバーサイドでMongoDBを起動する方法
```
- サーバーを起動する
$ sudo systemctl start mongod
- サーバーの自動起動
$ sudo systemctl enable mongod
- データベース起動
$ mongosh
- サーバーの状態を確認
$ sudo systemctl status mongod
- サーバの停止
$ sudo systemctl stop mongod
- 「ctrl + c」を二回押すことでmongoshを停止できる
```

## 手順
- mongoshでサーバー起動する
- seeds/index.jsから情報をサーバーへ送信
- nodemon app.jsでポートの起動，mongodbと接続

# ノート
- useCreateIndexは，mongoose6.0以降で使わない
- ミドルウェアとはリクエストとレスポンスの間で，ターミナルにログを出力，パスワードのチェックで使える
- bootstrap5はjQueryの依存関係が無くなった
- expressのエラー処理でミドルウェアを用いる
- expressにはデフォルトでエラー処理をするミドルウェアがある
- サーバーサイドでエラーハンドリングを行わないようにする
- エラーハンドリングは画面を使わずリクエストをポストする場合(サーバーサイドからのリクエスト)の対策を行うべきである
- Joiはスキーマのバリデーションを行う
- リレーションとはデータベースの関係
- 一対多ではテーブルが二つ必要であるが，多対多の場合はテーブルが三つ必要である
- populateでたくさんのデータを関連させる
- 親の参照を子が持つか，子の参照を親が持つか
- express.Routerではapp.getなどのルーティングをひとまとまりにしてくれる
- クッキーとは特定のブラウザを閲覧する場合に，ブラウザに保存される小領域の情報のこと(セッション管理，パーソナライゼーション，トラッキング)
- res.cookieでクッキーを渡すことができる．cookie-parserですべてのリクエストにクッキーを渡すことができる
- セッションとはhttpをステートフルにするために使用するサーバー側のデータストア．クッキーにデータを保存するのではなく，サーバー側で保存する．express-sessionを用いる
- flashを用いることで一度だけユーザーに表示したい情報を乗せることができる

# 参考資料(公式ドキュメント第一)
- MongoDB(https://www.mongodb.com/ja-jp/docs/manual/installation/)
- Mongoose(javascript)(https://mongoosejs.com/)
- Expressの公式ドキュメント(https://expressjs.com/ja/guide/writing-middleware.html)