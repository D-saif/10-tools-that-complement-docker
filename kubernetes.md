# General introduction
Kubernetes (also known as k8s) is an open-source container cluster manager. Used for automating deployment, scaling, and management of containerized applications.


# Some basic concepts
### Intro to Kubernetes clusters
Kubernetes clusters are comprised of one **master node** and a number of **worker nodes.** These nodes can either be physical computers or virtual machines, depending on the cluster.
 * **The master node or the Control plane**
	 * Scheduling and scaling applications
     * Maintaining a cluster’s state
     * Implementing updates
 * **Worker nodes**
	 * The components that run these applications

### What makes up a Kubernetes cluster?
 **Inside the master node:**
 * **API server:** Exposes a REST interface to all Kubernetes resources. Serves as the front end of the Kubernetes control plane.
 
* **Scheduler:** Places containers according to resource requirements and metrics. Makes note of Pods with no assigned node, and selects nodes for them to run on.
 
* **Controller manager:** Runs controller processes and reconciles the cluster’s actual state with its desired specifications. Manages controllers such as node controllers, endpoints controllers and replication controllers.

**Inside the worker nodes:**
* **Kubelet:** Ensures that containers are running in a Pod by interacting with the Docker engine , the default program for creating and managing containers. Takes a set of provided PodSpecs and ensures that their corresponding containers are fully operational.

* **Kube-proxy:** Manages network connectivity and maintains network rules across nodes. Implements the Kubernetes Service concept across every node in a given cluster.


![](https://miro.medium.com/max/800/1*HHRp0HENvfAu2hXT8Gto9g.png)

# Advantages
* Open source
* High availability
* Auto scaling
* More stability
* Minimize the coast
* Cheaper than other altenatives

# Disadvantages
* Overkill for small applciations
* Complex
* Hard migration
* Virtualization is bad when there is a high network or I/O traffic
* Steap learning curve due to the bunch of new technologies that K8s uses

# Useful links
[1](https://www.youtube.com/watch?v=PH-2FfFD2PU) 
[2](https://www.youtube.com/watch?v=PziYflu8cB8)
[3](https://www.youtube.com/watch?v=F3YB79-RIek)  from 17:55->29:45 
[4](https://devspace.cloud/blog/2019/10/31/advantages-and-disadvantages-of-kubernetes)
[5](https://www.quora.com/What-are-the-downsides-of-using-Kubernetes)

