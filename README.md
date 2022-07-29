# Introduction

1. Django website using Django, Python, Postgres and Docker-Compose
2. Utilized Helm to manage and update deployment of the website on the Kubernetes cluster

# Prerequisites

Install kubectl and helm

## Deploy the application to Kubernetes using helm chart

```
make helm-deploy
kubectl get pod
kubectl --namespace default port-forward django-tutorial-django-website-78578f9856-pfht9 8080:80 
elm delete django-tutorial 
```
