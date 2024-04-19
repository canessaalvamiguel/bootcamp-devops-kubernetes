# Commmands for the lesson:

## Pods with commands
```bash
kubectl run nginx --image nginx:latest --replicas 3
kubectl run nginx --image nginx:latest --namespace your-namespace
kubectl get pods nginx -o wide
```

## Pods using yml
```bash
kubectl apply -f Pod.yml
kubectl get pods
kubectl delete -f Pod.yml
kubectl port-forward pod/nginx 8080:80
kubectl exec -it pods/nginx -- bash
```

## Namespaces with commands
```bash
kubectl create ns test
kubectl get ns
```

## Namespaces with commands
```bash
kubectl get cm
```

## Testing configmap
```bash
kubectl apply -f Pod.yml
kubectl exec -it pods/my-test-app --namespace=example-namespace --container=nginx -- bash
echo $key1
```