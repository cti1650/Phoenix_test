# Myapp

To start your Phoenix server:

  * Run `mix setup` to install and setup dependencies
  * Start Phoenix endpoint with `mix phx.server` or inside IEx with `iex -S mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## 環境変数の作成

```
cp .env.example .env
```

## データベースの作成

```
docker compose run --rm app mix --version
docker compose run --rm db psql --version
docker compose up -d
docker compose run --rm app mix ecto.create
```

## Learn more

  * Official website: https://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Forum: https://elixirforum.com/c/phoenix-forum
  * Source: https://github.com/phoenixframework/phoenix

## 参考サイト
- [【2023年版】DockerでElixir/Phoenix1.7系の環境を立ち上げる #Docker - Qiita](https://qiita.com/Nexus0831/items/fd988c2781aa74b9710f)  
