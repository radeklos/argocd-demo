# ArgoCD

Simple helm file with ArgoCD  

```
helm dependency build argocd
helm dep update argocd

helm install argo-cd argocd --namespace argocd --create-namespace
```