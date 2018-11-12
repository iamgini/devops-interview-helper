OpenShift Interview Questions

Following are some of the most frequently asked OpenShift interview questions in the interview, here are the answers for them.

What is OpenShift ?

OpenShift is a cloud development Platform as a Service.It is an open source development platform by which developer develops and deploys application on cloud.

What is OpenShift online?

It is public PaaS of OpenShift community using which one can build and deploy its application on public cloud. It is red hat hosting platform.

What is OpenShift container registry ?

Its an inbuilt storage that is used to store Docker images.

What is Routes in OpenShift?

In OpenShift Routes is a way to externalize the services by providing externally reachable hostname.In OpenShift routes are created using routers developed by admin.

What is authentication in OpenShift ?

In OpenShift master has inbuilt OAuth server which generates tokens that can be used for API authentication.

 Desired to gain proficiency on OpenShift? explore OpenShift Training.

What type of build strategies are used in OpenShift ?

Docker Strategy

Custom Strategy

Pipeline Strategy

Source-to-image Strategy

What is Source-to-image Strategy ?

In this from source code images are created.In Source-to-image strategy source code is downloaded and compiled and deployed in same container.From same code image is created.

Define Pods?

It is the collection of containers and its storage.

What are stateful Pods?

StatefulSets are a Kubernetes feature that enables pods to be stopped and restarted while retaining the same network address and storage attached to them. StatefulSets (PetSets in OCP 3.4) are still an experimental feature, but full support should be added in an upcoming release.

What are the identity providers in OAuth?

HTTPassword

LDAP

Allow ALL

Deny All

Basic Authentication

What is Source-to-image Strategy ?

In this from source code images are created.In Source-to-image strategy source code is downloaded and compiled and deployed in same container.From same code image is created.

What is Deployment Strategies?

OpenShift provides deployment strategies that are defined by each deployment con‐figuration. Each application will have its own requirements for availability and quality of service during a deployment. Architectural consideration should be made at design and development time for applications to take into account state (e.g., session state, atomic data—that is, what is the source of truth) and its effects on the quality of business service during updates to the application. For example, an application server that clusters server-side session state will have different concerns than a stateless application that relies on client-side caching only.

OpenShift provides strategies to support a variety of deployment scenarios, which we
will cover in the following sections.

What is Deployment Pod Resources?

A deployment is completed by a pod that consumes resources (memory and CPU) on a node. By default, pods consume unbounded node resources. However, if a project specifies default container limits, then pods consume resources up to those limits. Another way to limit resource use is to (optionally) specify resource limits as part of the deployment strategy.

What is  blue-green deployments?

The blue-green deployment strategy minimizes the time it takes to perform a deployment cutover by ensuring you have two versions of your application stacks available during the deployment. We can make use of the service and routing tiers to easily switch between our two running application stacks—hence it is very simple and fast to perform a rollback.

What is Port Binding?

OpenShift ships with a HAProxy-based router which provides ingress routing of HTTP/HTTPS traffic into the running pods. While the main use case is to support web traffic, it is also possible to support non-HTTP traffic (e.g., AMQP) by passing the traffic over SSL and adding the route hostname via the Server Name Indication (SNI) header. It is also possible to integrate existing load/balancing tiers into Open‐Shift.

What are labels in Open‐Shift?

Labels are identifying metadata consisting of key/value pairs attached to resources. Labels are used to add identifying attributes to objects that are relevant to users and can be used to reflect architectural or organizational concepts. Labels can be used in conjunction with label selectors to uniquely identify individual resources or groups of resources.

Examples:

Release

Environment

Relationship

DMZBased

Tier

Node types

User type

What are Annotations in Open‐Shift?

Annotations are similar to labels but primarily concerned with attaching nonidentifying information, which is primarily used by other clients such as tools or libraries. Annotations don’t have the concept of selectors.

Annotation examples
• example.com/skipValidation=true
• example.com/MD5Checksum=23798FGH
• example.com/BUILDDATE=3479845

What is Downward API in OpenShift?

The Downward API is a mechanism whereby pods can retrieve their metadata without having to call into the Kubernetes API. The following metadata can be retrieved and used to configure the running pods:

Labels

Annotations

Pod name, namespace, and IP address

Pod CPU/memory request and limit information

Certain information can be mounted into the pod as an environment variable,whereas other information can be accessed as files within a volume.

What is Build Configurations?

Builds are configured and controlled by build configuration resources. Build configurations contain the details of the chosen build strategy as well as the source of the developer-supplied artifacts such as Git location, the details of the builder image to be used, and the output image.

What is SSH authentication?

OpenShift uses the Secure Shell (SSH) network protocol to authenticate your account credentials to the OpenShift servers for secure communication. Successful authentication is necessary to manage your cloud environment, and OpenShift supports both RSA and DSA keys for SSH authentication. This section describes briefly how OpenShift authentication works, and provides information on how to manage SSH keys for OpenShift user accounts.
