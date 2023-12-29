#### To list all K8s resources
```bash
kubectl api-resources
```

#### To get pods in namespace 
```agsl
kubectl get <resource type> <resource name: optional if you want all of them> --namespace <name>
```
Exemple:
```agsl
kubectl get pods draining-node-test-pod -o wide
```
* Use -o wide : to get more details
* Use -o yaml/json: to change output type
#### To describe a resource
```agsl
 kubectl describe  <type of resource> <name of resource> 
```
> kubectl describe  pods draining-node-test-pod

#### To exec command inside pod container 
```agsl
kubectl exec <name of pod> -c <name of container> -- <command to execute>
```
>kubectl exec  draining-node-test-pod -c nginx -- ls /etc/nginx/



