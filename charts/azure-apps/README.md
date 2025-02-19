# azure-apps

![Version: 0.1.1](https://img.shields.io/badge/Version-0.1.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.1.1](https://img.shields.io/badge/AppVersion-0.1.1-informational?style=flat-square)

Argo CD app-of-apps config for Azure applications

**Homepage:** <https://github.com/adfinis-sygroup/helm-charts/tree/master/charts/azure-apps>

## Maintainers
This chart is maintained by [Adfinis](https://adfinis.com/?pk_campaign=github&pk_kwd=helm-charts).

## Source Code

* <https://github.com/adfinis-sygroup/helm-charts>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.adfinis.com | argoconfig | 0.7.4 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| azureKvCsiProvider | object | - | [secrets-store-csi-driver-provider-azure](https://github.com/Azure/secrets-store-csi-driver-provider-azure) ([examplpe](./examples/azure-kv-csi-provider.yaml)) |
| azureKvCsiProvider.chart | string | `secrets-store-csi-driver-provider-azure"` | Chart |
| azureKvCsiProvider.destination.namespace | string | `"infra-azure-kv-csi-provider"` | Namespace |
| azureKvCsiProvider.enabled | bool | `false` | Enable secrets-store-csi-driver-provider-azure |
| azureKvCsiProvider.repoURL | string | [repo](https://raw.githubusercontent.com/Azure/secrets-store-csi-driver-provider-azure/master/charts) | Repo URL |
| azureKvCsiProvider.targetRevision | string | `"0.2.*"` | [vault-csi-provider-azure Helm chart](https://github.com/Azure/secrets-store-csi-driver-provider-azure/tree/master/charts/csi-secrets-store-provider-azure) version |
| azureKvCsiProvider.values | object | [upstream values](https://github.com/Azure/secrets-store-csi-driver-provider-azure/blob/master/charts/csi-secrets-store-provider-azure/values.yaml) | Helm values |

## About this chart

Adfinis fights for a software world that is more open, where the quality is
better and where software must be accessible to everyone. This chart
is part of the action behind this commitment. Feel free to
[contact](https://adfinis.com/kontakt/?pk_campaign=github&pk_kwd=helm-charts)
us if you have any questions.

## License

This Helm chart is free software: you can redistribute it and/or modify it under the terms
of the GNU Affero General Public License as published by the Free Software Foundation,
version 3 of the License.

----------------------------------------------
Autogenerated from chart metadata using [helm-docs](https://github.com/norwoodj/helm-docs/)
