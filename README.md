# k8

# To study kubernetes to present EXAM CKAD

# kubectl get pod name-pod -o yaml > pod-definition.yaml

# kubectl edit pod pod-name


# Pod
# kubectl get pods
# kubectl apply -f pod-definition.yml


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
 

