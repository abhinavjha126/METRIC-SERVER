# METRIC-SERVER
```bash
Service port changed from 443 to 80 to make it internal
CURL NOW: curl -X GET https://metrics-server.kube-system:80/apis/metrics.k8s.io/v1beta1/pods --insecure
```
```bash
Total Branches - 1

v1.0 - mainly for kubeedge purpose
```  
```bash
VERSION - v0.6.1
wget https://github.com/kubernetes-sigs/metrics-server/releases/download/v0.6.1/components.yaml -O deploy.yaml
Deployment Image - k8s.gcr.io/metrics-server/metrics-server:v0.6.1 (same image as below)
Zeblok Image - hub.docker.zeblok.com/zeblok/metrics-server:v0.6.1 (same image as above)
```
Used in kubeedge
```bash
kubectl top node
```
