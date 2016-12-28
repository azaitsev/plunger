# Plunger for ElasticSearch
## Elasticsearch force assign unassigned shards
No RED elasticsearch cluster anymore!

This simple script allocate unassigned shards to ES data nodes.

Usage:

`python plunger.py --host es.example.com --assign_to es-data1.example.com es-data2.example.com`

You can specify one ore multiple data nodes.
If you specified several nodes then destination node will be selected randomply for each shard.

Avalable params:

```
--host 
Your ES master name or IP

--port
ES master port

--assign_to
Names of ES data nodes (space separated)
```

Do not forget to install requirements.
