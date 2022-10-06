kubectl get pod <pod-name> -o yaml > pod-definition.yaml

kubectl edit pod <pod-name>

kubectl replace -f replicaset-definition.yml

kubectl scale --replicas=6 -f replicaset-definition.yml

kubectl scale --replicas=6 replicaset myapp-replicaset

kubectl explain replicaset

kubectl edit rs name-rs 

kubectl get all

-o name Print only the resource name and nothing else.

kubectl get pods --all-namespaces = kubectl get pods -A

kubectl get ns --no-headers | wc -l 