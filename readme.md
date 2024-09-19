## Commands

- kubectl proxy --port=<port>: Start a proxy to the Kubernetes API server
- kubectl get nodes: List all nodes
- kubectl config get-clusters: List all clusters
- kubectl config use-context <context>: Set the current-context
- kubectl get pods / po: List all pods
- kubectl get replicasets: List all replica sets
- kubectl port-forward <pod-name> <local-port>:<pod-port>: Forward a port from a pod to the local machine
- kubectl exec -it <pod-name> -- /bin/bash: Open a shell in a pod
- kubectl apply -f <file>: Apply a configuration file
- kubectl delete <pod-name>: Delete a pod
- kubectl get deployments: List all deployments
- kubectl describe deployment <deployment-name>: Describe a deployment
- kubectl rollout status deployment <deployment-name>: Check the status of a deployment
- kubectl rollout history deployment <deployment-name>: Check the history of a deployment
- kubectl rollout undo deployment <deployment-name>: Undo a last revision of a deployment
- kubectl rollout undo deployment <deployment-name> --to-revision=<revision>: Undo a specific revision of a deployment

> [!CAUTION]
> When updating a replica set, the pods will only be updated when all the pods from the old replica set are deleted. To resolve this, use the deployment.

## Services
- service != container
- Expose a pod to the outside world (or other pods)
- ClusterIP (default): Exposes the service on a cluster-internal IP
- NodePort: Exposes the service on each Node's IP at a static port
- LoadBalancer: Exposes the service externally using a cloud provider's load balancer

## VS Code

- Install the Kubernetes extension by Microsoft

