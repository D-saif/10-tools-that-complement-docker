# Little introduction

- Traefik is a modern HTTP reverse proxy and load balancer that makes deploying microservices easy. Traefik integrates with your existing infrastructure components (Docker, Swarm mode, Kubernetes, Marathon, Consul, Etcd, Rancher, Amazon ECS, ...) and configures itself automatically and dynamically.
 
- A reverse proxy accepts a request from a client, forwards it to a server that can fulfill it, and returns the server's response to the client. A load balancer distributes incoming client requests among a group of servers, in each case returning the response from the selected server to the appropriate client.

![how reversy proxy works](https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/reverse-proxy-02-1.jpg)


## Pros of using Traefik
 
* Supports multiple load balancing algorithms
* Provides HTTPS to your microservices by leveraging Let's Encrypt (wildcard certificates support)
* its clean web UI and Ready-to-use dashboard
* Kubernetes integration
* Letsencrypt support
* Swarm integration
* Several backends
* Easy setup
* Exposes a Rest API
* Fast
* Provides metrics

