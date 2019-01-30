
### 解决 gcr.io 问题
```
docker pull registry.cn-shenzhen.aliyuncs.com/shuhui/metrics-server:v0.3.1
docker tag registry.cn-shenzhen.aliyuncs.com/shuhui/metrics-server:v0.3.1 k8s.gcr.io/metrics-server-amd64:v0.3.1
docker rmi registry.cn-shenzhen.aliyuncs.com/shuhui/metrics-server:v0.3.1
```

## 部署
```
git clone https://github.com/kubernetes-incubator/metrics-server.git
cd metrics-server 
k create -f  deploy/1.8+/
```
