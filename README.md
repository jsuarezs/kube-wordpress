# kube-wordpress
Author: Javier Suarez

Deploying Wordpress example in Kubernetes.

1. Create namespace
   
   kubectl create ns wordpress

2. Create BBDD secret

    PASSWORD=mysecretpassword

    NAMESPACE=wordpress

    ````kubectl -n $NAMESPACE create secret generic credentials --from-literal=MYSQL_ROOT_PASSWORD=$PASSWORD````

3. ````kubectl apply -f .````