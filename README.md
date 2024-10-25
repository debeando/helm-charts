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

### Update repo

Update gets the latest information about charts from the respective chart repositories. Information is cached locally, where it is used by commands like 'helm search repo debeando'.

```bash
helm repo update debeando
```

### Remove repo

Remove chart repository:

```bash
helm repo remove debeando
```
