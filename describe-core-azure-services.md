# Describe Core Azure Services (30-35%)

## Describe the coreAzure architectural components

### Regions
A region is a geographical area on the planet containing at least one, but potentially multiple datacenters that are in close proximity and networked together with a low-latency network. At the time of writing this, Azure is generally available in 60 regions and available in 140 countries.

Things to know about regions:
* Azure has more global regions than any other cloud provider.
* Regions provide customers the flexibility and scale needed to bring applications closer to their users.
* Regions preserve data residency and offer comprehensive compliance and resiliency options for customers.
* For most Azure services, when you deploy a resource in Azure, you choose the region where you want your resource to be deployed.

### Region Pairs
Each Azure region is paired with another region within the same geography at least 300 miles away, which together make a region pair.

Things to know about regional pairs:
* __Physical isolation__: When possible, Azure prefers at least 300 miles of separation between datacenters in a regional pair, although this isn't practical or possible in all geographies. Physical datacenter separation reduces the likelihood of natural disasters, civil unrest, power outages, or physical network outages affecting both regions at once.
* __Platform-provided replication__: Some services such as Geo-Redundant Storage provide automatic replication to the paired region.
* __Region recovery order__: In the event of a broad outage, recovery of one region is prioritized out of every pair. Applications that are deployed across paired regions are guaranteed to have one of the regions recovered with priority.
* __Sequential updates__: Planned Azure system updates are rolled out to paired regions sequentially (not at the same time) to minimize downtime, the effect of bugs, and logical failures in the rare event of a bad update.

### Azure geography
An Azure geography is a discrete market typically containing two or more regions that preserves data residency and compliance boundaries.

This division has several benefits:
* Geographies allow customers with specific data residency and compliance needs to keep their data and applications close.
* Geographies ensure that data residency, sovereignty, compliance, and resiliency requirements are honored within geographical boundaries.
* Geographies are fault-tolerant to withstand complete region failure through their connection to dedicated high-capacity networking infrastructure.

### Availability Options
* A __single virtual machine__ with premium storage has an __SLA of 99.9%__. You can quickly migrate existing virtual machines to Azure through "__lift and shift__". Lift and shift is a no-code option where each application is migrated as-is, providing the benefits of the cloud without the risks or costs of making code changes.
* By placing virtual machines in an __availability set__, you protect against datacenter failures and increases the __SLA to 99.95%__.
* Adding virtual machines to __availability zones__ protects from entire datacenter failures and increases the __SLA to 99.99%__, which is highest level of protection that is provided.
* For multi-region disaster recovery, region pairs protect and provide data residency boundaries.

### Availability sets
Availability sets are a way for you to ensure your application remains online if a high-impact maintenance event is required, or if a hardware failure occurs. Availability sets are made up of __Update domains (UD)__ and __Fault domains (FD)__.

### Update Domains
When a maintenance event occurs (such as a performance update or critical security patch applied to the host), the update is sequenced through update domains. Sequencing updates using update domains ensures that the entire datacenter isn't unavailable during platform updates and patching. Update domains are a logical section of the datacenter, and they are implemented with software and logic.

### Fault Domains
Fault domains provide for the physical separation of your workload across different hardware in the datacenter. This includes power, cooling, and network hardware that supports the physical servers located in server racks. In the event the hardware that supports a server rack becomes unavailable, only that rack of servers would be affected by the outage.

### Availability Zones
Availability zones are physically separate locations within an Azure region that use availability sets to provide additional fault tolerance.

Availability Zone features:
* Each availability zone is an isolation boundary containing one or more datacenters equipped with independent power, cooling, and networking.
* If one availability zone goes down, the other continues working.
* The availability zones are typically connected to each other through very fast, private fiber-optic networks.
* Availability zones allow customers to run mission-critical applications with high availability and low-latency replication.
* Availability zones are offered as a service within Azure, and to ensure resiliency, there's a minimum of three separate zones in all enabled regions.

### Resource Group
A resource group is a __unit of management__ for your resources in Azure. You can think of your resource group as a container that allows you to aggregate and manage all the resources required for your application in a single manageable unit.

Resource Group features:
* Each resource must exist in one, and only one, resource group.
* A resource group can contain resources that reside in different regions.
* You decide how you want to allocate resources to resource groups based on what makes the most sense for your organization.
* You can add or remove a resource to a resource group at any time.
* You can move a resource from one resource group to another.
* Resources for an application do not need to exist in the same resource group. However, it is recommended that you keep them in the same resource group for ease of management.
* If you delete a resource group, all resources contained within are also deleted.
* By applying role-based access control (RBAC) permissions to a resource group, you can ease administration and limit access to allow only what is needed.

### Azure Resource Manager
Azure Resource Manager is a management layer. With Azure Resource Manager, you can:
* __Deploy Application resources__: Update, manage, and delete all the resources for your solution in a single, coordinated operation.
* __Organize resources__: Manage your infrastructure through declarative templates rather than scripts. You can view which resources are linked by a dependency, and you can apply tags to resources to categorize them for management tasks, such as billing.
* __Control access and resources__: You can control who in your organization can perform actions on the resources. You manage permissions by defining roles, adding users or groups to the roles, and applying policies at resource group level.

## Describe some of the core products available in Azure

### Azure compute
Azure compute is an on-demand computing service for running cloud-based applications. It provides computing resources such as disks, processors, memory, networking and operating systems. There are many compute services two of the most common are: __virtual machines__ and __containers__.

### Virtual Machines (VMs)
Virtual machines (VMs) are software emulations of physical computers. They include a virtual processor, memory, storage, and networking resources. VMs host an operating system, and you're able to install and run software just like a physical computer.

### Azure Virtual Machines
Azure virtual machines let you create and use virtual machines in the cloud. It provides __IaaS__ and can be used in a variety of different ways.

### Virtual machine scale sets
Virtual machine scale sets are an Azure compute resource that you can use to deploy and manage a __set of identical VMs__. With all VMs configured the same, virtual machine scale sets are designed to support true __autoscale__.

### App services
With App services , you can quickly build, deploy, and scale enterprise-grade web, mobile, and API apps running on any platform. App Services is a __platform as a service__ (PaaS) offering.

### Azure Functions
Azure Functions are ideal when you're concerned only about the code running your service and not the underlying platform or infrastructure.

### Azure Container Instances (ACI)
Azure Container Instances offers the fastest and simplest way to run a container in Azure without having to manage any virtual machines or adopt any additional services. It is a __PaaS__ offering that allows you to upload your containers.

### Azure Kubernetes Service (AKS)
Azure Kubernetes Service is a complete orchestration service for containers with distributed architectures and large volumes of containers. Orchestration is the task of automating and managing a large number of containers and how they interact.

### Azure Networking
Azure Networking allows you to connect cloud and on-premises infrastructure and services to provide your customers and users the best possible experience. 

### Azure Virtual Network
Azure Virtual Network enables many types of Azure resources such as Azure VMs to securely communicate with each other, the internet, and on-premises networks. A virtual network is __scoped to a single region__; however, __multiple__ virtual networks from different regions can be connected using __virtual network peering__. With Azure Virtual Network you can provide isolation, segmentation, communication with on-premises and cloud resources, routing and filtering of network traffic.

### Azure Load Balancer
Azure Load Balancer can provide scale for your applications and create high availability for your services.

### Virtual Private Network (VPN) gateway
A VPN gateway is a specific type of virtual network gateway that is used to send encrypted traffic between an Azure Virtual Network and an on-premises location over the public internet.

### Azure Application Gateway
Azure Application Gateway is a web traffic load balancer that enables you to manage traffic to your web applications. It is the connection through which users connect to your application.

### Content Delivery Network
A Content Delivery Network (CDN) is a distributed network of servers that can efficiently deliver web content to users. It is a way to get content to users in their local region to minimize latency.

### Azure Storage
Azure Storage is a service that you can use to store files, messages, tables, and other types of information. Some of the most common storage service types in Azure are disks, files, objects, queues, and tables.

### Disk storage
Disk storage provides disks for virtual machines, applications, and other services to access and use as they need, similar to how they would in on-premises scenarios.

### Azure Blob storage
Azure Blob storage is Microsoft's object storage solution for the cloud. Blob storage is optimized for storing massive amounts of unstructured data, such as text or binary data.

### Azure Files
Azure Files enables you to set up highly available network file shares that can be accessed by using the standard Server Message Block (SMB) protocol. That means that multiple VMs can share the same files with both read and write access.

### Azure Queue service
The Azure Queue service is used to store and retrieve messages. Queue messages can be up to 64 KB in size, and a queue can contain millions of messages. Queues are generally used to store lists of messages to be processed asynchronously.

### Azure Table storage
Azure Table storage stores large amounts of structured data. The service is a NoSQL datastore which accepts authenticated calls from inside and outside the Azure cloud. Azure tables are ideal for storing structured, non-relational data.

### Azure Database Services
Azure database services are fully managed PaaS database services that free up valuable time you’d otherwise spend managing your database.

### Azure Cosmos DB
Microsoft Azure Cosmos DB is a globally distributed database service that enables you to elastically and independently scale throughput and storage across any number of Azure's geographic regions. It supports __schema-less data__ that lets you build highly responsive and Always On applications to support constantly changing data.

### Azure SQL Database
Azure SQL Database is a relational __database as a service (DaaS)__ based on the latest stable version of Microsoft SQL Server database engine.

### Azure Database Migration
The Azure Database Migration Service is a fully managed service designed to enable seamless migrations from multiple database sources to Azure data platforms with minimal downtime (online migrations).

### Azure Marketplace
Azure Marketplace is a service on Azure that helps connect end users with Microsoft partners, __independent software vendors (ISVs)__, and start-ups that are offering their solutions and services, which are optimized to run on Azure.

## Describe some of the solutions available on Azure

### IoT Central
IoT Central is a fully managed global IoT software as a service (SaaS) solution that makes it easy to connect, monitor, and manage your IoT assets at scale.

### Azure IoT Hub
Azure IoT Hub is a managed service hosted in the cloud that acts as a central message hub for __bi-directional communication__ between your IoT application and the devices it manages.

### Azure Synapse Analytics
Azure Synapse Analytics (formerly Azure SQL Data Warehouse) is a limitless analytics service that brings together enterprise data warehousing and big data analytics.

### Azure HDInsight
Azure HDInsight is a fully managed, open-source analytics service for enterprises. It is a cloud service that makes it easier, faster, and more cost-effective to process massive amounts of data.

### Azure Data Lake Analytics
Azure Data Lake Analytics is an on-demand analytics job service that simplifies big data. Instead of deploying, configuring, and tuning hardware, you write queries to transform your data and extract valuable insights.

### Azure Cognitive Services
Cognitive services are a collection of domain-specific pre-trained AI models that can be customized with your data. They are categorized broadly into vision, speech, language, and search.

### Azure Machine Learning Service
The Azure Machine Learning service provides a cloud-based environment you can use to develop, train, test, deploy, manage, and track machine learning models.

### Serverless computing
Serverless computing is a cloud-hosted execution environment that runs your code but abstracts the underlying hosting environment.

### Azure Functions
Azure Functions are ideal when you're only concerned with the code running your service and not the underlying platform or infrastructure. Azure Functions scale automatically and they are stateless.

### Azure Logic Apps
Logic Apps is a cloud service that helps you automate and orchestrate tasks, business processes, and workflows when you need to integrate apps, data, systems, and services across enterprises or organizations.

### Azure Event Grid
Event Grid allows you to easily build applications with event-based architectures. It's a fully managed, intelligent event routing service that uses a publish-subscribe model for uniform event consumption.

### Azure DevOps Services
DevOps Services provides development collaboration tools including high-performance pipelines, free private Git repositories, configurable Kanban boards, and extensive automated and cloud-based load testing.

### Azure Lab Services
Lab Services is a service that helps developers and testers quickly create environments in Azure, while minimizing waste and controlling cost.

### Azure App Service
With Azure App Service you can quickly and easily build web and mobile apps for any platform or device. Azure App Service enables you to build and host web apps, mobile back ends, and RESTful APIs in the programming language of your choice without managing infrastructure. It offers auto-scaling and high availability, supports both Windows and Linux, and enables automated deployments from GitHub, Azure DevOps, or any Git repo.

## Describe Azure management tools

### Azure portal
The Azure portal is a public website that you can access with any web browser.

### Azure PowerShell
Azure PowerShell is a module that you add to Windows PowerShell or PowerShell Core that enables you to connect to your Azure subscription and manage resources.

### Azure Command Line Interface (CLI)
Azure CLI is a cross-platform command-line program that connects to Azure and executes administrative commands on Azure resources.

### Azure Cloud Shell
Azure Cloud Shell is a browser-based scripting environment in your portal.

### Azure Mobile App
The Microsoft Azure mobile app allows you to access, manage, and monitor all your Azure accounts and resources from your iOS or Android phone or tablet.

### Azure REST API
Representational State Transfer (REST) APIs are service endpoints that support sets of HTTP operations (methods), which provide create, retrieve, update, or delete access to the service's resources.

### Azure Advisor
Azure Advisor is a free service built into Azure that provides recommendations on high availability, security, performance, and cost. Advisor analyzes your deployed services and looks for ways to improve your environment across those four areas.