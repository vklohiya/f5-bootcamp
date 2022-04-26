# Pods

Let’s create our first pod.

kubectl run nginx --image=nginx --restart=Never


### Creating the pod using yaml file
kubectl create -f pod-example.yaml
kubectl get pods -o wide

curl <pod-ip>

### Creating the pod with environment variable
kubectl create -f pod-example-with-env.yaml

kubectl get pods -o wide

kubectl logs pod-env-example

Question: Why pod is getting crash?

### Pod with labels
kubectl create -f pod-label.yaml

kubectl get pods --selector=env=prod



