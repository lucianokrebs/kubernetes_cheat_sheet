## Kubernetes cheat sheet

wip

### minikube basic commands

```shell
minikube status # check minikube status
minikube version # get minikube version 
minikube start # start a local cluster
```

### kubeclt basic commands

```shell
kubectl version 
kubectl cluster-info

kubectl get nodes
kubectl get pods
kubectl get pods -o go-template --template '{{range .items}}{{.metadata.name}}{{"\n"}}{{end}}'
kubectl describe pods

kubectl create deployment $DEPLOYMENT_NAME --image=gcr.io/google-samples/kubernetes-bootcamp:v1
kubectl logs -f $POD_NAME
kubectl exec -ti $POD_NAME -- bash
```
