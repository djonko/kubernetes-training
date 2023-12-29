#### Pods and Containers

Secret values are always in base64 in yaml files

- To convert value in base64
```agsl
echo -n 'admin' | base64
```

- To go in `it` mode inside container
```agsl
kubectl exec <pod name> -c <container name>  -it -- sh
```
