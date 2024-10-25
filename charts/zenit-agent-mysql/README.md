# Zenit Agent for MySQL

zenit-agent-mysql is an open source database monitoring tool.

### Installing the Chart

To install the chart with the release name `zenit-agent-mysql`:

```bash
helm repo add debeando https://debeando.github.io/helm-charts/
helm install zenit-agent-mysql debeando/zenit-agent-mysql
```

The command deploys `zenit-agent-mysql` on the Kubernetes cluster.

### Uninstalling the Chart

To uninstall `zenit-agent-mysql` deployment:

```bash
helm uninstall zenit-agent-mysql
```

This command takes a release name and uninstalls the release.

It removes all of the resources associated with the last release of the chart as well as the release history.
