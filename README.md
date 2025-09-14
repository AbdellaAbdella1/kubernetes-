<img width="535" height="94" alt="image" src="https://github.com/user-attachments/assets/80acb835-5c2c-42b6-be85-ce95dc7c6b09" />



# Kubernetes Configuration Files

This repository contains Kubernetes YAML configuration files for deploying applications with Ingress, Secrets, and Pods.

## 📁 Files Included

- `ingress-only.yaml` - Kubernetes Ingress configuration
- `secret-only.yaml` - Kubernetes Secret configuration  
- `pod-only.yaml` - Kubernetes Pod configuration
- `ingress.yaml` - Additional Ingress configuration

## 🏗️ Kubernetes Architecture Overview
<img width="1606" height="838" alt="image" src="https://github.com/user-attachments/assets/7b9e3801-e31d-40c0-9f8e-2c105edc9aca" />

## Commands Successfully Used:
# Apply the Pod =
kubectl apply -f pod-only.yaml

# Cluster Information
kubectl cluster-info     
kubectl version           
kubectl config view   

# Working with Pods
kubectl get pods                
kubectl get pods -n kube-system  
kubectl describe pod <pod-name> 
kubectl logs <pod-name>          
kubectl exec -it <pod-name> -- bash   # open a shell inside pod

# Get Resources
kubectl get pods             
kubectl get services         
kubectl get deployments       
kubectl get ingress          
kubectl get secrets           
kubectl get nodes             
kubectl get all      

# Detailed Information

kubectl describe pod <pod-name>         
kubectl describe service <service-name> 
kubectl describe ingress <ingress-name>

# Create/Apply Resources

kubectl apply -f file.yaml             
kubectl create -f file.yaml            
kubectl create secret generic my-secret --from-literal=key=value
