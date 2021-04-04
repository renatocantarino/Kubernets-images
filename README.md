# Kubernets-images




![alt text](https://github.com/renatocantarino/Kubernets-images/blob/main/img/kube.png)




Create pods, Service, LoadBalancer and ConfigMaps


- Create a pod Nginx image : kubectl run nginx-pod --image=nginx:latest
- watch pod creating : kubectl get pods –watch
- describe a pod :  kubectl describe pod  PodName
- edit a pode Yaml: kubectl edit pod nginx-pod   -> abre o yaml do pod criado
- delete a pod :    kubectl delete pod nginx-pod
- get a pods : kubectl get pods

--------
- read a yaml file : kubectl apply -f pod-one.yaml
- delete a pod yaml based : kubectl delete -f pod-one.yaml


--------
- get services :  kubectl get service
- delete services : kubectl delete svc ServiceName
--------
Deployments

- kubectl apply -f nginx-deployment.yaml --record   : set a change cause action
- kubectl get deployments   : get all deployments
- kubectl rollout history deployment   : get all versions deployment containers
- kubectl annotate deployment nginx-deployment kubernetes.io/change-cause="versao latest"   : add a update description
- kubectl describe pod nginx-deployment-6645687878-c7b4p   : describe a specific pod by ID
- kubectl rollout undo deployment nginx-deployment --to-revision=1 : rollback to specific control version


