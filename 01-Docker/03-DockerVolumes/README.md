```  
767  ls
  768  docker ps -a 
  769  docker rm $(docker ps -aq)  
  770  docker ps -a 
  771  docker kill $(docker ps -qa) 
  772  docker rm $(docker ps -qa) 
  773  ls
  774  docker ps -a 
  775  docker volume ls 
  776  docker volume create my-vol 
  777  docker volume ls 
  778  docker volume inspect my-vol
  779  docker run -it --name volume-test-1 -v my-vol:/app ubuntu:16.04
  780  ls
  781  docker kill $(docker ps -qa) 
  782  docker rm $(docker ps -qa) 
  783  docker ps -a 
  784  docker volume ls 
  785  cd /var/lib/docker/volumes/
  786  ls
  787  cd my-vol/
  788  ls
  789  cd _data/
  790  ls
  791  cat hello.txt 
  792  cd ..
  793  ls
  794  cd ..
  795  cd 
  796  ls
  797  cd docker-kubernetes-ericsson-29-Nov-2021/01-Docker/03-DockerVolumes/
  798  ls
  799  docker run -it --name volume-test-1 -v my-vol:/app ubuntu:16.04
  800  docker run -itd --name volume-test-2 -v my-vol:/app ubuntu:16.04
  801  docker run -itd --name volume-test-3 -v my-vol:/app ubuntu:16.04
  802  docker run -itd --name volume-test-4 -v my-vol:/app:ro ubuntu:16.04
  803  docker ps 
  804  docker attach volume-test-1
  805  docker attach volume-test-2
  806  docker attach volume-test-3
  807  docker attach volume-test-4
  808  ls
  809  cd /var/lib/docker/volumes/my-vol/_data/
  810  ls
  811  cat hello.txt 
  812  hostname >> hello.txt 
  813  date >> hello.txt 
  814  pwd >> hello.txt 
  815  cd 
  816  docker attach volume-test-4
  817  docker run -itd --name volume-ondemand-1 -v /var/www/amit ubuntu:16.04
  818  docker inspect volume-ondemand-1
  819  docker attach volume-ondemand-1
  820  ls
  821  docker volume ls 
  822  cd /var/lib/docker/volumes/d0794183a4ebe30bb3330f76fee9c2345b9e1c4deed2b951c2a3793089920056/_data/
  823  ls
  824  cat hello.txt 
  825  cd 
  826  ls
  827  docker run -itd --name volume-ondemand-2 -v /var/www/amit -v /var/log/amit -v /etc/amit ubuntu:16.04
  828  docker volume ls 
  829  docker inspect volume-ondemand-2
  830  docker run -itd --name volume-ondemand-3 -v /var/www/amit -v /var/log/amit -v /etc/amit:ro ubuntu:16.04
  831  ls
  832  cd docker-kubernetes-ericsson-29-Nov-2021/
  833  ls
  834  pwd
  835  docker run -itd --name volume-maphostdir-1 -v /root/docker-kubernetes-ericsson-29-Nov-2021:/app ubuntu:16.04
  836  docker run -itd --name volume-maphostdir-2 -v /root/docker-kubernetes-ericsson-29-Nov-2021:/app:ro ubuntu:16.04
  837  docker ps 
  838  docker attach volume-maphostdir-1
  839  ls
  840  docker attach volume-maphostdir-2
  841  ls
  842  cd ..
  843  ls
  844  docker ps 
  845  docker kill $(docker ps -qa ) 
  846  docker rm $(docker ps -qa ) 
  847  docker ps -a 
  848  docker volume ls 
  849  docker volume ls -q
  850  docker volume rm $(docker volume ls -q) 
  851  ld
  852  ls
  853  docker volume sl 
  854  docker volume ls 
  855  s
  856  ls
  857  cd docker-kubernetes-ericsson-29-Nov-2021/
  858  ls
  859  cd 01-Docker/
  860  ls
  861  history >> 03-DockerVolumes/README.md
```
