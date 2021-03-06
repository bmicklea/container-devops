# container-devops

#How Containers are Disrupting Devops
DevOps is implemented through continuous delivery software pipeline. Continuous delivery encompasses continuous development, integration and deployment. With the rapid adoption of containers we asked ourselves,
“How do containers redefine DevOps?"


##Containers Make Environments Consistent
Containers provide a common set of building blocks that can be reused in any stage of development to recreate identical environments for development, testing, staging, and production.  Containers extend the idea of "write once, deploy anywhere" to an infrastructure abstraction that application developers can easily consume and operations professionals can predictably manage.

##Containers Make Tooling Consistent
Containers provide a disposable, reusable unit that can execute a segment of a delivery pipeline. Critical code quality, analysis, build, and test functions can be consistently reused within developer workspaces, continuous integration systems, and release management tools. Service injection into containers allows developers to code more productively and tooling vendors to provide value throughout the pipeline.


----------------------------------------------------------------------

##Code & Image Lifecycle With Containers
Containers defined by recipes allow developers to edit, version and commit changes in the same way they do code leading to a similar (and sometimes dependent) image lifecycle.

###1st column: The Code Lifecycle
1. Clone
2. Edit
3. Analyze
4. Build
5. Package (Artifacts and Source Injected [points to #3 in Image Lifecycle below])
6. Run
7. Debug
8. Commit
9. Push

###2nd column: The Image Lifecycle
1. Clone
2. Edit
3. Build (Dependency [points to #4 in the Code Lifecycle above])
4. Label
5. Push

----------------------------------------------------------------------
##Continuous Delivery and DevOps with Containers
Containers are being used by the products below to evolve and revolutionize the continuous delivery and DevOps pipelines.

###1st column: Continuous Delivery:
1. Continuous Development
2. Continuous Integration
3.Continuous Deployment

###2nd column: DevOps Pipeline:
1. Author Code & Check In
2. Check Out & Build Code
3. Unit Test
4. Quality Control
5. Package and Archiving
6. Integration Testing
7. Deploy to Test Environment
8. Deploy to pre-production
9. Acceptance testing
10. Deploy to Production
11. Management & Monitoring


----------------------------------------------------------------------

###Continuous Development
####Developer Workspace
[Codenvy] (https://codenvy.com/) (RESTful workspaces built with Docker containers)

Eclipse [Che] (http://www.eclipse.org/che/) (hosted workspaces that use containers for microservices)

JetBrains [IntelliJ Idea](https://www.jetbrains.com/idea/) (manage Docker containers from IDE)

[Nitrous.io](https://pro.nitrous.io/?l=1) (Docker containers as workspace)

[Vagrant](http://docs.vagrantup.com/v2/provisioning/docker.html) (Docker provisioner)

VMware [AppCatalyst](http://blogs.vmware.com/cloudnative/vmware-appcatalyst) (desktop hypervisor optimized for containers)



####Source Code Management
Containers have not yet significantly changed source code management.

###Continuous Integration
####Continuous Integration
[CircleCi](https://circleci.com/docs/docker) (supports Docker-based dev, test and deploy workflow)

[CodeFresh](http://codefresh.io/) (NodeJS workspaces built with Docker)

Cloudbees [Jenkins CI](https://www.cloudbees.com/jenkins/about/code-quality-analysis) (build slaves runnable within  containers)

[Codeship](https://codeship.com/features/parallelci) (Docker-based continuous integration and delivery)

[Drone.io](http://blog.drone.io/2014/2/5/open-source-ci-docker.html) (open source continuous integration built on Docker)

[Electric Cloud](http://electric-cloud.com/plugins/directory/p/docker/) (plug-in to invoke containers while building)

[Shippable](https://app.shippable.com/) (automated DevOps with Docker)

[Wercker](http://wercker.com/) (containerized build pipeline)

XebiaLabs [Overcast](https://github.com/xebialabs/overcast) (Docker for integration testing with other services)


####Code Quality Analysis
[CodeClimate](https://codeclimate.com/) (static analysis with containers)

[SonarQube](http://www.sonarqube.org/) (code quality with containers)


####Packaging and Build Automation
Atlassian [Bamboo](https://www.atlassian.com/software/bamboo)(using Docker containers to create build agents)

[Bitnami](https://bitnami.com/) (image cloud hosting)

[Gradle](https://gradle.org) (build management through Docker)


####Testing Frameworks
[PhantomJsEnv](https://github.com/Codeception/PhantomJsEnv) (can be run through Docker instead of installed)

[RoboCI](https://github.com/Codegyre/RoboCI) (aimed to run Travis CI builds locally inside Docker containers)

[Salt](http://docs.saltstack.com/en/latest/ref/states/all/salt.states.dockerio.html) (allows unit testing within container)

[SeleniumEnv](https://github.com/Codeception/SeleniumEnv) (can be run through Docker instead of installed)


###Continuous Deployment

####Artifact and Image Registry
Docker [Hub](https://www.docker.com/docker-hub) (hosted registry service)

Docker [Trusted Registry](https://www.docker.com/docker-trusted-registry) (private dedicated image registry)

[Google Container Registry](https://cloud.google.com/container-registry/) (secure Docker image storage)

JFrog [Artifactory](http://www.jfrog.com/confluence/display/RTF/Docker+Repositories) (doubles as Docker and artifact registry)

[Quay.io](https://quay.io/plans/) (secure hosting for Docker registries)

[Tutum Registry](https://support.tutum.co/support/solutions/articles/5000012183-using-tutum-s-private-Docker-image-registry) (private Docker registry)


####Release Automation
[Ansible](http://www.ansible.com/docker) (playbooks will generate consistent app in containers & vms)

[Chef.io](https://www.chef.io/solutions/containers/) (container management, provisioning and automation)

Amazon [OpsWorks](http://aws.amazon.com/opsworks/) (how to integrate with Docker can be found here)

PuppetLabs [Puppet Forge](https://forge.puppetlabs.com/tags/docker) (Docker management)

[Salt](http://docs.saltstack.com/en/latest/ref/states/all/salt.states.dockerio.html) (container management, provisioning and automation)


####Operations Tools
[AppDynamics](http://community.appdynamics.com/t5/eXchange-Community-AppDynamics/Docker-Monitoring-Extension/idi-p/14749) (extension for Docker monitoring)

CenturyLink Labs [Panamax.io](http://panamax.io/) (tools to visualize & manage containers)

[New Relic](https://blog.newrelic.com/2015/05/06/docker-support-2/) (distributed container monitoring and analytics)

[SignalFx](http://blog.signalfx.com/signalfx-is-proud-to-join-the-docker-ecosystem-technology-partner-program) (streaming analytics of Docker apps)

[Sysdig](https://sysdig.com/distributed-container-monitoring-sysdig-cloud-revolution/) (distributed container monitoring)


----------------------------------------------------------------------

##Container Infrastructure
ActiveState [Stackato](http://www.activestate.com/stackato) (agile PaaS platform optimized for containers)

Alpine [Linux](http://www.alpinelinux.org) (lightweight operating system container-optimized)

Amazon [EC2 Container Service](http://aws.amazon.com/ecs/) (Docker extension tools)

Apache [Mesos](http://mesos.apache.org/) (distributed systems and container kernel)

Apache [Zookeeper](https://zookeeper.apache.org) (centralizes container configurations)

[Brightbox](https://www.brightbox.com/) (high performance and flexible cloud servers and storage)

[CenturyLink Cloud](https://www.ctl.io/) (cloud management service with container support)

[Ceph](http://ceph.com/) (distributed block storage for Docker)

ClusterHQ [Flocker](https://clusterhq.com/2015/06/17/flocker-1-0/) (open source container data volume manager)

CoreOS [Tectonic](https://tectonic.com/) (kubernetes cluster for Docker)

CoreOS [Flannel](https://coreos.com/flannel/docs/latest/flannel-config.html) (cross-container communication)

Datawise.io [Project 6](http://www.datawise.io/project-6.html) (deploy and manage Docker 
containers across clusters)

Docker [Compose](https://docs.docker.com/compose/) (define and running multi-container applications)

Docker [Machine](https://www.docker.com/docker-machine) (automated Docker provisioning)

Docker [Swarm](https://docs.docker.com/swarm/) (native clustering for Docker)

EngineYard [Deis](http://deis.io/overview/) (open source PaaS for Docker)

Joyent [Triton](https://www.joyent.com/) (elastic container infrastructure)

Google [Compute Engine](https://cloud.google.com/compute/) (PaaS with container managed service)

Google [Kubernetes](http://kubernetes.io/) (orchestration of services running pods of containers)

HashiCorp [Packer.io](https://www.packer.io/) (image construction automation)

HashiCorp [Consul.io](https://www.consul.io/) (finds and configure infrastructure services)

IBM [Bluemix](https://console.ng.bluemix.net/) (hybrid PaaS based upon CloudFoundry and Docker)

[Jelastic](https://jelastic.com/docker/) (multi-container orchestration platform)

Microsoft [Azure](https://azure.microsoft.com/en-us/) (PaaS with container managed services)

Mesosphere [DCOS](https://mesosphere.com/product/) (data center OS works with Docker)

[Nirmata](http://nirmata.com/tag/docker/) (application deployment and operations with Docker)

OpenStack [Nova](https://wiki.openstack.org/wiki/Docker) (launches containers on a massive scale)

[Pertino](http://pertino.com/pertino-simplifies-networking-of-docker-containers-across-any-cloud-anywhere) (builds container-level VPC networks)

Portworx [PWX](http://portworx.com/products/) (scale out block storage for Docker)

Rackspace [Managed Cloud](http://www.rackspace.com/cloud) (management software)

RancherLabs [Rancher](http://rancher.com/rancher/) (infrastructure platform for Docker)

RancherLabs [RancherOS](http://rancher.com/rancher-os/) (Linux distribution that runs OS as Docker containers) 

Red Hat [Atomic](http://www.projectatomic.io/) (lightweight immutable platform for running containers)

Red Hat [OpenShift](https://www.openshift.com/) (hybrid PaaS based on Docker)

VMware [Photon](https://vmware.github.io/photon/) (lightweight linux host for containers)

[Weave](http://weave.in/) (create a network of Docker containers)






