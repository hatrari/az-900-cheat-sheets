# Describe Security, Privacy, Compliance, and Trust (25-30%)

## Describe securing network connectivity in Azure

### Azure Firewall
A __Firewall__ is a service that grants server access based on the __originating IP address__ of each request. __Azure Firewall__ is a managed, cloud-based, network security service that protects your Azure Virtual Network resources.

### Web Application Firewall (WAF)
WAF provides centralized, inbound protection for your web applications against common exploits and vulnerabilities.

### Azure DDoS Protection
Distributed Denial of Service (DDoS) attacks attempt to overwhelm and exhaust an application’s resources, making the application slow or unresponsive to legitimate users. When you combine Azure DDoS Protection with application design best practices, you help provide defense against DDoS attacks.

### Network Security Groups (NSG)
Network Security Groups (NSG) allow you to filter network traffic to and from Azure resources in an Azure virtual network. An NSG can contain multiple inbound and outbound security rules that enable you to filter traffic to and from resources by source and destination IP address, port, and protocol.

### Application security groups (ASG)
Application security groups (ASG) enable you to configure network security as a natural extension of an application's structure, allowing you to group virtual machines and define network security policies based on those groups.

## Describe core Azure Identity services

### Authentication.
Authentication is the process of establishing the identity of a person or service looking to access a resource.

### Authorization.
Authorization is the process of establishing what level of access an authenticated person or service has.

### Azure Active Directory
Azure Active Directory is a Microsoft cloud-based identity and access management service.

Azure AD provides services such as:
* __Authentication__: This includes verifying identity to access applications and resources, and providing functionality such as self-service password reset, multi-factor authentication (MFA), a custom banned password list, and smart lockout services.
* __Single sign-on (SSO)__: Enables users to remember only one ID and one password to access multiple applications.
* __Application management__: You can manage your cloud and on-premises apps using Azure AD Application Proxy, single sign-on, the My apps portal (also referred to as Access panel), and SaaS apps.
* __Business to business (B2B) identity services__: Manage your guest users and external partners while maintaining control over your own corporate data.
* __Business-to-customer (B2C) identity services__: Customize and control how users sign up, sign in, and manage their profiles when using your apps with services.
* __Device management__: Manage how your cloud or on-premises devices access your corporate data.

### Azure Multi-Factor Authentication (MFA)
Azure Multi-Factor Authentication provides additional security for your identities by requiring two or more elements for full authentication.

These elements fall into three categories:
* __Something you know__ could be a password or the answer to a security question.
* __Something you possess__ might be a mobile app that receives a notification, or a token-generating device.
* __Something you are__ is typically some sort of biometric property, such as a fingerprint or face scan used on many mobile devices.

## Describe security tools and features of Azure

### Azure Security Center
Azure Security Center is a monitoring service that provides threat protection across all of your services both in Azure, and on-premises. Security Center can:
* Provide security recommendations based on your configurations, resources, and networks.
* Monitor security settings across on-premises and cloud workloads, and automatically apply required security to new services as they come online.
* Continuously monitor all your services and perform automatic security assessments to identify potential vulnerabilities before they can be exploited.
* Use machine learning to detect and block malware from being installed on your virtual machines and services. You can also define a list of allowed applications to ensure that only the apps you validate can execute.
* Analyze and identify potential inbound attacks and help to investigate threats and any post-breach activity that might have occurred.
* Provide just-in-time access control for ports, reducing your attack surface by ensuring the network only allows traffic that you require.

Azure Security Center is available in two tiers:
* __Free__: Available as part of your Azure subscription, this tier is limited to assessments and recommendations of Azure resources only.
* __Standard__: This tier provides a full suite of security-related services including continuous monitoring, threat detection, just-in-time access control for ports, and more.

### Azure Key Vault
Azure Key Vault is a centralized cloud service for storing your applications' secrets. Key Vault helps you control your applications' secrets by keeping them in a single, central location and by providing secure access, permissions control, and access logging capabilities.

The benefits of using Key Vault include:
* __Centralized application secrets__: Centralizing storage for application secrets allows you to control their distribution and reduces the chances that secrets may be accidentally leaked.
* __Securely stored secrets and keys__: Azure uses industry-standard algorithms, key lengths, and HSMs, and access requires proper authentication and authorization.
* __Monitor access and use__: Using Key Vault, you can monitor and control access to company secrets.
* __Simplified administration of application secrets__: Key Vault makes it easier to enroll and renew certificates from public Certificate Authorities (CAs). You can also scale up and replicate content within regions and use standard certificate management tools.
* __Integrate with other Azure services__: You can integrate Key Vault with storage accounts, container registries, event hubs and many more Azure services.

### Azure Information Protection
Azure Information Protection is a cloud-based solution that helps organizations classify and (optionally) protect its documents and emails by applying labels. Labels can be applied automatically (by administrators who define rules and conditions), manually (by users), or with a combination of both (where users are guided by recommendations).

### Azure Advanced Threat Protection
Azure Advanced Threat Protection is a cloud-based security solution that identifies, detects, and helps you investigate advanced threats, compromised identities, and malicious insider actions directed at your organization. Azure ATP is capable of detecting known malicious attacks and techniques, security issues, and risks against your network.

Azure Advanced Threat Protection components:
* __Azure Advanced Threat Protection (ATP) portal__: Azure ATP has its own portal, through which you can monitor and respond to suspicious activity. The Azure ATP portal allows you to create your Azure ATP instance, and view the data received from Azure ATP sensors. You can also use the portal to monitor, manage, and investigate threats in your network environment.
* __Azure Advanced Threat Protection (ATP) sensor__: Azure ATP sensors are installed directly on your domain controllers. The sensor monitors domain controller traffic without requiring a dedicated server or configuring port mirroring.
* __Azure Advanced Threat Protection (ATP) cloud service__: Azure ATP cloud service runs on Azure infrastructure and is currently deployed in the United States, Europe, and Asia. Azure ATP cloud service is connected to Microsoft's intelligent security graph.

## Describe Azure governance methodologies

### Azure Policy
Azure Policy is a service in Azure that you use to create, assign, and, manage policies. These policies enforce different rules and effects over your resources, so those resources stay compliant with your corporate standards and service-level agreements (SLAs).

There are three steps to creating an implementing an Azure policy:
1. Create a policy definition
2. Assign a definition to a scope of resources (subscription, resource group)
3. Review the policy evaluation results

### Initiative definitions
An initiative definition is a collection of policy definitions that are tailored towards achieving a singular overarching goal. Initiative definitions simplify managing and assigning policy definitions.

### Initiative assignments
Like a policy assignment, an initiative assignment is an initiative definition assigned to a specific scope. Initiative assignments reduce the need to make several initiative definitions for each scope. This scope could also range from a management group to a resource group.

### Role-based access control (RBAC)
Role-based access control provides fine-grained access management for Azure resources, enabling you to grant users only the rights they need to perform their jobs. RBAC is provided at __no additional cost to all__ Azure subscribers.

RBAC uses an __allow model__. This means that when you are assigned a role, RBAC allows you to perform certain actions, such as read, write, or delete.

### Resource locks
Resource locks help you prevent accidental deletion or modification of your Azure resources.

### Azure Blueprints
Azure Blueprints enable cloud architects to define a repeatable set of Azure resources that implement and adhere to an organization's standards, patterns, and requirements. Azure Blueprint enables development teams to rapidly build and deploy new environments with the knowledge that they're building within organizational compliance with a set of built-in components that speed up development and delivery.

With Azure Blueprint, the relationship between the blueprint definition (__what should be deployed__) and the blueprint assignment (__what was deployed__) is __preserved__. This connection supports improved deployment tracking and auditing.

Azure Blueprints are __different__ from __Azure Resource Manager Templates__. When Azure Resource Manager Templates deploy resources, they have __no active relationship with the deployed resources__ (they exist in a local environment or in source control).

### Subscription governance
There are mainly three aspects to consider in relation to creating and managing subscriptions: 
* __Billing__: Reports can be generated by subscriptions, if you have multiple internal departments and need to do "chargeback", a possible scenario is to create subscriptions by department or project.
* __Access Control__: A subscription is a deployment boundary for Azure resources and every subscription is associated with an Azure AD tenant that provides administrators the ability to set up role-based access control (RBAC).
* __Subscription Limits__: Subscriptions are also bound to some hard limitations. For example, the maximum number of Express Route circuits per subscription is 10.

## Describe monitoring and reporting options in Azure

### Azure Monitor
Azure Monitor maximizes the availability and performance of your applications by delivering a comprehensive solution for collecting, analyzing, and acting on telemetry from your cloud and on-premises environments. Azure Monitor collects data from each of the following tiers: __Application monitoring data__, __Guest OS monitoring data__, __Azure resource monitoring data__, __Azure subscription monitoring data__ and __Azure tenant monitoring data__.

Under the resource settings you can enable __Diagnostics__:
* __Enable guest-level monitoring__
* __Performance counters__: collect performance data
* __Event Logs__: enable various event logs
* __Crash Dumps__: enable or disable
* __Sinks__: send your diagnostic data to other services for more analysis
* __Agent__: configure agent settings

Azure Monitor features can be organized into four categories, these categories are:
* __Analyze__: Application Insights, Azure Monitor for containers and Azure Monitor for VMs.
* __Respond__: Alerts and Autoscale.
* __Visualize__: Dashboards, Views and Power BI.
* __Integrate__: Integrate Azure Monitor with other systems and build customized solutions that use your monitoring data.

### Azure Service Health
Azure Service Health is a suite of experiences that provide personalized guidance and support when issues with Azure services affect you. It can notify you, help you understand the impact of issues, and keep you updated as the issue is resolved. Azure Service Health can also help you prepare for planned maintenance and changes that could affect the availability of your resources.

Azure Service Health is composed of the following:
* __Azure Status__ provides a global view of the health state of Azure services.
* __Service Health__ provides you with a customizable dashboard that tracks the state of your Azure services in the regions where you use them. You can use the Service Health dashboard to create and manage service __Health alerts__, which notify you whenever there are service issues that affect you.
* __Resource Health__ helps you diagnose and obtain support when an Azure service issue affects your resources.

## Describe privacy, compliance and data protection standards in Azure

### Microsoft privacy statement
The Microsoft privacy statement explains what personal data Microsoft processes, how Microsoft processes it, and for what purposes.

### Trust Center
The Trust Center is a website resource containing information and details about how Microsoft implements and supports security, privacy, compliance, and transparency in all Microsoft cloud products and services.

### Service Trust Portal (STP)
The Service Trust Portal (STP) hosts the Compliance Manager service, and is the Microsoft public site for publishing audit reports and other compliance-related information relevant to Microsoft’s cloud services.

### Compliance Manager
Compliance Manager is a workflow-based risk assessment dashboard within the Trust Portal that enables you to track, assign, and verify your organization's regulatory compliance activities related to Microsoft professional services and Microsoft cloud services such as Office 365, Dynamics 365, and Azure.

### Azure Government
Azure Government is a separate instance of the Microsoft Azure service. It addresses the security and compliance needs of US federal agencies, state and local governments, and their solution providers. Azure Government offers physical isolation from non-US government deployments and provides screened US personnel.

### Azure China 21Vianet
Azure China 21Vianet is operated by 21Vianet is a physically separated instance of cloud services located in China, independently operated and transacted by Shanghai Blue Cloud Technology Co., Ltd. ("21Vianet"), a wholly owned subsidiary of Beijing 21Vianet Broadband Data Center Co., Ltd.