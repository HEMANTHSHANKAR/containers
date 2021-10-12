# CONTAINERS

## Containers

Containers are an abstraction at the app layer that packages code and dependencies together. Multiple containers can run on the same machine and share the OS kernel with other containers, each running as isolated processes in user space. Containers take up less space than VMs (container images are typically tens of MBs in size), can handle more applications and require fewer VMs and Operating systems.

Containers play a big role in the shifting IT landscape because enterprises are moving towards fast, agile delivery of software and solutions to get ahead of competitors.

Containers are here to stay. In the very near future, other use cases, like serverless on the edge, will emerge and further change how we think about the speed of getting information to and from digital devices. The only way to survive these changes is to adapt to them.

## Process

A process is basically a program in execution. The execution of a process must progress in a sequential fashion.

A process is defined as an entity which represents the basic unit of work to be implemented in the system.
To put it in simple terms, we write our computer programs in a text file and when we execute this program, it becomes a process which performs all the tasks mentioned in the program.

A computer program is a collection of instructions that performs a specific task when executed by a computer. When we compare a program with a process, we can conclude that a process is a dynamic instance of a computer program.
A part of a computer program that performs a well-defined task is known as an algorithm. A collection of computer programs, libraries and related data are referred to as a software.

When a program is loaded into the memory and it becomes a process, it can be divided into four sections ─ stack, heap, text and data. 

Below document explains PROGRAM, PROCESS, PROCESS LIFE CYCLE, PROCESS CONTROL BLOCK

[Processes.pdf](https://github.com/HEMANTHSHANKAR/containers/files/7323923/Operating.System.-.Processes.pdf)

## Namespace

Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources.

Namespaces have been part of the Linux kernel since about 2002, and over time more tooling and namespace types have been added. Real container support was added to the Linux kernel only in 2013, however. This is what made namespaces really useful and brought them to the masses.

### Types of Namespaces
1. USER NAMESPACE
2. PID NAMESPACE
3. NETWORK NAMESPACE
4. MOUNT NAMESPACE
5. INTERPROCESS COMMUNICATION (IPC) NAMESPACE
6. UNIX TIME-SHARING NAMESPACE

Namespaces are one of the technologies that containers are built on, used to enforce segregation of resources. We’ve shown how to create namespaces manually, but container runtimes like Docker, rkt, and podman make things easier by creating namespaces on your behalf. 

## cgroups

A control group (cgroup) is a Linux kernel feature that limits, accounts for, and isolates the resource usage (CPU, memory, disk I/O, network, and so on) of a collection of processes.

Cgroups provide the following features:

1. RESOURES LIMITS
2. PRIORITIZATION
3. ACCOUNTING
4. CONTROL

In conclusion Namespaces and cgroups are the building blocks for containers and modern applications. Having an understanding of how they work is important as we refactor applications to more modern architectures.Namespaces provide isolation of system resources, and cgroups allow for fine‑grained control and enforcement of limits for those resources.[This artical explains Namespaces AND cgroups in-depth ](https://www.nginx.com/blog/what-are-namespaces-cgroups-how-do-they-work/)
