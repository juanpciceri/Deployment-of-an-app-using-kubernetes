# Deployment-of-an-app-using-kubernetes
This repository shows how to deploy an nginx app using kubernetes. The deployed app has got 3 replicas.

On the CLI you must execute the following commands to put your application up and running.

$  kubectl create -f webserver.yaml

To verify your deployment, you could use the following commands.

$  kubectl get replicasets
NAME                  DESIRED   CURRENT   READY     AGE
webserver-b477df957   3         3         3         45s

$ kubectl get pods

NAME                        READY     STATUS    RESTARTS   AGE
webserver-b477df957-7lnw6   1/1       Running   0          2m
webserver-b477df957-j69q2   1/1       Running   0          2m
webserver-b477df957-xvdkf   1/1       Running   0          2m
