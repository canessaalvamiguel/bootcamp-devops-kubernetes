# Running the next commands:
```bash
kubectl apply -f Pod-with-config-map.yml
kubectl get pods
kubectl exec -it pods/nginx -- bash
echo $color
exit
kubectl delete -f Pod-with-config-map.yml
```