# 国内Kubernetes初始化

## 要求

系统：CentOS 7 x86_64
节点:

```
10.211.55.21 k8s-master
10.211.55.22 k8s-worker1
10.211.55.23 k8s-worker2
```

## 安装

1. ssh-copy-id 到每台节点
2. `ansible-playbook -v -i hosts kube-dependencies.yml kube-master.yml kube-worker.yml`
