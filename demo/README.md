# Demo

Demo is an open source database monitoring tool.

### Installing the Chart

To install the chart with the release name `demo`:

```bash
helm repo add debeando https://debeando.github.io/helm-charts/
helm install demo debeando/demo
```

The command deploys `demo` on the Kubernetes cluster.

### Uninstalling the Chart

To uninstall `demo` deployment:

```bash
helm uninstall pmm
```

This command takes a release name and uninstalls the release.

It removes all of the resources associated with the last release of the chart as well as the release history.
