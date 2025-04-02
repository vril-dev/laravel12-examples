# laravel12-examples

### 開発環境

バックエンド ... `laravel12`, http://localhost:3030  
フロントエンド ... `react` `nextjs`, http://localhost:3000  

## 準備

```sh
docker compose build backend
docker compose build frontend
docker compose up -d backend mysql84

## Larvelインストール
docker compose exec -u ${APP_BACKEND_USER_ID} backend composer install

## フロントエンド準備
docker compose run --rm -u ${APP_BACKEND_USER_ID} frontend npm install
docker compose up -d frontend
```
