# Kuberneties (K8S)
---




<img width="1536" height="1024" alt="Kubernetes architecture overview and components" src="https://github.com/user-attachments/assets/0e68cf54-4aff-4d56-8a86-712dc1bc569d" />

---
## Control Plane (Master Node)

The control plane manages the entire cluster.

| Component | Role |
|----------|------|
| API Server | Entry point for all cluster communication |
| Scheduler | Assigns pods to worker nodes |
| Controller Manager | Maintains desired cluster state |
| etcd | Key-value database storing cluster data |

---
## Worker Node

Worker nodes run the application containers.

| Component | Role |
|----------|------|
| Kubelet | Communicates with control plane |
| Container Runtime | Runs containers (Docker / containerd) |
| Kube Proxy | Handles networking and load balancing |
| Pods | Smallest deployable unit in Kubernetes |

---
**1. NameSpace**

**2. Replication Controller  -- (Old Version)**

**3. Replica Set  -- (New Version)**

**4. Deamonset**

**5. Deployments**
  - Rolling update
  - Rolling out

**6. Stateful Set  -- Use in database**
    
**7. Configmap And Secrets** 

**8. Persistent Volume(PV) And Persistent Volume Claim(PVC)**

**9. AutoScaling**

  - Horizontal Pod Autoscaler (HPA)
  - Vertical Pod Autoscaler (VPA)
  - Cluster Autoscaler

**10. HPA with Minikube**
