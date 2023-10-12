# Kubernetes

<p>  
    <img src="https://upload.wikimedia.org/wikipedia/commons/6/67/Kubernetes_logo.svg" alt="Kubernetes Logo" height="260">
</p>

# Content
1. [Understanding Containers](#understandingcontainers)
2. [Kubernetes Basics](#kubernetesbasics)
3. [Services and Networking](#serviceandnetworking)
4. [Storage in Kubernetes](#storageinkubernetes)
5. [Configuration Management](#configurationmanagement)
6. [Helm](#helm)
7. [Application Observability](#obervability)
8. [Advanced Kubernetes Concepts](#advanceconcept)
9. [Kubernetes Security](#security)
10. [Multi-Cluster and Federation](#MultiClusterandFederation)
11. [CI/CD with Kubernetes](#cicdkubernetes)
12. [Kubernetes in the Cloud](#kubernetesinthecloud)
13. [Troubleshooting](#troubleshooting)
14. [Best Practices](#bestpratices)
15. [Kubernetes Community and Resources](#communityandresources)
16. [Hands-On Projects](#handsonproject)

# Understanding Containers


# Kubernetes Basics

-  Open Source Plateform for `managing containerized workloads`.
-  Kubernetes originates from Greek, meaning `helmsman or pilot`.
- Containers are a good way to bundle and run your applications
- Kubernetes provides you with a `framework to run distributed systems` resiliently. It `takes care of scaling and failover` for your application, `provides deployment patterns`, and more.
- It provides some generally applicable features common to `PaaS offerings`, such as `deployment`, `scaling`, `load balancing`, and lets users `integrate their logging, monitoring, and alerting solutions`.
- It eliminates the need for orchestration.
- Kubernetes comprises a set of independent, composable control processes that continuously drive the current state towards the provided desired state.

- <h3>Features</h3>

    1. `Service discovery and load balancing` - if traffic high kubenetes is able to load balance
    2. `Storage orchestration` - Allows mounting of storage system of choice
    3. `Automated rollouts and rollbacks`  - Can automate kubernetes to create new container 
    4. `Self healing` - Kubernetes restarts containers that fail.
    5. `Secrete and configuration mangement` - lets you store and manage sensitive information
    6. `Horizontal Scaling` - Scale your application up or down with simple command or UI

- <h3>Kubernetes Components</h3>

    - `Node`
        - Kubernetes cluster consist of set of nodes. Nodes are set of worker machines.
        - Components
            1. `kublet` - agent that runs on each node in the cluster. Make sures containers are runnning in Pod.
            2. `kube-proxy` - a network proxy that runs on each node in your cluster.
            3. `container runtime` - It is responsible for managing the execution and lifecycle of containers within the Kubernetes environment.
            4. `addons` - Addons use Kubernetes resources (DaemonSet, Deployment, etc) to implement cluster features.
            5. `DNS` - Cluster DNS is a DNS server.
            6. Web UI Dashboard - web-based UI for Kubernetes clusters.
            7. `Container Resource Monitoring` - records generic time-series metrics
            8. `Cluster-level Logging `- is responsible for saving container logs to a central log store with search/browsing interface.
            9. `Network Pluggins` - are responsible for allocating IP addresses to pods and enabling them to communicate with each other within the cluster.

    - `Pod`
        - Component of the application workload.

    - `Control Plane`
        - manages the worker nodes and the Pods in the cluster
        - Control plane's components make global decisions about the cluster.
        - Control plane components can be run on any machine in the cluster.
        - Components
            1. `kubi-apiserver` - exposes Kubernetes API
            2. `etcd` - Key value store for storing cluster data
            3. `kubi-scheduler` -  watches newly created pod which has no assigned node and selects them node.
            4. `kube-controller-manager` - runs controller process - like node controller, Service controller, Job controller, EndpointSlice controller
            5. `cloud-controller-manager` - lets you link your cluster into your cloud provider's API

- <h3> Install : Kubernetes Install</h3>
    
    1. [Ubuntu Install](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)
    2. [MacOS Install](https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/)
    3. [Windows Install](https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/)

- <h3> Minikube : Install Minikube </h3>

    1. [Minicube Install](https://minikube.sigs.k8s.io/docs/start/)

# Services and Networking

    Kubernetes Services: Learn how to expose your applications to the network and how to configure different types of services (e.g., ClusterIP, NodePort, LoadBalancer).

    Ingress Controllers: Understand how to manage and route external traffic to your services using Ingress controllers.

    Network Policies: Explore network policies to control and secure communication between pods.

# Storage in Kubernetes

    Persistent Volumes (PVs) and Persistent Volume Claims (PVCs): Learn how to manage storage in Kubernetes, including volume provisioning and mounting.

# Configuration Management

    ConfigMaps and Secrets: Discover how to manage configuration data and sensitive information securely.

# Helm

    Helm Package Manager: Learn how to use Helm for packaging and deploying applications to Kubernetes.

# Application Observability

    Logging and Monitoring: Explore tools like Prometheus and Grafana for monitoring and logging in Kubernetes clusters.

# Advanced Kubernetes Concepts

    StatefulSets: Understand how to manage stateful applications in Kubernetes.

    Custom Resource Definitions (CRDs): Learn how to define custom resources to extend Kubernetes functionality.

    Operators: Explore Kubernetes operators for automating complex, application-specific tasks.

# Kubernetes Security

    RBAC (Role-Based Access Control): Learn how to set up fine-grained access control in Kubernetes.

    Pod Security Policies: Understand how to implement security policies for pods.

# Multi-Cluster and Federation

    Multi-Cluster Management: Learn how to manage multiple Kubernetes clusters.

# CI/CD with Kubernetes

    CI/CD Pipelines: Integrate Kubernetes into your CI/CD pipelines using tools like Jenkins, GitLab CI/CD, or ArgoCD.

# Kubernetes in the Cloud

    Managed Kubernetes Services: Explore managed Kubernetes offerings from cloud providers like AWS EKS, Google GKE, and Azure AKS.

# Troubleshooting

    Debugging and Troubleshooting: Develop skills for diagnosing and resolving issues in Kubernetes clusters.

# Best Practices

    Kubernetes Best Practices: Learn best practices for optimizing performance, security, and scalability in Kubernetes.

# Kubernetes Community and Resources

    Kubernetes Documentation: Continuously refer to the official Kubernetes documentation for in-depth information.

    Kubernetes Community: Engage with the Kubernetes community through forums, mailing lists, and social media.

    Kubernetes Conferences and Meetups: Attend Kubernetes-related events and conferences to network and stay updated on the latest trends.

    Online Courses and Tutorials: Explore online courses and tutorials on platforms like Udemy, Coursera, and edX.

    Books: Consider reading books dedicated to Kubernetes, such as "Kubernetes Up & Running" and "The Kubernetes Book."

# Hands-On Projects