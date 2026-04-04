# Kubernetes AutoScaling
---
## Types of AutoScaling in Kubernetes

### Horizontal Pod Autoscaler (HPA)
 - **Purpose:** Adjusts the number of Pod replicas in a deployment based on CPU, memory, or custom metrics.
 - **Use Case:** Scaling out/in to handle variable workloads.
### Vertical Pod Autoscaler (VPA)
 - **Purpose:** Adjusts the resource requests and limits (CPU/memory) of containers in a Pod.
 - **Use Case:** Ensures optimal resource utilization for Pods.
### Cluster Autoscaler
 - **Purpose:** Adjusts the number of nodes in a cluster based on pending Pods that cannot be scheduled.
 - **Use Case:** Dynamically increases or decreases cluster size.
