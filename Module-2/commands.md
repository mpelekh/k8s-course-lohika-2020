# Commands

## Step 1: Configure Docker

```bash
gcloud auth configure-docker
```

## Step 2: Build an Image

```bash
docker build -t gcr.io/utopian-goods-272809/python-app:0.1 .
docker build -t gcr.io/[GCloud Project ID]/[image]:[tag] .
```

## Step 3: Authenticate to Container Registry

```bash
gcloud auth print-access-token | docker login -u oauth2accesstoken --password-stdin https://gcr.io
>>> Login Succeeded
```

## Step 4: Push an Image

```bash
docker push gcr.io/utopian-goods-272809/python-app:0.1
```

## Useful commands

```bash
kubectl get|delete|edit [type] [name]
kubectl logs -f [pod name]
kubectl describe [pod name]
kubectl rollout status deployment [deployment name]
kubectl exec -it [pod name] -- /bin/bash
kubectl port-forward [type]/[name] [proxy port]:[resource port]
```
