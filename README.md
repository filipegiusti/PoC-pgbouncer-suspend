# PoC-pgbouncer-suspend

This is a PoC on how to use pgbouncer to suspend and resume traffic to a Postgres DB

## Usage

```sh
docker-compose up
bin/benchmark_initialize
bin/benchmark_connection_pooler [SECONDS]
bin/send_command_to_pgbouncer "PAUSE"
bin/stop_database
bin/start_database
bin/send_command_to_pgbouncer "RESUME"
```
