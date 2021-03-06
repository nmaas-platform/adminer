# nmaas-adminer

GEANT NMaaS Adminer Helm chart for Kubernetes

![Version: 2.0.9](https://img.shields.io/badge/Version-2.0.9-informational?style=flat-square) ![AppVersion: 4.8.1](https://img.shields.io/badge/AppVersion-4.8.1-informational?style=flat-square)

## Quick Start

```bash
helm repo add nmaas-adminer https://nmaas-platform.github.io/adminer/
helm repo update
helm install nmaas-adminer nmaas-adminer/adminer
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"adminer"` |  |
| image.tag | string | `"4.8.1"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.class | string | `"nginx"` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0] | string | `"default.nmaas.local"` |  |
| ingress.tls.enabled | bool | `false` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"500m"` |  |
| resources.limits.memory | string | `"512Mi"` |  |
| resources.requests.cpu | string | `"150m"` |  |
| resources.requests.memory | string | `"128Mi"` |  |
| service.port | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
