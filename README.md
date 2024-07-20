# PROJECT-21
## **Orchestrating containers across multiple Virtual Servers with Kubernetes. Part 1**


- In previous Project 20 you have started to work with containerization and have learned how to prepare and deploy a Docker container using Docker Compose.

- In this project, you will continue building upon your containerization skills, and begin to work on industry tools that fit for production deployment.

- Containers are the most lightweight and easily transferrable workloads, they start faster than VMs, consume less space and memory and, they perfectly fit to accommodate microservice architecture. It means that number of containers will be usually significantly higher that number of VMs and with number comes complexity of managing containers.

- To manage a fleet of containers you can use different software solutions, but the most widely used one is [Kubernetes](https://kubernetes.io/) (also referred as K8s). It was originally developed by Google and now being maintained by [Cloud Native Computing Foundation (CNCF)](https://en.wikipedia.org/wiki/Cloud_Native_Computing_Foundation).

- Why has it become so popular? It is a powerful Swiss-army knife when it comes to managing multiple containers in production-grade solutions.

- For now we will not list down all the features and benefits of Kubernetes, you can watch [this overview video](https://www.youtube.com/watch?v=VnvRFRk_51k) to get to know more, but you certainly must have this tool in your DevOps arsenal and know when and how to use if for production-grade deployments.

- This project is the first of a series Kubernetes-related practice projects, so get ready to become a professional containers' fleet "pilot"*.

- *Kubernetes (κυβερνήτης, Greek for "helmsman" or "pilot" or "governor", and the etymological root of cybernetics)

![alt text](kubernetes-logo.PNG)


### Why migrate from Docker Compose to K8s

- In the previous project you successfully deployed your Docker containers using **Docker Compose**, it is a great tool that helps avoiding execution of multiple CLI commands by preparing a declarative configuration file. It is handy when you deploy one or a few containers, but in most cases, it does not fit for production deployments.

- Because of the many limitations that Docker Compose has, it is very important for us to consider migrating our solution to more an advanced technology. The most common alternatives to **Compose**, amongst a few others, are **Docker Swarm** and **Kubernetes**.

## What is wrong with Docker Compose?