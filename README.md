# k8s-jenkins


按照个人环境修改pvc配置，ingress域名。
顺序启动
```
kubectl create -f jenkins-pvc.yaml
kubectl create -f jenkins-rbac.yaml
kubectl create -f jenkins-deployment.yaml
kubectl apply -f jenkins-ingress.yaml
```
jenkinsweb初始密码查看pod日志或在pod内查看：cat /opt/nfs/jenkins2/secret/initAdminPassword

插件安装选择推荐的插件即可。
