
# Use helm deploy release into kubernetes

## Getting Started
- Install **helm** version latest.
- File **config** of kubernetest in **~/.kube** folder.

## Deploy release to k8s
```
helm upgrade --install --config --debug --kubeconfig ~/.kube/config --create-namespace --namespace sonarqube sonarqube sonarqube/
```

## Check release
```
helm list -n sonarqube
```

## Uninstall release
```
helm uninstall sonarqube -n sonarqube
```
