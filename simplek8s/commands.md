## Print status of all running pods
```
kubectl get pods
```

## Feed a config file to kubectl
- apply: Change current configuration of cluster
- -f: We want to specif a file that has the config changes
- <filanem>: Path to the file with the config
```
kubectl apply -f <filename>
```