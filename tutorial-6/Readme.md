# Running the next commands:
```bash
kubectl get pods
kubectl get secrets
kubectl apply -f Pod-with-secret.yml
kubectl get pods
kubectl get secrets
kubectl describe secret my-secret
kubectl exec -it pods/pod-secret -- bash
echo $USERNAME
```