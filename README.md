# ArgoCD

Simple helm file with ArgoCD  

### Install ArgoCD to K8S
```bash
helm dependency build argocd
helm dep update argocd

helm install argo-cd argocd --namespace argocd --create-namespace
```

### Make dashboard accessible
```bash
kubectl port-forward service/argo-cd-argocd-server 8080:80 -n argocd
```