

To deploy the app:

```shell
minikube tunnel
k apply -f . 
```

To access to argocd dashboard at https://localhost:8081/:

```shell
k port-forward svc/argocd-server -n argocd 8081:443

# get admin's password
argocd admin initial-password -n argocd
```

