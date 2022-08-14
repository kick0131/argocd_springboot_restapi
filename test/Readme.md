# Manifest file for kubernetes
Google Cloud のArtifact RegistryからPodを作成するサンプル

!(description)[https://github.com/kick0131/argocd_springboot_restapi/raw/images/scope.png]
赤い部分がスコープ

| file | description |
| -- | -- |
|deployment.yaml | springboot application deployment image |
|service.yaml | LoadBalancer service |


```bash
# deploy command
kubectl create -f deployment.yaml
kubectl create -f service.yaml
```

