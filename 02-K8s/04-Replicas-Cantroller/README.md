```
 2005  mkdir 04-Replicas-Cantroller
 2006  ls
 2007  cd 04-Replicas-Cantroller/
 2008  ls
 2009  vim helloworld-cantroller.yaml
 2010  ls
 2011  kubectl apply -f helloworld-cantroller.yaml
 2012  kubectl  get nodes
 2013  kubectl  get pods
 2014  kubectl  get rc
 2015  kubectl  describe  rc
 2016  kubectl  get rc
 2017  kubectl scale --replicas=1 rc helloworld-cantroller
 2018  kubectl scale --replicas=1 rc helloworld-controller
 2019  kubectl  get pods
 2020  kubectl  describe  rc
 2021  kubectl  get pods -o wide --show-labels
 2022  ls
 2023  kubectl scale --replicas=5 rc helloworld-controller
 2024  kubectl get pods
 2025  kubectl  delete pod helloworld-controller-br8t2 helloworld-controller-snjbw helloworld-controller-x26xh
 2026  ls
 2027  kubectl delete -f helloworld-cantroller.yaml
 2028  kubectl  delete pod/hello-k8s pod/mypythonwebapp
```
