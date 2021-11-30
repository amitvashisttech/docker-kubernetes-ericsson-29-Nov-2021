``` 
1052  cd 03-KubeApi/
 1053  ls
 1054  kubectl get pods -n kube-system 
 1055  kubectl get pods -n kube-system | grep -i apiserver
 1056  vim README.md 
 1057  ls
 1058  kubectl cluster-info
 1059  kubectl version 
 1060  kubectl api-versions
 1061  kubectl api-resources
 1062  kubectl run mypythonwebapp --image=amitvashist7/mypywebapp:v3 --port=8081 --dry-run 
 1063  kubectl  get pods 
 1064  kubectl run mypythonwebapp --image=amitvashist7/mypywebapp:v3 --port=8081 --dry-run 
 1065  kubectl run mypythonwebapp --image=amitvashist7/mypywebapp:v3 --port=8081 --dry-run -o yaml
 1066  kubectl run mypythonwebapp --image=amitvashist7/mypywebapp:v3 --port=8081 --dry-run -o yaml > Pod.yaml
 1067  ls
 1068  kubectl get pods 
 1069  vim Pod.yaml 
 1070  kubectl apply -f Pod.yaml 
 1071  kubectl  get pods 
 1072  kubectl api-resources
 1073  ls
 1074  cp -rf Pod.yaml Job.yaml
 1075  vim Job.yaml 
 1076  kubectl apply -f Job.yaml 
 1077  vim Job.yaml 
 1078  kubectl api-resources
 1079  kubectl  get pods 
 1080  kubectl  get po
 1081  ls
 1082  kubectl proxy --address='172.31.0.100' --port=8080 --accept-hosts='.' --accept-paths='.' &
 1083  kubectl get pods 
 1084  kubectl describe pods mypythonwebapp
 1085  ls
 1086  kubectl get pods 
 1087  kubectl config get-clusters 
 1088  kubectl config view
 1089  ls
 1090  vim /etc/kubernetes/admin.conf 
 1091  cd 
 1092  ls
 1093  pwd
 1094  ls -a 
 1095  cd .config/
 1096  ls
 1097  cd ..
 1098  ls
 1099  cd .kube/
 1100  ls
 1101  vim config 
 1102  ls
 1103  cd ..
 1104  ls
 1105  cd docker-kubernetes-ericsson-29-Nov-2021/
 1106  ls
 1107  cd 02-K8s/
 1108  ls
 1109  cd 03-KubeApi/
 1110  ls
 1111  history > README.md 
```
