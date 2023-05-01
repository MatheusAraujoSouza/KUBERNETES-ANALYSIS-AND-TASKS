The command you provided is a YAML configuration file that creates a Pod in Kubernetes using the declarative approach. Here is a breakdown of each part of the configuration:

apiVersion: This field specifies the Kubernetes API version to use, which in this case is "v1".
kind: This field specifies the kind of object you want to create, which in this case is a Pod.
metadata: This section contains metadata about the Pod, such as its name.
name: This field specifies the name of the Pod, which in this case is "first-pod-of-declaratively-way".
spec: This section specifies the desired state of the Pod.
containers: This section specifies the container(s) to run inside the Pod.
name: This field specifies the name of the container, which in this case is "nginx-container".
image: This field specifies the Docker image to use for the container, which in this case is "nginx:latest".
When you apply this YAML configuration file using the kubectl apply command, Kubernetes will create a new Pod with the specified name and configuration. The Pod will contain a single container running the latest version of the Nginx web server.