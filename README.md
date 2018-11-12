# openstack-interview-questions

## 1)      Explain what is OpenStack?

OpenStack is a set of software tools for managing and building cloud computing platforms for private and public clouds. It’s a free and open source software cloud computing platform.

## 2)      Mention what are the three components that make modular architecture of OpenStack?

The three components that make modular architecture for OpenStack are

    OpenStack Compute: For managing large networks of the virtual machine
    OpenStack Object Storage: A storage system that provides support for both block storage and object storage
    Image Service:  The delivery service provides discovery and registration for virtual disk images

## 3)      Give an overview of OpenStack Services?

OpenStack offers services like

    Keystone: Provides authorization and authentication for users
    Glance: Manages images in different formats
    Cinder: Provides persistent block storage
    Neutron: Enables users to create and attach interfaces to networks
    Nova: Provides instances on user’s demand
    Swift: Storage platform integrated directly into applications
    Ceilometer: Openstack for billing
    Heat: Allows automated infrastructure deployment

4)      What does “role” and “tenant” indicates in OpenStack?

In OpenStack, a tenant is referred for the group of users while role indicates the authorization level of the user.

5)      Explain what hypervisor is and what type of hypervisor does OpenStack supports?

Hypervisor is a piece of computer software or hardware that creates and run virtual machines. A system on which one or more virtual machines is defined is referred as host machine.

The types of hypervisor that supports OpenStack are

    KVM
    VMware
    Containers
    Xen and HyperV

OpenStack

6)      What are the two types of storage does OpenStack Compute provides?

OpenStack provides two classes of block storage,

    Ephemeral Storage:  It is associated with a single unique instance. Based on the instance, the size is defined. When the instance associated with it is terminated, data on ephemeral storage ceases to exist
    Volume Storage:   This storage is not dependent on any particular instance and is persistent.  Volumes are user created and within Quota

7)      What are the basic functions of Identity Service in OpenStack?

The basic functions of Identity Service is

    User Management:  It tracks the users and their permissions
    Service Catalog: It provides a catalog of available services with their API endpoints

8)      What are the main components of identity user management?

    Users: It is a digital representation of a person, service or system who uses OpenStack cloud services
    Tenants: A container used to group or isolate resource or identity objects.  Depending on service operator a tenant may map to a customer, account, organization or project
    Roles:  A role includes a set of rights and privileges.  A role determines what operations a user is permitted to perform in a given tenant

9)      Mention what are the networking options used in OpenStack?

The networking options used in OpenStack are

    Flat Network Manager: IP addresses for VM instances are fetched from the subnet, and then injected into the image on launch
    Flat DHCP Network Manager:  IP addresses for VM instances are fetched from the subnet specified by the network administrator
    VLAN Network Manager: Compute creates a VLAN and bridge; DHCP server is started for each VLAN to pass out IP addresses to VM instances.

10)   What is the meaning of term “Cinder” in OpenStack service?

For handling persistent storage for virtual machines, OpenStack provides the service referred as Cinder. There are multiple backends for cinder.  The one that is utilized by default is LVM, called Cinder-Volumes.

11)   List out the storage locations for VM images in OpenStack?

    OpenStack Object Storage
    Filesystem
    S3
    HTTP
    RBD or Rados Block Device
    GridFS

12)   Explain what is Cells in OpenStack?

Cells functionality enables you to scale an OpenStack Compute cloud in a more simplistic way.  When this functionality is enabled, the hosts in an OpenStack Compute cloud are partitioned into group called cells. Cells are configured as trees.

13)   For networking, what hardware is used in OpenStack?

In OpenStack, networking is done in following ways

    Networks
    Routers
    Subnets
    Ports
    Vendor Plugins

14)   Explain how you can transfer volume from one owner to another in OpenStack?

You can transfer a volume from one owner to another by using the command cinder transfer*.

15)   What is the command to manage floating IP addresses in OpenStack?

nova floating-ip-*

16)   What is bare-metal node and what does it comprised of?

It gives access to control bare metal driver, through which you can control physical hardware resources on the same network.

Bare metal node is comprised of two separate components

    Bare metal node Orchestrator: It’s a management software, which acts as a dispatcher to all nodes in the cluster.
    Bare metal node Operating System: It is a base software, which runs on each node in the cluster.

17)   Mention what is the command to remove network interface from bare-metal node?

To remove network interface from bare-metal node command used is bare-metal – interface remove.

18)   Explain what is the function of Cinder Scheduler?

Cinder Scheduler or routing volume create requests to the appropriate volume service

19)   Explain what is Token in OpenStack?

Token is an alpha-numeric string which allows access to a certain set of services depending upon the access level of the user

20)   Explain about OpenStack Python SDK?

For writing python scripts and managing in Openstack cloud, SDK (Software Development Kit) is used.  The SDK implements Python binding to the OpenStack API, which enables you to achieve automation tasks in Python by making calls on Python objects instead of making REST calls directly.

21)   What is the command used for pause and unpause an instance?

    To pause an instance, command used is $ nova pause INSTANCE_NAME
    To unpause an instance, command used is $ nova unpause INSTANCE_NAME

22)   What is the command used to list IP address information?

$ nova floating-ip-pool-list

23)   What is the meaning of term “flavor” in OpenStack?

A flavour is an available hardware configuration for a server, which defines the size of a virtual server that can be launched.
