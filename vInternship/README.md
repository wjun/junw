# vInternship 2021: Cloud Native Application Development
## 1. Introduction to Information Technology

- major reference course: https://online.stanford.edu/courses/soe-ycscs101-sp-computer-science-101
- [Computer architecture](images/computer.jpg)
- [Operating system components](images/monolithic_os_kernel.gif)
- sound file(wave format) introduction 采样频率，采样位数: https://www.cnblogs.com/ranson7zop/p/7657874.html
- compression in image, sound, video files: huffman coding: https://blog.csdn.net/FX677588/article/details/70767446 

## 2. Introduction to programming(Golang): https://gobyexample.com/
- It is encouraged you play and learn Golang when you have some time at: https://play.golang.org/
- major syntax: if, for, array, slice, map, struct, interface, method, pointer, goroutine, channel, file, network(http client/server)

## 3. Introduction to virtualization and cloud computing: https://cs4740-s21.martyhumphrey.info/
- https://www.netapp.com/blog/containers-vs-vms/
- Cloud computing is any type of resources sold and consumed through internet transparently to users. If the resources are machine/storage/network, the cloud is IaaS. If the resources are software like video/word, the cloud is SaaS.
- virtual machines on Windows or Linux: VMware Workstation player
- virtual machines on Mac: VMware Fusion
- virtual machines for enterprises: VMware vSphere(private cloud) and VMware cloud(public cloud)
## 4. Introduction to docker and docker image
The major work includes:
- create an account from https://docs.docker.com/docker-hub/
- add your applicaiton into a docker image through docker build https://docs.docker.com/engine/reference/builder/
- docker push your image to docker hub so others can consume it anywhere. http://c.biancheng.net/view/3143.html
- one example can be found from [dockerexample](dockerexample)
## 5. Introduction to kubernetes
### 5.1 Network programming basis
- client and server communicate with network packages under network protocol through network connections. A connection is distinguished by [source ip, source port, destination ip, destionation port].
- tcp/ip package format: https://www.cnblogs.com/wuyuan2011woaini/p/5778949.html
- port concept: https://www.jianshu.com/p/686ce760cc7a
### 5.2 k8s architecture
[k8s architecture](images/Kubernetes-architecture.png)
Solving two problems with containers mainly: 1. how to manange multiple replicas of an application so one replica is dead, others can still serve. 2. schedule containers to different machines(or called nodes) so no machine will run too many containers that it will result the running of applications slow.
### 5.3 k8s online self learning portal
- https://kubernetes.io/docs/tutorials/
- https://www.katacoda.com/courses/kubernetes/
## 6. Introduction to cloud native application development
- wrap your application as a container into a k8s deployment: https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/
- yaml format introduction: https://baike.baidu.com/item/YAML
- add a service to expose your application using LoadBalancer or NodePort.
- you need to add a docker hub username/password as a secret in order to pull images from docker io in k8s cluster: https://kubernetes.io/docs/tasks/configure-pod-container/pull-image-private-registry/#create-a-secret-by-providing-credentials-on-the-command-line
```
kubectl create secret docker-registry regcred --docker-server=docker.io --docker-username=your_docker_hub_username --docker-password=your_password
```
- one example can be found from [k8sexample](k8sexample) that wraps the helloserver image into a k8s service.
## 7. Online/Remote Work
- zoom to meet: https://www.zoom.com
- slack to chat: https://www.slack.com
- git to code/review in peers: https://github.com
- online docs, etc google docs, microsoft offices, confluence pages
- online whiteboards: https://micro.com
- emails

