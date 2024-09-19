## Commands

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
> Ao atualizar um replica set, os pods só serão atualizados quando for deletado todos os pods do replica set antigo. Para resolver isso, utilizar o deployment.

## VS Code

- Install the Kubernetes extension by Microsoft

