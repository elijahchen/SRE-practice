# Create deployment
kubectl create deployment hello-python-k8 --image=your-username/your-repo-name:tag

# Create a service to expose the deployment
kubectl expose deployment hello-python-k8 --type=NodePort --port=80

# Get the service url
minikube service hello-python-k8 --url