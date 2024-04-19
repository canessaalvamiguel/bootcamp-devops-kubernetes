# clusterIP
El service type clusterIP crea un servicio interno que solo es accesible desde dentro del cluster.
Permite acceder a los pods a través de un nombre de servicio.
El nombre del servicio sigue la estrucutra de nombre del servicio.nombre del namespace.svc.cluster.local
En este ejemplo seria backend-service.default.svc.cluster.local

```bash
KUBECTL apply -f cluster.yml
kubectl get pods
kubectl get services
kubectl exec -it pods/frontend -- bash
apt-get update && apt-get install curl -y
curl http://backend-service.default.svc.cluster.local
exit
kubectl delete -f cluster.yml
```