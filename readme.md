https://www.cnblogs.com/bakari/p/9577649.html


```https://kubernetes.io/docs/tasks/tools/install-kubectl/```

```sudo apt-get update && sudo apt-get install -y apt-transport-https```

```curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -```

```sudo touch /etc/apt/sources.list.d/kubernetes.list```

```echo "deb http://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee -a /etc/apt/sources.list.d/kubernetes.list```

```sudo apt-get update```

```sudo apt-get install -y kubectl```


https://kubernetes.io/docs/tasks/tools/install-minikube/
https://github.com/kubernetes/minikube/releases
https://github.com/kubernetes/minikube


https://docs.docker.com/install/linux/docker-ce/ubuntu/


```curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.28.2/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/```

```minikube start --vm-driver=none```

```minikube dashboard --url```

部署一个 APP

```kubectl run kubernetes-bootcamp --image=gcr.io/google-samples/kubernetes-bootcamp:v1 --port=8080```





