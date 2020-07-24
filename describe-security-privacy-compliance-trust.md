# Describe Security, Privacy, Compliance, and Trust(25-30%)

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