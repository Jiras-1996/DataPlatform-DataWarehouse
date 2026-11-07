# ClickHouse

Run ClickHouse independently from this folder with `docker compose up -d`. Copy `.env.example` to `.env` first and set a strong password. Its data and logs are stored in Docker volumes.

- HTTP interface: `http://localhost:8123`
- Native protocol: `localhost:9002`
- From another container on `data-platform-network`: `clickhouse:8123` (HTTP) or `clickhouse:9000` (native)

Create the shared network once before starting either service: `docker network create data-platform-network`.
