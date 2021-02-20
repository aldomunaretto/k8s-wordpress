# Wordpress in Kubernetes

## Installation

1. Create secret
```
kubectl -n wordpress create secret generic credentials --from-literal=MYSQL_ROOT_PASSWORD=password --dry-run=client -o yaml > mysql-secret.yaml
```