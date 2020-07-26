# Describe Azure Pricing, Service Level Agreements, and Lifecycles (20-25%)

## Describe Azure subscriptions

### Azure subscription
Using Azure requires an Azure subscription which provides you with authenticated and authorized access to Azure products and services and allows you to provision resources. An Azure subscription is a logical unit of Azure services that links to an Azure account, which is an identity in Azure Active Directory (Azure AD) or in a directory that an Azure AD trusts.

An account can have one subscription or multiple subscriptions that have different billing models and to which you apply different access-management policies. There are two types of subscription boundaries that you can use, including:
* __Billing boundary__: This subscription type determines how an Azure account is billed for using Azure. You can create multiple subscriptions for different types of billing requirements, and Azure will generate separate billing reports and invoices for each subscription so that you can organize and manage costs.
* __Access control boundary__: Azure will apply access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. An example is that within a business, you have different departments to which you apply distinct Azure subscription policies. This allows you to manage and control access to the resources that users provision with specific subscriptions.

### Subscriptions offers
Azure offers free and paid subscription options to suit different needs and requirements:
* __A free account__: Get started with 12 months of popular free services, a credit to explore any Azure service for 30 days, and 25+ services that are always free.
* __Pay-As-You-Go__: This subscription allows you to pay for what you use by attaching a credit or debit card to your account.
* __Member offers__: Your existing membership to certain Microsoft products and services affords you credits for your Azure account and reduced rates on Azure services.

### Management groups
The organizing structure for resources in Azure has four levels:
* __Management groups__: These are containers that help you manage access, policy, and compliance for multiple subscriptions. All subscriptions in a management group automatically inherit the conditions applied to the management group.
* __Subscriptions__: A subscription groups together user accounts and the resources that have been created by those user accounts. For each subscription, there are limits or quotas on the amount of resources you can create and use. Organizations can use subscriptions to manage costs and the resources that are created by users, teams, or projects.
* __Resource groups__: A resource group is a logical container into which Azure resources like web apps, databases, and storage accounts are deployed and managed.
* __Resources__: Resources are instances of services that you create, like virtual machines, storage, or SQL databases.

## Describe planning and management of costs

### Purchase Azure products and services
There are three main customer types on which the available purchasing options for Azure products and services is contingent, including:
* __Enterprise__: Enterprise customers sign an Enterprise Agreement with Azure that commits them to spending a negotiated amount on Azure services, which they typically pay __annually__. Enterprise customers also have access to __customized Azure pricing__.
* __Web direct__: Web direct customers pay public prices for Azure resources, and their __monthly billing__ and payments occur through the Azure website.
* __Cloud Solution Provider__: Cloud Solution Provider (CSP) typically are Microsoft partner companies that a customer hires to build solutions on top of Azure. Payment and billing for Azure usage occurs through the customer's CSP.

### Factors affecting costs
When you provision an Azure resource, Azure creates one or more meter instances for that resource. The meters track the resources' usage, and each meter generates a usage record that is used to calculate your bill.
* __Usage meters__: Compute Hours, Data Transfer In and Out, Standard IO-Block Blob Read, Write and Delete, etc.
* __Resource type__.
* __Services__: Azure usage rates and billing periods can differ between __Enterprise__, __Web Direct__, and __Cloud Solution Provider (CSP)__ customers.
* __Location__.

### Bandwidth
Bandwidth refers to data moving in and out of Azure datacenters. __Some inbound__ data transfers, are __free__. For __outbound__ data transfers, data transfer pricing is based on Zones.

### Zone
A Zone is a geographical grouping of Azure Regions for billing purposes.

### Pricing Calculator
The Pricing Calculator is a tool that helps you estimate the cost of Azure products.

### Total Cost of Ownership Calculator
The Total Cost of Ownership Calculator is a tool that you use to estimate cost savings you can realize by migrating to Azure. To use the TCO calculator, complete the three steps that the following sections explain.
1. __Define your workloads__: Enter details about your on-premises infrastructure into the TCO calculator according to four groups (Servers, Databases, Storage and Networking).
2. __Adjust assumptions__: Adjust the values of key assumptions that the TCO calculator makes, which might vary between customers.
3. __View the report__: The report allows you to compare the costs of your on-premises infrastructure with the costs using Azure products and services to host your infrastructure in the cloud.

### Azure Reservations
Azure Reservations offer discounted prices on certain Azure products and resources. To get a discount, you reserve products and resources by paying in advance.

### Explore minimizing costs
The following best practice guidelines can help minimize your Azure costs:
* Perform cost analyses (Azure Pricing and Total Cost of Ownership (TCO) calculators).
* Monitor usage with Azure Advisor.
* Use spending limits.
* Use Azure Reservations.
* Choose low-cost locations and regions.
* Research available cost-saving offers.
* Apply tags to identify cost owners.

### Cost Management
Cost Management is an Azure product that provides a set of tools for monitoring, allocating, and optimizing your Azure costs.

The main features of the Azure Cost Management toolset include:
* __Reporting__: Generate reports using historical data to forecast future usage and expenditure.
* __Data enrichment__: Improve accountability by categorizing resources with tags that correspond to real-world business and organizational units.
* __Budgets__: Create and manage cost and usage budgets by monitoring resource demand trends, consumption rates, and cost patterns.
* __Alerting__: Get alerts based on your cost and usage budgets.
* __Recommendations__: Receive recommendations to eliminate idle resources and to optimize the Azure resources you provision.
* __Price__: Free to Azure customers.

## Describe Azure Service Level Agreements (SLAs)

### Service Level Agreements (SLAs)
A SLA defines performance targets for an Azure product or service. The performance targets that a SLA defines are specific to each Azure product and service.

SLAs also describe how Microsoft will respond if an Azure product or service fails to perform to its governing SLA's specification.

### Composite SLA
When combining SLAs across different service offerings, the resultant SLA is a called a Composite SLA. The resulting composite SLA can provide higher or lower uptime values, depending on your application architecture.

### Application SLA
You can create your own SLAs and set performance targets to suit your specific Azure application. When creating an Application SLA consider the following:
* __Identify workloads__: A workload is a distinct capability or task that is logically separated from other tasks, in terms of business logic and data storage requirements.
* __Plan for usage patterns__: Usage patterns also play a role in requirements.
* __Establish availability metrics__: mean time to recovery (MTTR) and mean time between failures (MTBF).
* __Establish recovery metrics__: recovery time objective and recovery point objective (RPO). RTO is the maximum acceptable time an application can be unavailable after an incident. RPO is the maximum duration of data loss that is acceptable during a disaster.
* __Implement resiliency strategies__: Resiliency is the ability of a system to recover from failures and continue to function.
* __Build availability requirements into your design__: Availability is the proportion of time your system is functional and working.

## Describe service lifecycle in Azur

### Preview feature
An Azure feature is available to certain Azure customers for evaluation purposes.

### Public preview
An Azure feature is available to all Azure customers for evaluation purposes.

### Azure Preview Terms and Conditions
Azure feature previews are available with their own terms and conditions. The terms and conditions are specific to each Azure preview.

### General Availability (GA)
Once a feature is evaluated and tested successfully, it may release to customers as part of Azure. A feature released to all Azure customers typically goes to General Availability or GA.

### Azure updates 
Azure updates is a page for information about the latest updates to Azure products, services, and features, as well as product roadmaps and announcements.