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