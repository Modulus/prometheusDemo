# Namespace

kubectl create namespace monitoring

# Configuration

kubectl apply -f config.yml

# Deploy the server

kubectl apply -f deployment.yml

# Port forward
kubectl get pods -n monitoring
kubectl port-forward -n monitoring prometheus-monotoring-3123213123-xsdjk 8080:9090

# Service
kubectl apply -n monitoring -f service.yml