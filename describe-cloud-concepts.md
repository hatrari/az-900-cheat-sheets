# Describe cloud concepts (15-20%)

## Describe the benefits and considerations of using cloud services

### Cloud computing 
Cloud computing is the delivery of computing services—including servers, storage, databases, networking, software, analytics, and intelligence—over the Internet (the cloud) to offer faster innovation, flexible resources, and economies of scale. You typically pay only for cloud services you use, and scale as your business needs change.

### High availability
The ability to keep services up and running for long periods of time, with very little downtime, depending on the service in question.

### Scalability
The ability to __increase or decrease__ resources for any given workload. You can add additional resources to service a workload (__scaling out__), or add additional capabilities to manage an increase in demand to the existing resource (__scaling up__). Scalability doesn't have to be done automatically.

### Elasticity
The ability to automatically or dynamically increase or decrease resources as needed. A distinction between scalability and elasticity is that elasticity is done __automatically__.

### Agility
The ability to react __quickly__. Cloud services can allocate and deallocate resources quickly.

### Fault tolerance
The ability to remain up and running even in the event of a component (or service) no longer functioning. Typically, redundancy is built into cloud services architecture, so if one component fails, a backup component takes its place.

### Disaster recovery
The ability to recover from an event which has taken down a cloud service. Cloud services disaster recovery can happen very quickly, with automation and services being readily available to use.

### Global reach
The ability to reach audiences around the globe.

### Customer latency capabilities
Cloud services have the ability to deploy resources in datacenters around the globe, which addresses any customer latency issues.

### Predictive cost considerations
The ability for users to predict the costs they will incur for a particular cloud service. You can also perform analysis based on future growth.

### Technical skill requirements and considerations
Cloud services can provide and manage hardware and software for workloads. A user can be an expert in the application they want to run without requiring skills to build and maintain the underlying hardware and software infrastructure.

### Increased productivity
On-site datacenters typically require a lot of hardware setup (otherwise known as racking and stacking), software patching, and other time-consuming IT management chores. Cloud computing eliminates the need for many of these tasks. This allows IT teams to spend time focusing on achieving more important business goals.

### Security
Cloud providers offer a broad set of policies, technologies, controls, and expert technology skills that can provide better security than most organizations can otherwise achieve.

### Economies of scale
the ability to reduce costs and gain efficiency when operating at a larger scale in comparison to operating at a smaller scale.

### Capital Expenditure (CapEx)
This is the up front spending of money on physical infrastructure (server, storage, network, technical personnel, etc), and then deducting that up front expense over time. The up front cost from CapEx has a value that reduces over time.

### Operational Expenditure (OpEx)
This is spending money on services or products now and being billed for them now. You can deduct this expense in the same year you spend it. There is no up front cost, as you pay for a service or product as you use it.

### Consumption-based model
It means that end users only pay for the resources that they use.
A consumption-based model has many benefits, including:
* No upfront costs.
* No need to purchase and manage costly infrastructure that they may or may not use to its fullest.
* The ability to pay for additional resources when they are needed.
* The ability to stop paying for resources that are no longer needed.

## Describe the differences between Public, Private and Hybrid cloud models

### Public cloud
This is the most common deployment model. In this case, you have no local hardware to manage or keep up-to-date everything runs on your cloud provider's hardware. In some cases, you can save additional costs by sharing computing resources with other cloud users. Businesses can use multiple public cloud providers of varying scale.

__Advantages:__
* __No CapEx__: You don’t have to buy a new server in order to scale.
* __Agility__: Applications can be made accessible quickly, and deprovisioned whenever needed.
* __Consumption-based model__: Organizations pay only for what they use, and operate under an OpEx model.
* __Maintenance__: Organizations have no responsibility for hardware maintenance or updates.
* __Skills__: No deep technical skills are required to deploy, use, and gain the benefits of a public cloud. Organizations can leverage the skills and expertise of the cloud provider to ensure workloads are secure, safe, and highly available.

__Disadvantages:__
* __Security__: There may be specific security requirements that cannot be met by using public cloud.
* __Compliance__: There may be government policies, industry standards, or legal requirements which public clouds cannot meet.
* __Ownership__: Organizations don't own the hardware or services and cannot manage them as they may wish.
* __Specific scenarios__: If organizations have a unique business requirement, such as having to maintain a legacy application, it may be hard to meet that requirement with public cloud services.

### Private cloud
In a private cloud, you create a cloud environment in your own datacenter and provide self-service access to compute resources to users in your organization. This offers a simulation of a public cloud to your users, but you remain completely responsible for the purchase and maintenance of the hardware and software services you provide.

__Advantages:__
* __Control__: Organizations have complete control over the resources.
* __Security__: Organizations have complete control over security.
* __Compliance__: If organizations have very strict security, compliance, or legal requirements, a private cloud may be the only viable option.
* __Specific scenarios__: If an organization has a specific scenario not easily supported by a public cloud provider (such as having to maintain a legacy application), it may be preferable to run the application locally.

__Disadvantages:__
* __Upfront CapEx__: Hardware must be purchased for start-up and maintenance.
* __Agility__: Private clouds are not as agile as public clouds, because you need to purchase and set up all the underlying infrastructure before they can be leveraged.
* __Maintenance__: Organizations have the responsibility for hardware maintenance and updates.
* __Skills__: Private clouds require in-house IT skills and expertise that may be hard to get or be costly.

### Hybrid cloud
A hybrid cloud combines public and private clouds, allowing you to run your applications in the most appropriate location. For example, you could host a website in the public cloud and link it to a highly secure database hosted in your private cloud (or on-premises datacenter).

__Advantages:__
* __Flexibility__: With a hybrid cloud setup, an organization can decide to run their applications either in a private cloud or in a public cloud.
* __Costs__: Organizations can take advantage of economies of scale from public cloud providers for services and resources as they wish. This allows them to access cheaper storage than they can provide themselves.
* __Control__: Organizations can still access resources over which they have total control.
* __Security__: Organizations can still access resources for which they are responsible for security.
* __Compliance__: Organizations maintain the ability to comply with strict security, compliance, or legal requirements as needed.
* __Specific scenarios__: Organizations maintain the ability to support specific scenarios not easily supported by a public cloud provider, such as running legacy applications. In this case, they can keep the old system running locally, and connect it to the public cloud for authorization or storage. Additionally, they could host a website in the public cloud, and link it to a highly secure database hosted in their private cloud.

__Disadvantages:__
* __Upfront CapEx__: Is still required before organizations can leverage a private cloud.
* __Costs__: Purchasing and maintaining a private cloud to use alongside the public cloud can be more expensive than selecting a single deployment model.
* __Skills__: Deep technical skills are still required to be able to set up a private cloud.
* __Ease of management__: Organizations need to ensure there are clear guidelines to avoid confusion, complications or misuse.

## Describe the differences between IaaS, PaaS and SaaS

The importance of understanding the __shared responsibility model__ is essential for customers who are moving to the cloud. Cloud providers offer considerable advantages for security and compliance efforts, but these advantages do not absolve the customer from protecting their users, applications, and service offerings.

### Infrastructure as a Service (IaaS)
IaaS is the most basic category of cloud computing services. With IaaS, you rent IT infrastructure servers and virtual machines (VMs), storage, networks, and operating systems from a cloud provider on a pay-as-you-go basis. It's an instant computing infrastructure, provisioned and managed over the internet.

__Advantages:__
* __No CapEx__: Users have no upfront costs.
* __Agility__: Applications can be made accessible quickly, and deprovisioned whenever needed.
* __Consumption-based model__: Organizations pay only for what they use and operate under an OpEx model.
* __Skills__: No deep technical skills are required to deploy, use, and gain the benefits of a public cloud. Organizations can leverage the skills and expertise of the cloud provider to ensure workloads are secure, safe, and highly available.
* __Cloud benefits__: Organizations can leverage the skills and expertise of the cloud provider to ensure workloads are made secure and highly available.
* __Flexibility__: IaaS is the most flexible cloud service as you have control to configure and manage the hardware running your application.

__Disadvantages:__
* __Management__: The shared responsibility model applies; the user manages and maintains the services they have provisioned, and the cloud provider manages and maintains the cloud infrastructure.

### Platform as a Service (PaaS)
PaaS provides an environment for building, testing, and deploying software applications. The goal of PaaS is to help create an application as quickly as possible without having to worry about managing the underlying infrastructure.

__Advantages:__
* __No CapEx__: Users have no upfront costs.
* __Agility__: PaaS is more agile than IaaS, and users do not need to configure servers for running applications.
* __Consumption-based model__: Users pay only for what they use, and operate on an OpEx model.
* __Skills__: No deep technical skills are required to deploy, use, and gain the benefits of PaaS.
* __Cloud benefits__: Users can leverage the skills and expertise of the cloud provider to ensure their workloads are made secure and highly available. In addition, users can gain access to more cutting-edge development tools and toolsets. They then can apply these tools and toolsets across an application's lifecycle.
* __Productivity__: Users can focus on application development only, as all platform management is handled by the cloud provider. Working with distributed teams as services is easier, as the platform is accessed over the internet and can be made globally available more easily.

__Disadvantages:__
* __Platform limitations__: There may be some limitations to a cloud platform that could affect how an application runs.

### Software as a Service (SaaS)
Software as a Service (SaaS) is software that is centrally hosted and managed for the end customer. It allows users to connect to and use cloud-based apps over the internet.

__Advantages:__
* __No CapEx__: Users don’t have any upfront costs.
* __Agility__: Users can provide staff with access to the latest software quickly and easily.
* __Pay-as-you-go pricing model__: Users pay for the software they use on a subscription model, typically monthly or yearly, regardless of how much they use the software.
* __Flexibility__: Users can access the same application data from anywhere.

__Disadvantages:__
* __Software limitations__: There may be some limitations to a software application that might affect how users work. Since you are using as-is software you don't have direct control of features.
