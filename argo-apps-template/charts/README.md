# charts/

Empty on purpose. Fill it from the StrategyOne package of the version **running** on your
cluster (RUNBOOK.md §4a). Never hand-edit the charts.

| Folder | From the package | Only if |
| --- | --- | --- |
| `mstr-operator/` | `mstr-operator.tgz` | always |
| `redis-cluster/` | `third-party/redis-cluster.tgz` | managed Redis is installed |
| `elasticsearch/` | `third-party/elasticsearch.tgz` | managed Elasticsearch is installed |
| `cloudnative-pg/` | `third-party/cnpg-operator.tgz` | CloudNativePG is installed |
| `keda/` | `third-party/keda.tgz` | KEDA is installed |
| `kube-prometheus-stack/` | `third-party/kube-prometheus-stack.tgz` | Prometheus is installed |
