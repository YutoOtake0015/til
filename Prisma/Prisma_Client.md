# 説明
Prismaの機能の1つで、DBの操作をJavaScriptで実現する機能。
***
例えば、以下の記述において、**create**はPrisma Clientの機能。
DBにデータを登録する。
```javascript
await prisma.users.create({
  ...
})
```
