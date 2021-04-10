# 環境構築
Docker image をbuildする。
```
docker-compose build
```

## Rails
bundle install を実行する。
```
docker-compose run backend bundle
```
DBを作成する。
```
docker-compose exec backend bin/rails db:create
```

## Nuxt
npm install を実行する。
```
docker-compose run frontend npm i
```

## 確認
`http://localhost:3000/` にアクセスしてNuxtの画面が表示されたら成功🎉