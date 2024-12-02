---
tags:
  - Room
  - CyberNotes
---
## Kubernetes Architecture 
![[Pasted image 20241112221608.png]]
Cluster > Nodes > Pod
### Kubernetes Control Plane
Kube-apiserver
Etcd : store containing cluster data 
Kube-scheduler : Monitor
Kube-controller-manager : Node controler
![[Pasted image 20241112222816.png]]
### Worker Node
Kubelet
Kube-proxy 
Container runtime
![[Pasted image 20241112223402.png]]
### Communication Between Components
![[Pasted image 20241112223442.png]]

## 