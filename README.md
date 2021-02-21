# Wordpress in Kubernetes

## Installation
1. Create namespace
```
kubectl create namespace wordpress
```

2. Create secret
```
kubectl -n wordpress create secret generic credentials --from-literal=MYSQL_ROOT_PASSWORD=password
```

```
para el network policy
kubectl -n wordpress label namespace wordpress app=wordpress
```

3. Create DNS Wildcard for your IP Address
`nip.io`