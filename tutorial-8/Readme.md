# INIT CONTAINERS
Los init-containers se ejecutan antes que los containers principales.
Se pueden usar para realizar tareas de inicialización como la descarga de archivos, la instalación de dependencias, etc.

En este ejemplo se crea un archivo index.html en el directorio /var/www antes de que el contenedor principal se inicie.

El init-container se ejecuta primero y crea el archivo index.html en el directorio /var/www.

```bash
KUBECTL apply -f Pod-with-init-container.yml
kubectl get pods
kubectl exec -it pods/init-container -- bash
cd /var/www/
ls
```