# PoC-pgbouncer-suspend

This is a PoC on how to use pgbouncer to suspend and resume traffic to a Postgres DB

## Usage

```sh
docker-compose up
bin/benchmark_initialize
bin/benchmark [SECONDS]
bin/pause
bin/resume
```
