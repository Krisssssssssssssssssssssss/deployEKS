- Follow those steps for creating and connecting the cluster (assuming you already have an Azure account and CLI installed):
https://learn.microsoft.com/en-us/azure/aks/learn/quick-kubernetes-deploy-portal?tabs=azure-cli

- For the deployment please run the manifests in this project:
kubectl apply -f frontend.yaml
kubectl apply -f backend.yaml
kubectl apply -f db.yaml

- get the external IP of the frontend:
kubectl get services
- paste it in the browser, the NGNIX homepage should be displayed.

- delete all reasources with:
kubectl delete -f frontend.yaml
kubectl delete -f backend.yaml
kubectl delete -f db.yaml
