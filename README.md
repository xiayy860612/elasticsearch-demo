# Elasticsearch Demo

## Elasticsearch Cluster

make sure vm.max_map_count at least 26144, or cluster will create failed.

```
$ sudo sysctl vm.max_map_count
$ sudo sysctl -w vm.max_map_count=262144
```

run cluster

```
$ docker-compose -f docker-compose-cluster.yml up -d
```

shutdown cluster
```
$ docker-compose -f docker-compose-cluster.yml down
```

---
[Elasticsearch Doc]: https://www.elastic.co/guide/index.html
[docker-compose v3]: https://docs.docker.com/compose/compose-file/