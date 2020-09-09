### Pré requisitos
- Instalação docker.
- Intalação Kubectl
- Instalação Minikube
  
```shell
# Aplicando configuração
kubectl apply -f configmap.yaml 
kubectl apply -f deployment.yaml 
kubectl apply -f service.yaml

# Acessando o serviço
minicube service nginx-service
```
  