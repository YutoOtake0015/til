# 説明
Prismaの機能の1つで、DB操作をJavaScript/TypeScriptで実現する機能。

ローカル環境では、`npx prisma generate`でDB操作で使用するコードのライブラリを生成する。
格納場所: node_modules/.prisma/client

## ライブラリは以下を含む
 - 型付けされたデータベースクライアント:
   - Prisma Client主要部分。
   - データベースとの実際のやり取りを行う部分で、接続情報やトランザクション管理をする。
 - 型定義:
   - schema.prisma ファイルに基づいて、JavaScript/TypeScriptのコードで使用される型が生成される。
   - データベースとのやり取りが型安全になる。
 - クエリエンジン:
   - Prisma Clientの背後で動作するバイナリファイル。
   - 実際のデータベース操作を担当する。
 - モデルに基づくCRUD API:
   - 各モデルに対して、CRUD操作をサポートするAPIが生成される。
 - 関連するヘルパーAPI:
   - リレーションやトランザクションなど、データベース操作に関連する追加のAPIを提供する。
 - ランタイム:
   - PrismaClientのランタイム。
   - エリの生成や実行、クエリエンジンとの通信など、PrismaClientの動作に必要なコードを含む。

***
# 例
例えば、以下の記述を実行する場合
```javascript
await prisma.users.create({
  ...
})
```
1. `prisma.users.create()`のPrismaClient APIが呼び出される。
2. ランタイムにより、`prisma.users.create()`がSQLに変換され、クエリエンジンに渡される。
3. クエリエンジンにより、SQLクエリはDBに送信され、レスポンスを受け取る。
4. クエリエンジンは、レスポンスをランタイムに渡し、その結果がコードとして表示される。



