# Kubernetes YAML Notes

## YAML in Kubernetes
Kubernetes uses YAML to define objects like Pods, Deployments, and Services. Every Kubernetes YAML file follows a structure with **four required fields**:

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-app-pod
  labels:
    app: my-app
spec:
  containers:
    - name: my-container
      image: nginx
```

### Breakdown of Required Fields:
- **`apiVersion`** – Defines the Kubernetes API version to use.
- **`kind`** – Specifies the type of Kubernetes object (e.g., Pod, Deployment, Service).
- **`metadata`** – Contains the name and optional labels for the object.
- **`spec`** – Defines the object's specifications, such as containers inside a Pod.

### Containers in a Pod:
- The `containers` field is a **list** because a Pod can have multiple containers.
- Each container is defined by:
  - **`name`** – The name of the container inside the Pod.
  - **`image`** – The Docker image to run.

### Creating a Pod:
Run the following command to create a Pod using a YAML file:
```sh
kubectl create -f pod-definition.yml
```

### Viewing Pods:
- List all Pods:
  ```sh
  kubectl get pods
  ```
- Get detailed information about a Pod:
  ```sh
  kubectl describe pod my-app-pod
  ```

---
For more Kubernetes YAML examples, refer to the [official Kubernetes documentation](https://kubernetes.io/docs/concepts/).
