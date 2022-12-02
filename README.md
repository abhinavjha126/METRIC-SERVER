# METRIC-SERVER
```bash
Added in deployment.yaml
nodeSelector: # configure the nodeSelector here to directly schedule pods to specific nodes
  node: cloudcore
hostNetwork: true
podAntiAffinity:
  requiredDuringSchedulingIgnoredDuringExecution:
    - labelSelector:
        matchExpressions:
          - key: kubeedge
            operator: In
            values:
              - cloudcore
      topologyKey: kubernetes.io/hostname
```  
```bash
VERSION - v0.6.1
wget https://github.com/kubernetes-sigs/metrics-server/releases/download/v0.6.1/components.yaml -O deploy.yaml
Deployment Image - k8s.gcr.io/metrics-server/metrics-server:v0.6.1
```
Used in kubeedge
```bash
kubectl top node
```
