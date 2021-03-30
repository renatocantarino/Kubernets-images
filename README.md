# Kubernets-images
Create pods, Service and LoadBalancer


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



