# Commands

## Useful commands
```bash
kubectl get pv|pvc|sc

# Creates a ConfigMap contains a data file.
kubectl create configmap [name] --from-file=[path to file]

# Creates a ConfigMap contains environment variables from file.
kubectl create configmap [name] --from-env-file=[path to file]

# Creates a Secret contains sensitive data from file.
kubectl create secret generic [name] --from-file=[path to file]

# Creates a Secret contains sensitive data like credentials or tokens.
kubectl create secret generic [name] /
					--from-literal=[key_1]=[value_1] /
					--from-literal=[key_2]=[value_2]
