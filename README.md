# k8-tutorial-overview

### Kube tutorial

These tutorials look to cover the basics of Kubernetes so that you can perform the basic tasks in a Kubernetes cluster!

There are several exercises to help cover the points raised during this overview that help cover a the practical elements of the Kubernetes architecture. 

### So, what is Kubernetes

Kubernetes is a “container orchestration system”, or in their own words:

“***Kubernetes is a portable, extensible, open-source platform for managing containerised workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.***”

Originally designed and developed by, it is now maintained by the Cloud Native Computing Foundation. 

To understand more about the benefits of Kubernetes (K8), we can see how things have progressed over time (again, thanks to the wonderful K8 concept pages)

![container_evolution](container_evolution.svg "Container Evolution")


This new way of working provides significant benefits over a “bare metal”, or “traditional” approach, namely around the concept of loosely coupled software development practises.

### Doesn’t Docker do this already?

Yes, sort of. Docker has Docker Swarm which is also a “container orchestration system”, and given Docker is nearly always the containerisation technology of choice, why isn’t everyone using this?

![swarm-diagram](swarm-diagram.png "Swarm")
  
Well, this likely comes back to the principle identified above, loose coupling.

### K8 vs Swarm

Kubernetes entire architecture is incredibly modular, from how your nodes (servers) talk to one another, to the containerisation technology used, monitoring tools, the works! Swarm provides a lot of the functionality Kubernetes does, just not quite at the same scale, nor with anywhere near the same level of flexibility.

Given this scope for customisation, Kubernetes tends to find itself fitting more naturally into large, operation environments running complex software distributions, whilst Swarm for more ad-hoc, small scale deployments.

The major difference however between the two is K8’s scope for the automatic scaling of services running within the cluster; something that Swarm, manual intervention is required to achieve. Users in K8’s can use the CPU/Memory demands of a container to inform K8 to increase or decrease the number of running instances, or alternatively, the containers own custom metrics (from the application running inside) to inform that decision.

There are many other differences we could cover here, but overall, in a simple, controversy causing analogy: K8 is to an Enterprise Linux Server that Docker Swarm is to a Windows Server deployment. Both achieve a lot of the same functionality, but one is going to require you to do things exactly their way, and therefore, may not get used in the same type of scenarios the other would.

### K8 architecture

-> Nodes
-> Node Roles
-> Namespaces
-> Pods/Services/Deployments/Replica Sets…
-> Ingresses

Tutorial 1 & 2

### K8 Components

-> API Server
-> DNS
-> Kubelet

### K8 Commands

-> List of commands

Tutorial 3








