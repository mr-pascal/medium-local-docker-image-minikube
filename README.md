# medium-local-docker-image-minikube

```sh

### Build container
docker build -t pz/demo .

### Run container
docker run -it --rm -p 8080:8080 pz/demo

## ---

### Load local Docker image into Minikube
minikube image load pz/demo

### Build container directly in minikube
minikube image build -t pz/demo .

### Check Deployment logs
kubectl logs deployment.apps/myapp

### Port forward port to Deployment
kubectl port-forward deployment/myapp 8080:8080

```