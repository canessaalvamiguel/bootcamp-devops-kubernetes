# Running the next commands:

```bash
kubectl apply -f Pod-with-volume.yml 
kubectl get pods
kubectl exec pods/mypod --container=ubuntu1 -- touch /var/www/hola.txt

kubectl exec pods/mypod --container=ubuntu1 -- ls /var/www/
kubectl exec pods/mypod --container=ubuntu2 -- ls /root/test
```