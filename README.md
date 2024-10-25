# DeBeAndo Kubernetes Helm Charts

The code is provided as-is with no warranties.

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repo as follows:

```bash
helm repo add debeando https://debeando.github.io/helm-charts/
```

You can then run `helm search repo debeando` to see the charts.

### Installing the Chart

To install the chart with the release name `demo`:

```bash
helm install demo debeando/demo
```

The command deploys `demo` on the Kubernetes cluster in the default configuration.

### Update the Chart

Update gets the latest information about charts from the respective chart repositories. Information is cached locally, where it is used by commands like 'helm search repo debeando'.

```bash
helm repo update debeando
```

### Uninstalling the Chart

To uninstall `demo` deployment:

```bash
helm uninstall pmm
```

This command takes a release name and uninstalls the release.

It removes all of the resources associated with the last release of the chart as well as the release history.
