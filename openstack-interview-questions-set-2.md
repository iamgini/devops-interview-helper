## Question 1. What You Mean By Tenant And Role Regarding Openstack ?
In OpenStack,  the authorization level of the user is called role and the group of users is called tenant.

## Question 2. What Types Of Storage Openstack Compute Provides?
OpenStack provides two classes of block storage:

Volume Storage: It is persistent and not dependent on any particular instance. Volumes are created by users and within Quota
Ephemeral Storage: It is associated with a single instance.They effectively disappear when a virtual machine is terminated.

## Question 3. Define Openstack?
OpenStack is a set of software tools for building and managing cloud computing platforms for public and private clouds.

## Question 4. Give An Overview Of Openstack Services?
OpenStack offers services like :

- Glance: Manages images in different formats
- Ceilometer: Openstack for billing
- Cinder: Provides persistent block storage
- Neutron: Enables users to create and attach interfaces to networks
- Nova: Provides instances on user’s demand
- Swift: Storage platform integrated directly into applications
- Heat: Allows automated infrastructure deployment
- Keystone: Provides authorization and authentication for users

## Question 5. What Are The Basic Functions Of Identity Service In Openstack?
The basic functions of Identity Service is:

Service Catalog: It provides a catalog of available services with their API endpoints
User Management: It tracks the users and their permissions

## Question 6. Explain Modular Architecture Of Openstack?
The three components that make modular architecture for OpenStack are:

- OpenStack Compute: For managing large networks of the virtual machine.
- Image Service: The delivery service provides discovery and registration for virtual disk images.
- OpenStack Object Storage: A storage system that provides support for both block storage and object storage.

## Question 7. Explain What Hypervisor Is And What Type Of Hypervisor Does Openstack Supports?
In virtualization technology, hypervisor is a software program that manages multiple operating systems (or multiple instances of the same operating system) on a single computer system.

The types of hypervisor that OpenStack supports are :
- KVM
- Containers
- Xen and HyperV
- VMware

## Question 8. What Is The Meaning Of Term “cinder” In Openstack Service?
Cinder is used for handling persistent storage in OpenStack.The one that is utilized by default is LVM, called Cinder-Volumes.

## Question 9. What Is The Command Used For Unpause And Pause An Instance?
- To unpause an instance – $ nova unpause INSTANCE_NAME
- To pause an instance – $ nova pause INSTANCE_NAME

## Question 10. Explain How You Can Transfer Volume From One Owner To Another In Openstack?
You can transfer a volume from one owner to another by using the command cinder transfer*.

## Question 11. What Are The Main Components Of Identity User Management?
- Users: It is a digital representation of a person, service or system who uses OpenStack cloud services
- Roles: A role includes a set of rights and privileges. A role determines what operations a user is permitted to perform in a given tenant
- Tenants: A container used to group or isolate resource or identity objects. Depending on service operator a tenant may map to a customer, account, organization or project.

## Question 12. Mention What Is The Command To Remove Network Interface From Bare-metal Node?
To remove network interface from bare-metal node command used is bare-metal – interface remove.

## Question 13. Explain What Is The Function Of Cinder Scheduler?
Cinder Scheduler or routing volume create requests to the appropriate volume service

Question 14. List Out The Storage Locations For Vm Images In Openstack?

Answer :

OpenStack Object Storage :

     Filesystem
     S3
     HTTP
     RBD or Rados Block Device
     GridFS

Question 15. Explain About Openstack Python Sdk?

Answer :

For writing python scripts and managing in Openstack cloud, SDK (Software Development Kit) is used. The SDK implements Python binding to the OpenStack API, which enables you to achieve automation tasks in Python by making calls on Python objects instead of making REST calls directly.

Question 16. Explain What Is Token In Openstack?

Answer :

Token is an alpha-numeric string which allows access to a certain set of services depending upon the access level of the user

Question 17. Explain What Is Cells In Openstack?

Answer :

Cells functionality enables you to scale an OpenStack Compute cloud in a more simplistic way.  When this functionality is enabled, the hosts in an OpenStack Compute cloud are partitioned into group called cells. Cells are configured as trees.

Question 18. For Networking, What Hardware Is Used In Openstack?

Answer :

In OpenStack, networking is done in following ways :

    Ports
    Vendor Plugins
    Networks
    Routers
    Subnets

Question 19. Mention What Are The Networking Options Used In Openstack?

Answer :

The networking options used in OpenStack are:

VLAN Network Manager: Compute creates a VLAN and bridge; DHCP server is started for each VLAN to pass out IP addresses to VM instances.
Flat DHCP Network Manager: IP addresses for VM instances are fetched from the subnet specified by the network administrator
Flat Network Manager: IP addresses for VM instances are fetched from the subnet, and then injected into the image on launch

Question 20. What Is The Command To Manage Floating Ip Addresses In Openstack?

Answer :

nova floating-ip-*

Question 21. What Is The Meaning Of Term “flavor” In Openstack?

Answer :

A flavour is an available hardware configuration for a server, which defines the size of a virtual server that can be launched.

Question 22. What Is Bare-metal Node And What Does It Comprised Of?

Answer :

    It gives access to control bare metal driver, through which user can control physical hardware resources on the same network.
    Bare metal node is comprised of two separate components
    Bare metal node Operating System: It is a base software, which runs on each node in the cluster.
    Bare metal node Orchestrator: It’s a management software, which acts as a dispatcher to all nodes in the cluster.

Question 23. What Is The Command Used To List Ip Address Information?

Answer :

$ nova floating-ip-pool-list

Question 24. What Are Functions Of “nova” ?

Answer :

    Instance life cycle management
    Management of compute resources
    Networking and Authorization
    REST-based API
    Asynchronous eventually consistent communication
    Hypervisor agnostic : support for Xen, XenServer/XCP, KVM, UML, VMware vSphere and Hyper-V

Question 25. What Are Components Of Openstack Compute ?

Answer :

Nova Cloud Fabric is composed of the following major components:

    API Server (nova-api)
    Message Queue (rabbit-mq server)
    Compute Workers (nova-compute)
    Network Controller (nova-network)
    Volume Worker (nova-volume)
    Scheduler (nova-scheduler)

Question 26. What Is Job Of Api-server ?

Answer :

The API Server provides an interface for the outside world to interact with the cloud infrastructure.

Question 27. What Is Rabbit Mq Server ?

Answer :

OpenStack communicates among themselves using the message queue via AMQP.

Question 28. What Are Functions And Features Of Swift ?

Answer :

    Storage of large sized objects
    Storage of large number of objects
    Data Redundancy
    Archival capabilities – Work with large datasets
    Data container for virtual machines and cloud apps
    Media Streaming capabilities
    Secure storage of objects
    Extreme scalability
    Backup and archival

Question 29. What Do You Understand By Horizon ?

Answer :

Horizon the web based dashboard can be used to manage /administer OpenStack services.

Question 30. What Are Commands To Generate Keypairs ?

Answer :

    ssh-keygen
    cd .ssh
    nova keypair-add –pub_key id_rsa.pub mykey

Question 31. How You Can View The Rules ?

Answer :

Rules can be viewed with the command:

$ nova secgroup-list-rules myservers

Question 32. Give An Example Where Logs Help In Openstack Security ?

Answer :

For instance, analyzing the access logs of Identity service or its replacement authentication system would alert us to failed logins, frequency, origin IP, whether the events are restricted to select accounts and other pertinent information. Log analysis supports detection.

Question 33. Why Compliance Is Required In Openstack ?

Answer :

Compliance means adhering to regulations, specifications, standards and laws.

An OpenStack deployment may require compliance activities for many purposes, such as regulatory and legal requirements, customer need, privacy considerations, and security best practices. The Compliance function is important for the business and its customers.

Question 34. What Are Data Privacy Concerns In Openstack, How Those Can Be Remediated?

Answer :

Data residency: Concerns over who owns data in the cloud and whether the cloud operator can be ultimately trusted as a custodian of this data have been significant issues in the past.

Data disposal:– Best practices suggest that the operator sanitize cloud system media (digital and non-digital) prior to disposal, release out of organization control or release for reuse.

Data not securely erased:- This may be remediated with database and/or system configuration for auto vacuuming and periodic free-space wiping.

Instance memory scrubbing, Cinder volume data, Image service delay delete feature.

Question 35. What Is Sanitization Process ?

Answer :

The sanitization process removes information from the media such that the information cannot be retrieved or reconstructed. Sanitization techniques, including clearing, purging, cryptographic erase, and destruction, prevent the disclosure of information to unauthorized individuals when such media is reused or released for disposal.

Question 36. How To Create A Normal User In Openstack ?

Answer :

sudo nova-manage user create user-name

Question 37. How You Assign A Project To A User ?

Answer :

sudo nova-manage project add –project=project_name

–user=user_name

Question 38. How You Can Remove A Rule From Security Group ?

Answer :

nova secgroup-delete-rule webserver tcp 443 443 0.0.0.0/0

Question 39. How To Display Images Using Nova Client ?

Answer :

nova image-list

Question 40. How To See A List Of Roles And The Associated Ids In Our Environment ?

Answer :

keystone role-list

Question 41. What Is Job Of User Crud ?

Answer :

The user CRUD filter enables users to use a HTTP PATCH to change their own password.

Question 42. Where Caching Configuration Is Stored ?

Answer :

The majority of the caching configuration options are set in the [cache] section of the keystone.conf file.

Question 43. What Is Alarm In Openstack ?

Answer :

Alarms provide user-oriented Monitoring-as-a-Service for resources running on OpenStack. This type of monitoring ensures you can automatically scale in or out a group of instances through the Orchestration module, but you can also use alarms for general-purpose awareness of your cloud resources’ health.

Question 44. How To Migrate Running Instances From One Openstack Compute Server To Another Openstack Compute Server ?

Answer :

    Check the ID of the instance to be migrated
    Check the information associated with the instance
    Select the compute node the instance will be migrated to.
    Check that Host has enough resources for migration
    Migrate the instance using the $ nova live-migration SERVER HOST_NAME command.

Question 45. How You Can Change Behavior Of Dhcp Server ?

Answer :

The behavior of dnsmasq can be customized by creating a dnsmasq configuration file

Question 46. What Is Orchestration ?

Answer :

Orchestration is an orchestration engine that provides the possibility to launch multiple composite cloud applications based on templates in the form of text files that can be treated like code.

Question 47. What Is Use Of Account Reaper ?

Answer :

In the background, the account reaper removes data from the deleted accounts.

Question 48. What You Will Do In Case Of Drive Failure ?

Answer :

In the event that a drive has failed, the first step is to make sure the drive is unmounted. This will make it easier for Object Storage to work around the failure until it has been resolved. If the drive is going to be replaced immediately, then it is just best to replace the drive, format it, remount it, and let replication fill it up.

Question 49. What You Will Do In Case Of Server Failure ?

Answer :

If a server is having hardware issues, it is a good idea to make sure the Object Storage services are not running. This will allow Object Storage to work around the failure while you troubleshoot.

If the server just needs a reboot, or a small amount of work that should only last a couple of hours, then it is probably best to let Object Storage work around the failure and get the machine fixed and back online. When the machine comes back online, replication will make sure that anything that is missing during the downtime will get updated.

If you cannot replace the drive immediately, then it is best to leave it unmounted, and remove the drive from the ring. This will allow all the replicas that were on that drive to be replicated elsewhere until the drive is replaced. Once the drive is replaced, it can be re-added to the ring.

Question 50. How You Will Install Dhcp Agent ?

Answer :

# apt-get install neutron-dhcp-agent

Question 51. Who Is Openstack For?

Answer :

OpenStack is for service providers, enterprises, government agencies and academic institutions that want to build public or private clouds. Industries range from IT & telco to SaaS and eCommerce to finance and healthcare. You can read more about how organizations are becoming agile, reducing costs and avoiding vendor lock-in with OpenStack.

Question 52. What Does It Mean For The Cloud Ecosystem?

Answer :

Wide adoption of an open-source, open-standards cloud should be huge for everyone. It means customers won’t have to fear lock-in and technology companies can participate in a growing market that spans cloud providers. Companies are already using OpenStack to provide public clouds, support, training and system integration services and hardware and software products.

A great analogy comes from the early days of the Internet: the transition away from fractured, proprietary flavors of UNIX toward open-source Linux. An open cloud stands to provide the same benefits for large-scale cloud computing that the Linux standard provided inside the server.

Question 53. Mention What Are The Three Components That Make Modular Architecture Of Openstack?

Answer :

The three components that make modular architecture for OpenStack are:

    OpenStack Compute: For managing large networks of the virtual machine
    OpenStack Object Storage: A storage system that provides support for both block storage and object storage
    Image Service: The delivery service provides discovery and registration for virtual disk images

Question 54. What Is Identity Service In Openstack?

Answer :

Keystone is the most important and preferred Identity Service in OpenStack and executes the complete OpenStack Identity API.

Question 55. How Can You Create A Token?

Answer :

Users first need to authenticate their Keystone credentials to create a token.
