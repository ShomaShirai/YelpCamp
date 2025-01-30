# YelpCamp(Udemy)

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

# 参考資料(公式ドキュメント第一)
- MongoDB(https://www.mongodb.com/ja-jp/docs/manual/installation/)
- Mongoose(javascript)(https://mongoosejs.com/)