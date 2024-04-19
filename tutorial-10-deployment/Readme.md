# Deployment

```bash
kubectl apply -f deployment.yml
kubectl get pods
kubectl get deployments
kubectl port-forward nginx-deployment-57f79d6686-2482w 8080:80
kubectl delete -f deployment.yml
```