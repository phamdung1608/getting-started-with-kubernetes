## Objective
- Kubernetes overview
- Know to step by step master K8s and ignore unnecessary parts when getting started with Kubernetes
- Use Kubernetes to make a real-world (WordPress) application scalable and auto scaling
## Prior knowledge:
- What is container, VM?
    - Basically, containers and VM are similar in their goals. They support to isolate an application into a container unit and run it, re-use it everywhere. Container and VM support simulating a computer with installed softwares, applications.
    - The main difference between container and VMs is in their architectural approach.
    - reference: https://medium.freecodecamp.org/a-beginner-friendly-introduction-to-containers-vms-and-docker-79a9e3e119b    
- What is a orchestration platform? 
    - List a few container orchestrators platform: Kubernetes, Docker Swarm, Mesospher,...
## Kubernetes Overview:
- Kubernetes: What and Why
- Kubernetes node architecture
- Kubernetes cluster
    - What is Kubernetes cluster?
        - 
    - List some kind of Kubernetes Cluster.
        - Google Kubernetes Engine.
    - Set up Kubernetes Cluster on local using minikube (Single node cluster)
    - Setup minikube: https://github.com/kubernetes/minikube        
        - Follow the guide to install minikube, I will also install kubectl in your CLI.
        - kubectl support to interact with Kubernetes cluster. You can work with multiple Kubernetes cluster and switch the current context (current kubernetes cluster)
- Pods.
    -  Introduction
    -  Example
- Deployment
    - Introduction
    - Example
    - Demo apply a Deployment API Object
- Service 
    -  Introduction
    -  Example
    -  Demo apply Service API object
-  Service Discovery - DNS
    -   Introduction
    -   Demo
-  Storage
    - On-disk files in a Container are ephemeral
    - When a Container crashes, kubelet will restart it, but the files will be lost
    - When running Containers together in a Pod it is often necessary to share files between those Containers
    - It will be solved by PersistentVolume, PersistenVolumeClaim
    - Kubernetes supports several types of Volumes:
        - awsElasticBlockStore
        - gcePersistentDisk
        - azureDisk      
        - persistentVolumeClaim
        - ...     
    - PersistentVolume, PersistentVolumeClaim provides an API for users and administrators that abstracts details of how storage is provided from how it is consumed
- Auto Scaling
- Network
    - ClusterIp, NodePort, LoadBalancer
- How K8s integrate with CI/CD pipeline
- After all, keep researching below topics:
    -   helm
    -   Google Kubernetes Engine
    -   etcd