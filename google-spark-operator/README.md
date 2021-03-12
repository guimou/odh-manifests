# Google Spark operator

[Kubernetes Operator for Spark](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator) contains one component, the [spark operator](#spark-operator), that deploys [Apache Spark](https://spark.apache.org) clusters for large-scale data processing.

## Spark Operator

Deploys the Radanalytics [Kubernetes Operator for Spark](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator). This operator will watch for the following custom resources cluster-wide:

1. [SparkApplication](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator/blob/master/docs/user-guide.md#using-a-sparkapplication)
2. [ScheduledSparkApplication](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator/blob/master/docs/user-guide.md#running-spark-applications-on-a-schedule-using-a-scheduledsparkapplication)

### Parameters

Spark Operator does not provide any parameters.

#### Examples

```yaml
  - kustomizeConfig:
      repoRef:
        name: manifests
        path: google-spark-operator/operator
    name: google-spark-operator
```

### Overlays

Spark Operator does not provide any overlays.
