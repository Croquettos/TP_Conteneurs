Déboguer Deployment

kubectl get pods => lister pods
kubectl describe pod <POD_NAME> => Status et Event
kubectl get pod <POD_NAME> -o yaml => voir les valeurs
kubectl port-forward pod/POD_NAME HOST_PORT:POD_PORT
kubectl port-forward svc/SVC_NAME HOST_PORT:POD_PORT

./kind-with-registry.sh pour démarrer le registre
docker-compose build
docker-compose push
kubectl kubernetes-manifests/. pour déployer les tide pods
