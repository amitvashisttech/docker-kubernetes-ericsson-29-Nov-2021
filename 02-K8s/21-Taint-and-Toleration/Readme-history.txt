```
 2270  cd 21-Taint-and-Toleration/
 2271  ls
 2272  cat 01-helloworld.yaml
 2273  kubectl  apply -f 01-helloworld.yaml
 2274  kubectl describe nodes dworker2 | grep -i taint
 2275  kubectl taint node dworker2 app=myapp:NoSchedule
 2276  kubectl describe nodes dworker2 | grep -i taint
 2277  kubectl  scale --replicas=10 deploy helloworld-deployment
 2278  kubectl  scale --replicas=1 deploy helloworld-deployment
 2279  kubectl  scale --replicas=0 deploy helloworld-deployment
 2280  kubectl  scale --replicas=10 deploy helloworld-deployment
 2281  kubectl  scale --replicas=3 deploy helloworld-deployment
 2282  kubectl describe nodes | grep -i taint
 2283  ls
 2284  cat  02-helloworld-toleration.yaml
 2285  kubectl  apply -f 02-helloworld-toleration.yaml
 2286  kubectl  scale --replicas=10 deploy toleration-deployment
 2287  kubectl  scale --replicas=1 deploy toleration-deployment
 2288  ls
 2289  cat 03-helloworld-toleration-2.yaml
 2290  ls
 2291  cd ..
 2292  ls
 2293  kubectl  delete -f 21-Taint-and-Toleration/
 2294  ls
 2295  cd -
 2296  ls
 2297  cat 03-helloworld-toleration-2.yaml
 2298  kubectl taint node dworker1 example=amitvashist:NoSchedule
 2299  kubectl describe nodes | grep -i taint
 2300  ls
 2301  kubectl  apply -f 01-helloworld.yaml
 2302  kubectl  apply -f 02-helloworld-toleration.yaml
 2303  kubectl  delete  -f 01-helloworld.yaml
 2304  kubectl  scale --replicas=10 deploy toleration-deployment
 2305  cat 02-helloworld-toleration.yaml
 2306  ls
 2307  cat 03-helloworld-toleration-2.yaml
 2308  kubectl  apply -f 03-helloworld-toleration-2.yaml
 2309  kubectl  scale --replicas=10 deploy toleration-2-deployment
 2310  kubectl  delete -f 02-helloworld-toleration.yaml
 2311  kubectl  scale --replicas=1 deploy toleration-2-deployment
 2312  kubectl  scale --replicas=5 deploy toleration-2-deployment
 2313  kubectl  scale --replicas=10 deploy toleration-2-deployment
 2314  ls
 2315  cat 04-helloworld-toleration-3.yaml
 2316  kubectl taint node dworker2 example2=example2-key:NoExecute
 2317  kubectl  delete -f 03-helloworld-toleration-2.yaml
 2318  ls
 2319  kubectl  apply -f 04-helloworld-toleration-3.yaml
 2320  ls
 2321  cat 05-helloworld-ds.yaml
 2322  kubectl  apply -f 05-helloworld-ds.yaml
 2323  kubectl describe nodes | grep -i taint
 2324  kubectl taint node dworker2 app-
 2325  kubectl taint node dworker1 example-
 2326  kubectl describe nodes | grep -i taint
 2327  kubectl taint node dworker1 example2-
 2328  kubectl taint node dworker2 example2-
 2329  cat 05-helloworld-ds.yaml

 1076  kubectl  delete -f 18-Taint-and-Toleration/

```
