# MHDDoS auto Helm charts

This is a Helm chart for Kubernetes

## Prerequisites

Make sure that you installed `helm` package on your local machine and you have connection to the Kubernetes cluster.

## Install a release

```bash
cd kubernetes/helm-charts/
helm upgrade --install \
    --create-namespace \
    --namespace=mhddos \
    -f values.yaml mhddos .
```

## Destroy a release

```bash
helm uninstall mhddos -n mhddos
```
