# Manifest file for kubernetes
Google Cloud のArtifact RegistryからPodを作成するサンプル

| file | description |
| -- | -- |
|deployment.yaml | springboot application deployment image |
|service.yaml | LoadBalancer service |


```bash
# deploy command
kubectl create -f deployment.yaml
kubectl create -f service.yaml
```

