OpenShift Interview Questions And Answers

1) What is OpenShift Container Platform?

A) OpenShift is an open source container application platform by Red Hat based on top of Docker containers and the Kubernetes container cluster manager for enterprise app development and deployment.

2) How OpenShift works with Docker and Kubernetes?

A) OpenShift combines the power of Docker and Kubernetes with an enterprise-ready control system. It enables you to create a Continues Deployment Pipeline with all you need from testing to autoscaling.

3) What is OpenShift Online?

A) OpenShift Online is Red Hat’s public cloud application development and hosting service.

4) What is OpenShift Dedicated?

A) OpenShift Dedicated is Red Hat’s managed private cluster offering, built around a core of application containers powered by Docker, with orchestration and management provided by Kubernetes, on a foundation of Red Hat Enterprise Linux. It’s available on the Amazon Web Services (AWS) and Google Cloud Platform (GCP) marketplaces.

5) What is OpenShift Container Platform?

A) OpenShift Container Platform is Red Hat’s on-premises private platform as a service product, built around a core of application containers powered by Docker, with orchestration and management provided by Kubernetes, on a foundation of Red Hat Enterprise Linux.

5) OpenShift environment that is running on Amazon Web Services consists of which systems?

A) When interacting with an OpenShift environment that is running on Amazon Web Services. The environment consists of the following systems:

    1 master nodes
    1 infrastructure nodes
    24 “application” nodes
    An NFS server

6) The infrastructure node is providing which services?

A) The infrastructure node is providing several services:

    Aggregated logging
    Cluster metrics
    GitLab

7) What is OpenShift CLI?

OpenShift ships with a feature rich web console as well as command line tools to provide users with a nice interface to work with applications deployed to the platform. The OpenShift tools are a single executable written in the Go programming language and is available for the following operating systems:

    Microsoft Windows
    Apple OS X
    Linux
    This lab manual
    The OpenShift Docker registry
    The OpenShift router
    Etherpad

8) What is OpenShift Web Console?

A) OpenShift also provides a feature-rich Web Console that provides a friendly graphical interface for interacting with the platform.

9) What are Pods in OpenShift?

A) In OpenShift, the smallest deployable unit is a Pod. A Pod is a group of one or more Docker containers deployed together and guaranteed to be on the same host.

Pods can contain multiple Docker instances. The general idea is for a Pod to contain a “server” and any auxiliary services you want to run along with that server. Examples of containers you might put in a Pod are, an Apache HTTPD server, a log analyzer, and a file service to help manage uploaded files.
OpenShift Origin Interview Questions

OpenShift Interview Questions # 10) What is OpenShift Origin?

A) OpenShift Origin is a distribution of Kubernetes optimized for continuous application development and multi-tenant deployment. OpenShift adds developer and operations-centric tools on top of Kubernetes to enable rapid application development, easy deployment and scaling, and long-term lifecycle maintenance for small and large teams.

OpenShift Interview Questions # 11) What are the features of OpenShift Origin?

A) OpenShift Origin Features:

    Easily build applications with integrated service discovery and persistent storage.
    Quickly and easily scale applications to handle periods of increased demand.
    Support for automatic high availability, load balancing, health checking, and failover.
    Push source code to your Git repository and automatically deploy containerized applications.
    Web console and a command-line client for building and monitoring applications.
    Centralized administration and management of an entire stack, team, or organization.
    Create reusable templates for components of your system, and iteratively deploy them over time.
    Roll out modifications to software stacks to your entire organization in a controlled fashion.
    Integration with your existing authentication mechanisms, including LDAP, Active Directory, and public OAuth providers such as GitHub.
    Multi-tenancy support, including team and user isolation of containers, builds, and network communication.
    Allow developers to run containers securely with fine-grained controls in production.
    Limit, track, and manage the developers and teams on the platform.
    Integrated Docker registry, automatic edge load balancing, cluster logging, and integrated metrics.

OpenShift Interview Questions # 12) What can you run on OpenShift?

A) OpenShift is designed to run any existing Docker images. Additionally, you can define builds that will produce new Docker images using a Dockerfile.

For an easier experience running your source code, Source-to-Image (S2I) allows developers to simply provide an application source repository containing code to build and run. It works by combining an existing S2I-enabled Docker image with application source to produce a new runnable image for your application.

OpenShift Interview Questions # 13) What are the security controls does OpenShift provide for containers?

A) OpenShift runs with the following security policy by default:

    Containers run as a non-root unique user that is separate from other system users
    They cannot access host resources, run privileged, or become root
    They are given CPU and memory limits defined by the system administrator
    Any persistent storage they access will be under a unique SELinux label, which prevents others from seeing their content
    These settings are per project, so containers in different projects cannot see each other by default
    Regular users can run Docker, source, and custom builds
    By default, Docker builds can (and often do) run as root. You can control who can create Docker builds through the builds/docker and builds/custom policy resource.
    Regular users and project admins cannot change their security quotas.

OpenShift Interview Questions # 14) What is Source-to-Image (S2I)?

A) Source-to-Image (S2I) is a toolkit and workflow for building reproducible Docker images from source code. S2I produces ready-to-run images by injecting source code into a Docker container and letting the container prepare that source code for execution.

By creating self-assembling builder images, you can version and control your build environments exactly like you use Docker images to version your runtime environments.

OpenShift Interview Questions # 15) What are the benefits of OpenShift Origin?

A) The benefits available to the developer are numerous:

    Run a PaaS locally on your laptop
    Run a PaaS behind your firewall
    Become a developer on a PaaS and expand your skills and solve interesting technical problems
    Integrate your middleware or framework into an open source PaaS
    Create a new thing based on PaaS technology
    By utilizing an open source IaaS codebase, build a cloud stack using open source

OpenShift Interview Questions # 16) What are the new features introduced in OpenShift Container Platform 3.7?

A) OpenShift Container Platform 3.7 significantly expands how we integrate third-party services for our customers, both on-premises and in the cloud. It includes:

The general availability of OpenShift Service Catalog, which includes a new user experience to make it easier for developers to find the runtimes, frameworks, and services they need to be productive.

Access to AWS through the OpenShift platform In OCP 3.7, AWS and OpenShift users will be able to configure and deploy AWS services from within the OpenShift platform, with a single path for support.

OpenShift Interview Questions # 17) What is OpenShift Cartridges?

A) Cartridges in OpenShift were the focal point for building applications. Each cartridge provided the required libraries, source code, build mechanisms, connection logic, and routing logic along with a pre-configured environment to run the components of your applications.

OpenShift Interview Questions # 18) What is Cartridge vs Image?

A) The easiest replacement term for the cartridge in OpenShift v3 is the image. An image does more than a cartridge from a packaging perspective, providing better encapsulation and flexibility.

But the cartridge concept also included logic for building, deploying, and routing which do not exist in images. In OpenShift v3, these additional needs are met by Source-to-Image (S2I) and templated configuration.

OpenShift Interview Questions # 19) What is Project vs Domain?

A) The project is essentially a rename of the domain from OpenShift v2. Projects do have several features that are not a part of domains in OpenShift v2.

OpenShift Interview Questions # 20) What is Gear vs Container?

A) The gear and container terms are interchangeable. Containers have a cleaner mapping of being one-to-one with images, whereas many cartridges could be added to a single gear. With containers, the collocation concept is satisfied by pods.
Red Hat OpenShift Interview Questions And Answers

21) What is Master vs Broker?

A) Masters in OpenShift v3 do the job of the broker layer in OpenShift v2. However, the MongoDB and ActiveMQ layers used by the broker in OpenShift v2 are no longer necessary because the key-value store etcd is typically installed with each master.

22) What are the features of OpenShift v3?

A) OpenShift v3 is a layered system designed to expose underlying Docker-formatted container image and Kubernetes concepts as accurately as possible, with a focus on easy composition of applications by a developer. For example, install Ruby, push code, and add MySQL.

23) What Are the Layers in OpenShift?

A) The Docker service provides the abstraction for packaging and creating Linux-based, lightweight container images. Kubernetes provides the cluster management and orchestrates containers on multiple hosts.

OpenShift Origin adds:

    Source code management, builds, and deployments for developers
    Managing and promoting images at scale as they flow through your system
    Application management at scale
    Team and user tracking for organizing a large developer organization
    Networking infrastructure that supports the cluster

24) What Is the OpenShift Origin Architecture?

A) OpenShift Origin has a microservices-based architecture of smaller, decoupled units that work together. It runs on top of a Kubernetes cluster, with data about the objects stored in etcd, a reliable clustered key-value store. Those services are broken down by function:

REST APIs, which expose each of the core objects.

25) Can you explain about Kubernetes Infrastructure in OpenShift?

A) Within OpenShift Origin, Kubernetes manages containerized applications across a set of containers or hosts and provides mechanisms for deployment, maintenance, and application-scaling. The Docker service packages, instantiates, and runs containerized applications.

A Kubernetes cluster consists of one or more masters and a set of nodes. You can optionally configure your masters for high availability (HA) to ensure that the cluster has no single point of failure.

Controllers, which read those APIs, apply changes to other objects, and report status or write back to the object.

26) What are Masters?

A) The master is the host or hosts that contain the master components, including the API server, controller manager server, and etcd. The master manages nodes in its Kubernetes cluster and schedules pods to run on nodes.

27) What are Nodes?

A) Nodes – A node provides the runtime environments for containers. Each node in a Kubernetes cluster has the required services to be managed by the master. Nodes also have the required services to run pods, including the Docker service, a kubelet, and a service proxy.

28) What is Kubelet?

A) Each node has a kubelet that updates the node as specified by a container manifest, which is a YAML file that describes a pod. The kubelet uses a set of manifests to ensure that its containers are started and that they continue to run.

29) What are Init Containers?

A) A pod can have init containers in addition to application containers. Init containers allow you to reorganize setup scripts and binding code. An init container differs from a regular container in that it always runs to completion. Each init container must complete successfully before the next one is started.

30) What is Image Version Tag Policy?

A) Rather than version numbers, the Docker service allows applying tags (such as v1, v2.1, GA, or the default latest) in addition to the image name to further specify the image desired, so you may see the same image referred to as centos (implying the latest tag), centos:centos7, or fd44297e2ddb.
