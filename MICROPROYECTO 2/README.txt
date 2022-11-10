1. poner los archivos yaml dentro del servidor en una ruta deseada.
2. una vez dentro de la ruta de se deberan correr los siguentes comandos.

-kubectl apply -f deployment.yaml #se corre la aplicacion de deteccion de imagenes.
-kubectl expose deployment kubermatic-dl-deployment  --type=LoadBalancer --port 80 --target-port 5000 # se expone la aplicacion
-kubectl apply -f myfile.yaml #se corre la aplicacion de conteo de gatos vs perros.

3. Validar pods y servicios

-kubectl get pods ## lista los pods.
-kubectl get services ## se listan los servicios con las direcciones IP .


NOTA: Es importante que antes de correr los comandos anteriormente dichos se debe de tener configurado y probado el cluster
kubernetes.