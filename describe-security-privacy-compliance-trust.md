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