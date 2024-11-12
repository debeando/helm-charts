# DeBeAndo Agent for MySQL

Database monitoring tool designed for small environments, adapted for Kubernetes and send metrics to InfluxDB.

### Installing the Chart

To install the chart with the release name `agent-mysql`:

```bash
helm repo add debeando https://debeando.github.io/helm-charts
helm install agent-com-env-mysql-stack-node01 \
	--namespace debeando \
	--create-namespace \
	--set debug=true \
	--set interval=10 \
	--set influxdb_host=com-env-influxdb-observability-node01.aws.com \
	--set influxdb_token="abc123cde456==" \
	--set mysql_host=com-env-mysql-stack-node01.aws.com \
	--set mysql_user=monitor \
	--set mysql_password=passmon \
	--set server=com-env-mysql-stack-node01 \
	debeando/agent-mysql
```

The command deploys `agent-mysql` on the Kubernetes cluster. You can change the name to one more appropriate.

For more details about environment variables to set, please visit the [repository project](https://github.com/debeando/agent-mysql/tree/main).

### Uninstalling the Chart

To uninstall `agent-mysql` deployment:

```bash
helm uninstall agent-mysql
```

This command takes a release name and uninstalls the release.

It removes all of the resources associated with the last release of the chart as well as the release history.
