# k8s-multi-containers-app
- First of all we have to create our kubernetes secrets for the postgres password by executing the command < kubectl create secret generic pgpassword --from-literal PGPASSWORD=thedesiredpassword >

- After that apply our K8S files by executing the command "kubectl apply -f k8s" ( delete the "to get token.txt" file )
And then if you are using minikube you have to acess to the minikube ip ( you can get it by executing "minikube ip") otherwise if you're using kubernetes within docker desktop you just have to acess the http://localhost/ to display your application.

- AND FOR SURE : your multi-client , multi-worker and multi-server images should be pushed on your dockerhub repository as well. ( and you have to change their names on the k8S Deployments objects config files)
