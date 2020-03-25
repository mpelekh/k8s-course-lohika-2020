# Commands

# connect to k8s cluster

```bash
gcloud container clusters get-credentials k8s-course-lohika-2020 --zone europe-west1-b --project kubernetes-course-lohika-2020
```

## kubectl

```bash
kubectl get ns
kubectl get pods
kubectl config get-clusters
kubectl config get-contexts
```

# push to docker registry

```bash
docker-compose build
docker tag flask-app:latest us.gcr.io/kubernetes-course-lohika-2020/flask-app:1.0.0
docker push us.gcr.io/kubernetes-course-lohika-2020/flask-app:1.0.0  
# where:
# - us.gcr.io - zone
# - kubernetes-course-lohika-2020 - the name of project

# if you can't push container, try the follownig command
gcloud auth configure-docker # Yes
```