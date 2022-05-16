# CreatePod
# kubectl run nginx --image=nginx


# GetMoreDetails
# kubectl get pod -o wide

# GetOnlyNameResource
# kubectl get pod -o name

# CreateAFileWithoutCreateResource
# kubectl run nginx --image=nginx --dry-run=client -o yaml > namefile.yml
# kubectl run nginx --image=nginx --dry-run=client -o yaml
# kubectl run nginx --image=nginx --dry-run=client -o json

# ListAllPodsInAllNamespaces
# kubectl get pods --all-namespaces

# Switch
# kubectl config set-context $(kubectl config current-context) --namespace=dev

# GetNameImagePod
# kubectl describe pod webapp | grep -i image

# Edit
# kubectl edit rs replicaset-name.yml

# CreateDeployment
# kubectl create deployment httpd-frontend --image=httpd:2.4-alpine
# kubectl scale deployment --replicas=3 httpd-frontend
# kubectl create deployment httpd-frontend --image=httpd:2.4-alpine --dry-run=client -o yaml > deployment-definition.yaml

# CountNamespaces
# kubectl get ns --no-headers | wc -l

# CreatePodWithLabels
# kubectl run redis --image=redis:alpine --labels="tier=db"

# ImperativeCommands
# kubectl expose pod redis --name redis-service --port=6379 --target-port=6379
# kubectl create deployment webapp --image=kodekloud/webapp-color --replicas=3
# kubectl run custom-nginx --image=nginx --port=8080
# kubectl deployment redis-deploy --image=redis --namespace=dev-ns --replicas=3
# kubectl run httpd --image=httpd:alpine --port:80 --expose