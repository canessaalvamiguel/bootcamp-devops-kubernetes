# Running the next command:

```bash
kubectl apply -f Pod-not-running.yml
kubectl get pods
```

The pods will fail with error `CrashLoopBackOff` due to this doesn't have a process running.
To fix we need to add this to the YML:
`tty: true`


and then run:

```bash
kubectl delete -f Pod-not-running.yml
kubectl apply -f Pod-not-running.yml
kubectl get pods
```
