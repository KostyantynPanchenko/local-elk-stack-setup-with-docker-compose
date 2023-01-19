# Setting up local Elasticsearch and Kibana with docker-compose

## Soure

[Start a single-node cluster with Docker](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html#docker-compose-file)

```shell
$ wsl -d docker-desktop
sysctl -w vm.max_map_count=262144
vm.max_map_count = 262144
exit
```
then
```shell
docker-compose up
```

## Troubleshooting

* [Elasticsearch: Max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]](https://stackoverflow.com/questions/51445846/elasticsearch-max-virtual-memory-areas-vm-max-map-count-65530-is-too-low-inc)
* [ECK elasticsearch pod not starting on AKS : max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]](https://discuss.elastic.co/t/eck-elasticsearch-pod-not-starting-on-aks-max-virtual-memory-areas-vm-max-map-count-65530-is-too-low-increase-to-at-least-262144/305788/3)