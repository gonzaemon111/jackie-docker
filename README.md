# Jackie

## ディレクトリ構成

**client**ディレクトリと**server**ディレクトリは、

`git submodule`で管理している

  ```
    Jackie
      ┣━ mysql (mysqlのdataディレクトリ)
      ┃
      ┣━ client (Nuxtのディレクトリ)
      ┃   ┣━ Dockerfile
      ┃   ┣━ package.json
      ┃   ┣━ yarn.lock
      ┃   ┣━ .nuxt (dir)
      ┃   ┣━ assets (dir)
      ┃   ┣━ components (dir)
      ┃   ┗━ ...
      ┃   
      ┣━ server (Ginのディレクトリ)
      ┃   ┣━ Dockerfile
      ┃   ┣━ Gopkg.toml
      ┃   ┣━ main.go
      ┃   ┣━ .env
      ┃   ┣━ models (dir)
      ┃   ┣━ controllers (dir)
      ┃   ┗━ ...
      ┃
      ┣━ .gitignore
      ┣━ .gitsubmodule
      ┣━ docker-compose.yml
      ┗━ valriables.env
  ```

Docker for Macで環境を構築しており、

clientもserverもいずれもホットリロードで開発ができる。