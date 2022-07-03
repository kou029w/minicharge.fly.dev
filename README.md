# minicharge.fly.dev

## 前提

- PostgreSQL

## 構築

```sh
git clone git@github.com:kou029w/minicharge.fly.dev.git
curl -L https://fly.io/install.sh | sh
flyctl auth login
flyctl launch
flyctl secrets set DATABASE_URL=postgres://*** # PostgreSQL接続URLを設定
flyctl deploy
```
