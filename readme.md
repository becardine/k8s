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

> [!CAUTION]
> Ao atualizar um replica set, os pods só serão atualizados quando for deletado todos os pods do replica set antigo. Para resolver isso, utilizar o deployment.

## VS Code

- Install the Kubernetes extension by Microsoft

