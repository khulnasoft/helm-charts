![KhulnaSoft logo](https://avatars3.githubusercontent.com/u/43526139?s=200&v=4)
# KhulnaSoft Security Helm Charts

[![License][license-img]][license]

[license-img]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
[license]: https://github.com/khulnasoft/helm-charts/blob/master/LICENSE

KhulnaSoft Security Open Source Projects Helm Charts on a [Kubernetes](https://kubernetes.io) cluster using the
[Helm](https://helm.sh) package manager.

## Charts

- [Tunnel Operator](https://github.com/khulnasoft/tunnel-operator/tree/main/deploy/helm)
- [Starboard](https://github.com/khulnasoft/starboard/tree/main/deploy/helm)
- [Tunnel](https://github.com/khulnasoft/tunnel/tree/main/helm/tunnel)
- [Postee](https://github.com/khulnasoft/postee/tree/main/deploy/helm/postee)
- [harbor-scanner-tunnel](https://github.com/khulnasoft/harbor-scanner-tunnel/tree/main/helm/harbor-scanner-tunnel)

## Prerequisites

- Kubernetes 1.15+ with Beta APIs enabled
- PV provisioner support in the underlying infrastructure

#### Installing [Helm](https://helm.sh)

```
curl -L https://git.io/get_helm.sh | bash
helm init
```

## Installing KhulnaSoft Community Helm Repository

```
helm repo add khulnasoft https://khulnasoft.github.io/helm-charts/
helm repo update
```

## Installing the Chart

Search all the repositories available
```
helm search repo khulnasoft -l
```

Install specific helm chart
```
helm install starboard khulnasoft/starboard-operator
helm status starboard
```

## Uninstalling the Chart

To uninstall/delete the `starboard` deployment:

```
$ helm delete starboard
```
