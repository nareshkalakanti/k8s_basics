## PODS
- Command to create a POD from YAML
    * kubectl create -f nginx.yaml 

- Command to view the created pod
  - kubectl get pods
  - kubectl get pods --show-labels
  - kubectl describe pod <pod-name>
- Command to delete PODS
  - kubectl delete pod <pod-name>
- Commands for replica set
  - kubectl get replicaset
  - kubectl get rs
- Commands for deployments
  - kubectl create -f nginx-deployment.yaml
  - kubectl get deployments
  - kubectl get replicaset
  - kubectl get pods
  - kubectl rollout status deployment/nginx-deployment
  - kubectl describe deployment nginx-deployment

### Deployments
#### Task : Release a newer version of the application - upgrade nginx to 1.16.1, change to 4 replicas

- kubectl edit deployment nginx-deployment
- kubectl get rs
- kubectl get pods
- kubectl rollout status deployment/nginx-deployment
- kubectl rollout history deployment/nginx-deployment
- OR
- kubectl replace -f nginx-deployment.yaml
- kubectl describe deployment nginx-deployment

### Services 
- ClusterIP

- NodePort
- kubectl create -f node-port-service.yaml
- kubectl describe pod nginx
- kubectl get svc
- kubectl describe svc my-service

### Namespaces 
- kubectl get namespaces
- kubectl get pods --namespace=default




       