
## About Pods: 

In Kubernetes, a pod is the smallest deployable unit that can be created, scheduled, and managed. A pod is a logical host for one or more containers. It represents a single instance of a process in a cluster, and it can contain one or more containers that share the same network namespace and the same storage volumes.

Pods are designed to be ephemeral and disposable. They can be easily created, destroyed, and replaced as needed. Pods are also used to provide a stable network and storage interface for their containers, and they allow containers to communicate with each other using inter-process communication (IPC) mechanisms like shared memory or Unix sockets.

Pods can be thought of as a wrapper around one or more containers that provides a common network and storage interface. They are often used to group containers that need to work together, such as a web server and a database, or to create a single logical unit of an application.

## some command to manipulate pods in prompt

- `kubectl get pods`: List all running pods in the current namespace
- `kubectl describe pod <pod-name>`: Show detailed information about a specific pod
- `kubectl logs <pod-name>`: Show the logs of a specific pod
- `kubectl exec <pod-name> <command>`: Run a command inside a specific pod
- `kubectl port-forward <pod-name> <local-port>:<pod-port>`: Forward a local port to a port inside the pod
- `kubectl delete pod <pod-name>`: Delete a specific pod