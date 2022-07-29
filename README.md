# django-website-tutorial
Project files for the Django Website Tutorial

1. Install kubectl and helm in your local


2. make helm-deploy  or  helm upgrade --install django-tutorial ./helm/django-website/ 

3. kubectl get pod

4. kubectl --namespace default port-forward $POD_NAME 8080:$CONTAINER_PORT (# check in deployment.yaml)
ex: kubectl --namespace default port-forward django-tutorial-django-website-78578f9856-pfht9 8080:80 


5. stop kubernetes pod, remove prior release, release create -> helm delete django-tutorial 
 