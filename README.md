# AzureDatabricks Formula1 Analysis

### Creating New Cluster Policy for analysis: 
```
{
  "spark_conf.spark.databricks.cluster.profile": {
    "type": "fixed",
    "value": "singleNode",
    "hidden": true
  },
  "node_type_id": {
    "type": "allowlist",
    "values": [
      "Standard_DS3_v2",
      "Standard_D3_v2",
      "Standard_DS12_v2",
      "Standard_D12_v2"
    ],
    "defaultValue": "Standard_DS3_v2"
  },
  "autotermination_minutes": {
    "type": "fixed",
    "value": 20
  },
  "spark_version": {
    "type": "fixed",
    "value": "auto:latest-lts",
    "hidden": true
  },
  "cluster_type": {
    "type": "fixed",
    "value": "all-purpose"
  }
}

```
