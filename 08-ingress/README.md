enable ingress controller | minikube addons enable ingress
get ingress | kubectl get pods -n ingress-nginx
create deployment | create deployment web --image=gcr.io/google-samples/hello-app:1.0
expose deployent | kubectl expose deployment web --type=NodePort --port=8080
get minikube service url | minikube service web --url
verify that url working | curl http://192.168.49.2:31973 
create ingress file 
kubectl apply -f ingress.yml

kubectl get ingress

add entry /etc/hosts | 172.17.0.15 hello-world.info


check working status | curl hello-world.info
