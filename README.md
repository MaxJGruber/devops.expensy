# Instructions

1. Create EKS cluster

```
az aks create --resource-group rg-expensy-aks --name aks-expensy --node-count 1 --node-vm-size Standard_D2s_v3 --enable-managed-identity --generate-ssh-keys --location westeurope
```

2. Provision cluster using Kubernetes

```
./apply_all.sh
```
