# k8

# alias k=kubectl

# To study kubernetes to present EXAM CKAD

# kubectl get pod name-pod -o yaml > pod-definition.yaml

# kubectl edit pod pod-name


# Pod
# kubectl get pods
# kubectl apply -f pod-definition.yml
# kubectl get pod name-pod -o yaml > pod-definition.yaml


# ReplicationController
# kubectl get replicationcontroller
# kubectl get rc
# kubectl create -f rc-definition.yml


# ReplicaSet
# kubectl get replicaset
# kubectl get rs
# kubectl apply -f rs-definition.yml
# kubectl replace -f rs-definition.yml
# kubectl scale --replicas=6 -f rs-definition.yml
# kubectl scale --replicas=6 replicaset rs-name
# kubectl delete replicaset rs-name


# Deployment
# kubectl apply -f deployment-definition.yml
# kubectl get deployment

# Namespace
# kubectl get pods --namespace=dev
# kubectl create -f namespace.yml
# kubectl get ns
# kubectl get namespaces


# ResourceQuota
# kubectl apply -f resourcequota.yml
# kubectl get resourcequota

# ConfigMap
# kubectl create configmap configmap-name --from-literal=<key>=<value>
# kubectl create configmap configmap-name --from-file=app_config.properties
# kubectl get configmaps
# kubcetl describe configmap name-configmap


# Secret 
# kubectl create secret generic secret-name --from-literal=<key>=<value>
# kubectl create secret generic secret-name --from-file=<path-to-file>
# kubectl get secrets
# kubectl describe secrets
# kubectl get secret app-secret -o yaml
# echo -n 'mysql' | base64
# echo -n 'value' | base64 --decode 


# SecurityContexts
# kubectl exec it name-pod -- bin/sh
# ps aux
# kubectl exec name-pod -- whoami

# ServiceAccounts
# kubectl create serviceaccount dashboard-sa
# kubectl get serviceaccount
# kubectl describe serviceaccount dashboard-sa
# kubectl describe secret dashboard-sa-token-kbbdm
# kubectl exec -it pod-name ls /var/run/secrets/kubernetes.io/serviceaccount
# kubectl exec -it pod-name ls /var/run/secrets/kubernetes.io/serviceaccount/token
# kubectl create token dashboard-sa

# Tains (Node) & Tolerations (Pods)
# kubectl taint nodes node-name key=value:taint-effect (NoSchedule | PreferNoSchedule | NoExecute)
# kubectl taint nodes node1 app=blue:NoSchedule
# kubectl taint nodes controlplane node-role.kubernetes.io/master:NoSchedule-

# Node Selector
# kubectl label nodes <name-node> <label-key>=<label-value>

# Node Affinity
# 