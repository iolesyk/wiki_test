<!-- TITLE: Docker -->
<!-- SUBTITLE: A quick summary of Docker -->

# Docker



[video](https://www.youtube.com/watch?v=iN3he0eVUyw&t=796s){.youtube}


-----



Technology

Docker can use different interfaces to access virtualization features of the Linux kernel.[25]
Docker is developed primarily for Linux, where it uses the resource isolation features of the Linux kernel such as cgroups and kernel namespaces, and a union-capable file system such as OverlayFS and others[26] to allow independent "containers" to run within a single Linux instance, avoiding the overhead of starting and maintaining virtual machines (VMs).[27] The Linux kernel's support for namespaces mostly[28] isolates an application's view of the operating environment, including process trees, network, user IDs and mounted file systems, while the kernel's cgroups provide resource limiting for memory and CPU.[29] Since version 0.9, Docker includes the libcontainer library as its own way to directly use virtualization facilities provided by the Linux kernel, in addition to using abstracted virtualization interfaces via libvirt, LXC and systemd-nspawn.[12][30][25]

Building on top of facilities provided by the Linux kernel (primarily cgroups and namespaces), a Docker container, unlike a virtual machine, does not require or include a separate operating system.[31] Instead, it relies on the kernel's functionality and uses resource isolation for CPU and memory,[29] and separate namespaces to isolate the application's view of the operating system. Docker accesses the Linux kernel's virtualization features either directly using the libcontainer library, which is available as of Docker 0.9, or indirectly via libvirt, LXC (Linux Containers) or systemd-nspawn.[25][13]

Components
The Docker software is a service consisting of three components:

Software: The Docker daemon, called dockerd, is a persistent process that manages Docker containers and handles container objects. The daemon listens for requests sent via the Docker Engine API.[32][33] The Docker client program, called docker, provides a command-line interface that allows users to interact with Docker daemons.[34][32]
Objects: Docker objects are various entities used to assemble an application in Docker. The main classes of Docker objects are images, containers, and services.[32]
A Docker container is a standardized, encapsulated environment that runs applications.[35] A container is managed using the Docker API or CLI.[32]
A Docker image is a read-only template used to build containers. Images are used to store and ship applications.[32]
A Docker service allows containers to be scaled across multiple Docker daemons. The result is known as a "swarm", a set of cooperating daemons that communicate through the Docker API.[32]
Registries: A Docker registry is a repository for Docker images. Docker clients connect to registries to download ("pull") images for use or upload ("push") images that they have built. Registries can be public or private. Two main public registries are Docker Hub and Docker Cloud. Docker Hub is the default registry where Docker looks for images.[36][32]
Tools
Docker Compose is a tool for defining and running multi-container Docker applications.[37] It uses YAML files to configure the application's services and performs the creation and start-up process of all the containers with a single command. The docker-compose CLI utility allows users to run commands on multiple containers at once, for example, building images, scaling containers, running containers that were stopped, and more.[38] Commands related to image manipulation, or user-interactive options, are not relevant in Docker Compose because they address one container.[39] The docker-compose.yml file is used to define an application's services and includes various configuration options. For example, the build option defines configuration options such as the Dockerfile path, the command option allows one to override default Docker commands, and more.[40] The first public version of Docker Compose (version 0.0.1) was released on December 21, 2013.[41] The first production-ready version (1.0) was made available on October 16, 2014.[42]
Docker Swarm provides native clustering functionality for Docker containers, which turns a group of Docker engines into a single virtual Docker engine.[43] In Docker 1.12 and higher, Swarm mode is integrated with Docker Engine.[44] The swarm CLI utility allows users to run Swarm containers, create discovery tokens, list nodes in the cluster, and more.[45] The docker node CLI utility allows users to run various commands to manage nodes in a swarm, for example, listing the nodes in a swarm, updating nodes, and removing nodes from the swarm.[46] Docker manages swarms using the Raft Consensus Algorithm. According to Raft, for an update to be performed, the majority of Swarm nodes need to agree on the update.[47][48]
Operation
Docker implements a high-level API to provide lightweight containers that run processes in isolation.[11]

According to a Linux.com article,

Docker is a tool that can package an application and its dependencies in a virtual container that can run on any Linux server. This helps enable flexibility and portability on where the application can run, whether on premises, public cloud, private cloud, bare metal, etc.[31]

Because Docker containers are lightweight, a single server or virtual machine can run several containers simultaneously. A 2016 analysis found that a typical Docker use case involves running five containers per host, but that many organizations run 10 or more.[49]

Using containers may simplify the creation of highly distributed systems by allowing multiple applications, worker tasks and other processes to run autonomously on a single physical machine or across multiple virtual machines. This allows the deployment of nodes to be performed as the resources become available or when more nodes are needed, allowing a platform as a service (PaaS)-style of deployment and scaling for systems such as Apache Cassandra, MongoDB and Riak.[50][51]

Integration
Docker can be integrated into various infrastructure tools, including Amazon Web Services,[52] Ansible,[53] CFEngine,[54] Chef,[55] Google Cloud Platform,[56] IBM Bluemix,[57] HPE Helion Stackato, Jelastic,[58] Jenkins,[59] Kubernetes,[60] Microsoft Azure,[61] OpenStack Nova,[62] OpenSVC,[63] Oracle Container Cloud Service,[64] Puppet,[65] ProGet,[66] Salt,[67] Vagrant,[68] and VMware vSphere Integrated Containers.[69][70]

The Cloud Foundry Diego project integrates Docker into the Cloud Foundry PaaS.[71]

Nanobox uses Docker (natively and with VirtualBox) containers as a core part of its software development platform.[72]

Red Hat's OpenShift PaaS integrates Docker with related projects (Kubernetes, Geard, Project Atomic and others) since v3 (June 2015).[73]

The Apprenda PaaS integrates Docker containers in version 6.0 of its product.[74]

Jelastic PaaS provides managed multi-tenant Docker containers with full compatibility to the native ecosystem.[75]

The Tsuru PaaS integrates Docker containers in its product in 2013, the first PaaS to use Docker in a production environment.[76]

For Windows
On October 15, 2014, Microsoft announced integration of the Docker engine into the next Windows Server release, and native support for the Docker client role in Windows.[77][78] On June 8, 2016, Microsoft announced that Docker now could be used natively on Windows 10 with Hyper-V Containers, to build, ship and run containers utilizing the Windows Server 2016 Technical Preview 5 Nano Server container OS image.[79]

Since then, a feature known as Windows Containers was made available for Windows 10 and Windows Server 2016. There are two types of Windows Containers: "Windows Server Containers" and "Hyper-V Isolation". The former has nothing to do with Docker. The latter, however, is a form of hardware virtualization (as opposed to OS-level virtualization) and uses Docker to deliver the guest OS image.[80] The guest OS image is a Windows Nano Server image, which is 652 MB in size and has the same limitations of Nano Server,[81] as well as a separate end-user license agreement.[82]



