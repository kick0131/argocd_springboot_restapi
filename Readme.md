## usage kustomize

```base
# format check
kubectl kustomize base
kubectl kustomize overlays/dev

# exec orchestration
kubectl apply -k overlays/dev

# create and delete with namespace
kubectl create namespace dockerhub
kubectl apply -k overlays/dockerhub -n dockerhub
kubectl delete -k overlays/dockerhub -n dockerhub

```

## directory

| directory    | description                          |
|--|--|
| base         |  use google cloud service(GCS) image |
| overlays     |                                      |
|   /dev       |  change replica size                 |
|   /dockerhub |  use dockerhub image                 |

## Notes
See below for a description of the $patch(use [overlays/docerhub])  
https://github.com/kubernetes-sigs/kustomize/issues/306


