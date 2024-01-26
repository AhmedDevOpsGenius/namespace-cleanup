# namespace-cleanup

#A Kubernetes CronJob script (namespace-cleanup) designed to run at a specified frequency, checking for namespaces older than 4 days, excluding specified ones, and forcefully deleting them. The script uses a service account (namespace-manager-service-account) and executes within a container using the docker.io/bitnami/kubectl:latest image.

**#commands to execute the cronjob:**

kubectl apply -f service-account.yml
kubectl apply -f clusterrole.yml
kubectl apply -f clusterrolebinding.yml
kubectl apply -f cronjob.yml




