# Flink on Docker

execute Flink on docker.

## Run

```bash
$ docker compose up -d 
```

### show web ui

`localhost:8081`


### execute task

```bash
# show log in another tab in terminal
$ docker logs -f flink-jobmanager
$ docker logs -f flink-taskmanager

# run WordCount 
$ docker compose exec jobmanager ./bin/flink run ./examples/streaming/WordCount.jar
```


refs: https://nightlies.apache.org/flink/flink-docs-master/docs/deployment/resource-providers/standalone/docker/
