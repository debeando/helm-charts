# DeBeAndo Port Forward

Port forward over SSH, allow connect to remote server over SSH to local or private kubernetes cluster.

### Installing the Chart

To install the chart with the release name `port-forward`:

```bash
helm repo add debeando https://debeando.github.io/helm-charts
helm install port-forward-com-env-mysql-stack-node01 \
	--namespace debeando \
	--create-namespace \
	--set debug=true \
	--set ssh_host="<ssh_host>" \
	--set ssh_key="`cat /Users/<username>/.ssh/<private>.pem | base64`" \
	--set remote_host="<mysql_host>" \
	debeando/port-forward
```

The command deploys `port-forward` on the Kubernetes cluster. You can change the name to one more appropriate.

For more details about environment variables to set, please visit the [repository project](https://github.com/debeando/port-forward/tree/main).

### Uninstalling the Chart

To uninstall `port-forward` deployment:

```bash
helm uninstall port-forward
```

This command takes a release name and uninstalls the release.

It removes all of the resources associated with the last release of the chart as well as the release history.
