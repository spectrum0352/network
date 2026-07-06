# Architecture

A network security architecture is a layered defense system safeguarding your network's infrastructure and data. It combines various tools to fight unauthorized access, malware, and other threats. Here are key components:

- **Firewalls:** The first line of defense, controlling traffic flow based on pre-defined rules.
- **Intrusion Detection/Prevention Systems (IDS/IPS):** Monitors network traffic for suspicious activity and can alert or block it.
- **Access Control Systems:** Determine who can access what resources and their permissions.
- **Encryption:** Scrambles data for authorized users only, protecting sensitive information.
- **Network Segmentation:** Divides the network into smaller sections to limit the impact of attacks.
- **Vulnerability Management:** Continuously identifies and patches weaknesses in systems and software.
- **Security Information and Event Management (SIEM):** Collects and analyses security data to identify potential threats.
- **Security Orchestration, Automation, and Response (SOAR):** Automates routine security tasks for better efficiency.
- **Secure Access Service Edge (SASE):** A cloud-based approach that combines network security with access control.
- **Zero-Trust Security:** A model where no user or device is inherently trusted, requiring constant verification.

## Components

- Functionalities: These are the services that support network operations and user activities, such as:
- Dynamic Host Configuration Protocol (DHCP): Automatically assigns IP addresses to devices on the network.
- Network Address Translation (NAT): Translates private IP addresses into public IP addresses, conserving IP address space and enhancing security.
- File sharing services: Allow users to share files and resources across the network.
- Printing services: Enable users to access shared printers on the network.
- Directory services: Store and manage information about users, devices, and resources on the network, such as Active Directory.
- What is a good practice for securing network devices?
- Disabling unused ports.


- **Network appliances**: Servers, Routers, Switches, Load Balancers, Clients.
- **Network protocols**: TCP/IP, DNS, DHCP, FTP, HTTP/HTTPS, SMTP.
- **Network security tools**: Firewalls, WAFs, VPN, IPsec, TLS, etc.
- **Data privacy solutions**: Classification, encryption, key management, etc…


- Network Firewall
- Web Application Firewall
- Intrusion Detection System
- Intrusion Prevention System
- Payload Inspection System
- Distributed Denial of Service Protection
- Network Segmentation
- Load Balancer

**What is the difference while configuring the point to site vpn and site to site vpn?**

| Feature | P2S VPN | S2S VPN |
|----|----|----|
| Number of networks involved | One | Two or more |
| VPN client software required | Yes | No |
| VPN gateway required | Yes | Yes |
| Authentication | Client device to VPN server | VPN gateway to VPN gateway |
| Routing | Client device's routing table must be updated | Routing tables at each network must be updated |

| **Feature** | **Unicast IP** | **Multicast IP** |
|----|----|----|
| Communication | One-to-one | One-to-many |
| Destination | Single IP address | Multicast group address |
| Packet forwarding | All devices on the network ignore the packet except for the destination device | All devices on the network that are members of the multicast group will receive the packet |
| Common uses | Web browsing, file transfer, email | Streaming media, online gaming, software updates |

# How network security works?

- Network security combines multiple layers of defenses at the edge and in the network.

- Each network security layer implements policies and controls.

- Authorized users gain access to network resources, but malicious actors are blocked from carrying out exploits and threats.

**Network security** is a multi-layered approach to protecting a network and its data from unauthorized access, misuse, or disruption. It involves a combination of hardware, software, and policies to safeguard network resources.

Core Principles

- **Defense in Depth:** Employing multiple layers of security controls to protect against various attack vectors.  

- **Least Privilege:** Granting users only the necessary permissions to perform their tasks.  

- **Continuous Monitoring:** Regularly assessing network security posture and identifying potential threats.

**Key Components**

- **Firewalls:** Act as a barrier between the internal network and the external world, filtering incoming and outgoing traffic.  

- **Intrusion Detection and Prevention Systems (IDPS):** Monitor network traffic for malicious activity and can block or alert on suspicious behaviour.  

- **Virtual Private Networks (VPNs):** Create secure encrypted connections over public networks.  

- **Encryption:** Protects data confidentiality by converting it into an unreadable format.  

- **Access Controls:** Restrict network access based on user identity, role, and device.  

- **Security Policies:** Define the organization's security rules and procedures.

How it Works?

1. **Authentication:** Verifies the identity of users and devices attempting to access the network.  

2. **Authorization:** Determines the level of access granted to authenticated users.  

3. **Accounting:** Tracks user activity for auditing and security purposes.  

4. **Monitoring:** Continuously analyses network traffic for suspicious activity.  

5. **Incident Response:** Handles security breaches and minimizes their impact.

By implementing these measures and following best practices, organizations can significantly reduce the risk of cyberattacks and protect their valuable data.

## QnA

Briefly describe the process of network packet capture and analysis. How is it used for troubleshooting network issues?

Network Packet Capture and Analysis

- **Packet capture** involves intercepting and recording data packets as they travel across a network. These packets contain information about the data being transmitted, including source and destination addresses, protocols used, and the actual data itself.  

- **Packet analysis** is the process of examining captured packets to understand network behaviour, identify issues, or extract valuable information. Tools like Wireshark are commonly used for this purpose.  

**How it is used for Troubleshooting**

Packet capture and analysis is a powerful tool for diagnosing network problems. It allows network administrators to:  

- **Identify network congestion:** By analysing packet sizes, inter-packet arrival times, and retransmissions, network bottlenecks can be pinpointed.
- **Detect packet loss:** Missing packets can indicate network issues or application problems. Analysing packet captures can help identify the cause.  
- **Troubleshoot connectivity problems:** By inspecting packet headers, it is possible to determine if packets are reaching their destination and if there are any routing or firewall issues.
- **Investigate security incidents:** Malicious activity can often be detected by examining packet content and patterns.  
- **Optimize network performance:** Analysing traffic patterns can help identify opportunities to improve network efficiency.

In essence, packet capture provides a detailed snapshot of network activity, enabling network professionals to accurately diagnose and resolve a wide range of issues.  

**Would you like to know more about specific tools or techniques for packet capture and analysis?**

Explain the concept of firewalls in TCP/IP networks and their role in network security.

**What is a Firewall?**

A firewall is essentially a security system that acts as a barrier between a trusted internal network and an untrusted external network, typically the internet. It monitors incoming and outgoing network traffic and allows or blocks data packets based on predefined security rules.  

**How Firewalls Work in TCP/IP Networks**

In the context of TCP/IP networks, a firewall operates at different layers of the OSI model, depending on its type:

- **Packet filtering firewalls:** These operate at the network layer (Layer 3) and examine packet headers (source/destination IP addresses, ports) to decide whether to allow or block traffic.
- **Stateful inspection firewalls:** An enhancement over packet filtering, these keep track of network connections (session state) to make more informed decisions.  

- **Application-level firewalls:** They operate at the application layer (Layer 7) and can inspect the content of data packets, providing deeper protection against sophisticated threats.  

**Role of Firewalls in Network Security**

Firewalls play a crucial role in safeguarding network security by:

- **Preventing unauthorized access:** They act as a first line of defense, blocking intruders from entering the network.  

- **Protecting against attacks:** Firewalls can help prevent a variety of attacks, including:

 - Denial-of-service (DoS) attacks
 - Malware infections  
 - Unauthorized access attempts  
 - Data breaches  

- **Enforcing security policies:** They can be configured to implement specific security policies, such as restricting access to certain websites or services.  

- **Monitoring network traffic:** Firewalls can log network activity, which can be used for troubleshooting, security analysis, and compliance purposes.  

**Additional Considerations**

- **Types of Firewalls:** There are various types of firewalls, including hardware, software, and cloud-based solutions, each with its own strengths and weaknesses.  

- **Firewall configuration:** Proper configuration is essential for effective firewall protection. Misconfigured firewalls can leave vulnerabilities.  

- **Firewall limitations:** While firewalls are essential, they are not foolproof. They should be used in conjunction with other security measures for comprehensive protection.  

**In conclusion,** firewalls are a fundamental component of network security. By understanding their principles and proper implementation, organizations can significantly enhance their protection against cyber threats.  

Explain the concept of routing in TCP/IP networks. How do routers use IP addresses to direct data packets?

**Routing in TCP/IP Networks**

**Routing** is the process of selecting the best path for data packets to travel from a source to a destination across multiple interconnected networks. In TCP/IP networks, this crucial function is performed by specialized devices called **routers**.

**How Routers Use IP Addresses**

Routers make intelligent decisions about packet forwarding based on the information contained within the IP header of each packet. The IP header includes two critical pieces of information:

- **Source IP Address:** Identifies the originating host or device.

- **Destination IP Address:** Specifies the destination of the packet.

Here is a breakdown of how routers utilize IP addresses:

1. **Packet Arrival:** A router receives a data packet from an incoming network interface.

2. **IP Header Examination:** The router extracts the destination IP address from the packet's header.

3. **Routing Table Consultation:** The router refers to its routing table, a database that stores information about network destinations and the best paths to reach them.

4. **Path Determination:** The router compares the destination IP address with the entries in its routing table to identify the optimal outgoing interface for the packet.

5. **Packet Forwarding:** The router forwards the packet to the selected outgoing interface, directing it towards the next hop on its journey to the destination.

**Key Points:**

- **IP Addressing:** The unique IP address assigned to each device on a network serves as a fundamental identifier for routers to determine packet forwarding decisions.

- **Routing Tables:** Routers maintain dynamic routing tables that are constantly updated with information about network reachability. This information is obtained through routing protocols like OSPF, RIP, or BGP.

- **Path Selection:** Routers select the best path based on various factors, including network congestion, link costs, and available bandwidth.

- **Packet Switching:** Routers operate on the packet-switching principle, breaking data into smaller packets, routing each independently, and reassembling them at the destination.

**In essence, routers act as intelligent traffic directors within the internet, ensuring that data packets reach their intended destinations efficiently and reliably by leveraging the information contained within IP addresses.**

Compare and contrast different network topologies (bus, star, ring, mesh).

Define the CIA triad (Confidentiality, Integrity, Availability) and its importance in security.

Describe how routing protocols (e.g., BGP, OSPF) work.

Describe the challenges and benefits of cloud-based networking.

Describe the challenges and solutions for securing Internet of Things (IoT) networks.

Describe the challenges and solutions for securing remote access in COVID-19 era.

Describe the different types of network cables and their uses.

Describe the different types of network intrusion detection and prevention systems (IDS/IPS).

Describe the importance of user authentication and authorization mechanisms.

Describe the key considerations when choosing network hardware (routers, switches, firewalls).

Describe the process of designing and implementing a VPN solution.

Describe the process of network capacity planning and forecasting future requirements.

Describe the purpose and functions of a firewall.

Describe your experience with automating network tasks using scripting languages.

Describe your experience with incident response planning and procedures.

Describe your experience with network troubleshooting methodologies (e.g., divide-and-conquer).

Describe your experience with scripting languages commonly used in network automation (Python, Bash).

Describe your experience working in a team environment on network projects.

Describe your experience working with different network vendors and equipment.

Differentiate between LAN, WAN, and MAN.

Discuss the challenges and best practices for secure remote access.

Discuss the challenges and solutions for high-speed network technologies (e.g., fiber optic).

Discuss the challenges and solutions for managing network automation and scripting.

Discuss the challenges and solutions for managing network devices in geographically dispersed locations.

Discuss the challenges and solutions for securing Software-Defined Networks (SDN).

Discuss the configuration and troubleshooting of network firewalls (stateful, deep packet inspection).

Discuss the factors to consider when choosing a network operating system (NOS).

Discuss the impact of artificial intelligence (AI) and machine learning (ML) on network design and security.

Discuss the implementation and configuration of different VLAN types (802.1q, 802.1x).

Discuss the importance of network documentation and best practices for maintaining it.

Discuss the importance of network documentation and best practices for maintaining it.

Discuss the importance of network performance monitoring and optimization techniques.

Discuss the security challenges and considerations for emerging technologies like IoT and 5G.

Discuss the trade-offs between security and performance in network design decisions.

Explain how you would secure a network against a specific type of attack (e.g., DDoS).

Explain the challenges and solutions for managing network deployments in complex environments.

Explain the concept of high availability and its implementation in network design.

Explain the concept of network access control (NAC) and its role in network security.

Explain the concept of network function virtualization (NFV) and its benefits.

Explain the concept of network load balancing and its benefits.

Explain the concept of network telemetry and its potential for network monitoring and troubleshooting.

Explain the concept of network virtualization and its different technologies (VMware, Docker).

Explain the concept of software-defined networking (SDN) and its potential.

Explain the concept of subnetting and its benefits.

Explain the concept of vulnerability management and its role in network security.

Explain the concept of zero-trust security and its implications for network design.

Explain the concepts of network management tools (SNMP, CLI).

Explain the concepts of port security, QoS, and VLAN trunking.

Explain the difference between routing and switching.

Explain the differences between static and dynamic routing protocols.

Explain the differences between various wireless technologies (Wi-Fi, Bluetooth, Cellular).

Explain the different types of firewalls (packet-filtering, stateful, application-level).

Explain the different types of network addressing (static, dynamic, private, public).

Explain the different types of network authentication protocols (RADIUS, TACACS+).

Explain the different types of network management platforms and their functionalities.

Explain the different types of network troubleshooting tools and their functionalities.

Explain the importance of network backup and disaster recovery planning.

Explain the OSI model and its layers.

Explain the purpose of network protocols like TCP/IP, UDP, and BGP.

How do intrusion detection and prevention systems (IDS/IPS) work?

How do you approach ethical hacking and vulnerability assessments?

How do you configure and manage network access points (APs) for secure wireless access?

How do you configure and manage network devices (routers, switches, firewalls)?

How do you design a disaster recovery plan for your network infrastructure?

How do you design a network for multi-tenancy in cloud environments?

How do you design a network for scalability and redundancy?

How do you design a secure wireless network infrastructure?

How do you ensure compliance with regulations related to network security (e.g., HIPAA, PCI-DSS)?

How do you ensure network configuration consistency and compliance with standards?

How do you ensure network uptime and minimize downtime?

How do you handle network troubleshooting situations involving multiple devices and protocols?

How do you implement data loss prevention (DLP) technologies in your network design?

How do you implement network segmentation and its different approaches?

How do you monitor and analyze network logs for security purposes?

How do you stay up-to-date with the latest network engineering tools and technologies?

How do you stay up-to-date with the latest network technologies and trends?

How do you troubleshoot network connectivity issues (e.g., ping, traceroute)?

How firewall works?

How to analyse network traffic?

How to choose Network Firewall? Or What is the selection criteria to buy network firewall?

How to implement Network Firewall?

Present a network design case study you've worked on.

Present a network security case study you've handled successfully.

 What are the basic network security components?

What are the components of Firewall?

What are the different types of network security threats (malware, viruses, phishing)?

What are the ethical considerations when managing network security? 

What are the open-source tools to analyse network traffic?

What are the types of firewalls?

What are VLANs and why are they used?

What are your communication and problem-solving skills?

What IDS and what are the known open source IPS products?

What IPS and what are the known open source IPS products?

What is DHCP protocol and how to implement it?

What is DMZ and how to configure it?

What is DNS and how to implement it?

What is encryption and how does it help secure data?

What is FTP protocol and how to configure FTP server?

What is FTP protocol?

What is FTPS protocol?

What is HTTP protocol?

What is HTTPS protocol?

What is IP and MAC address and what is difference between both?

What is Load Balancer

What is Network Firewall?

What is Network Segmentation?

What is OpenSSL, and how to configure it?

What is Proxy and how to configure it?

What is SFTP protocol?

What is SMB protocol?

What is SMTP protocol?

What is SSL?

What is the difference between IPS and IDS?

What is the difference between SSH, RDP and Telnet?

What is the difference between TCP/IP and OSI Layer network frameworks?

Why are you interested in this specific network design/engineering/security position?

# The End

Network Architecture

# Network Architecture

Assisted security architect to define policies and best practices for NSG.

Assisted security architect to define policies and best practices for Azure Firewall.

Assisted security architect to define policies and best practices for Application Gateway (WAF).

## VNET Peering

**Peering Types:**

- Standard peering

- Gateway transit peering

Can we do VNET peering of VNETs in different subscription of same Tenant?

- Yes, we can do Vnets peering in different subscriptions of the same tenant

- Network Contributor role required in both subscriptions for peering.

- Peered VNETs should have non-overlapping IP address space.

Can we do VNET peering of VNETs in different subscription of different Tenant?

- No, you cannot directly peer VNets in different Azure AD tenants.

- VNet peering is a feature designed to connect VNets within the same Azure AD tenant. It provides a direct, private connection between the VNets, offering benefits like improved performance and reduced costs.

- Why Can't You Peer Across Tenants?

 - **Security and Isolation:** Different tenants represent distinct organizational boundaries. Peering across tenants could potentially compromise security and isolation.

 - **Authentication and Authorization:** Managing access and permissions across different tenants would be complex and introduce additional security challenges.

 - **Network Topology:** Azure's networking infrastructure is designed to operate within tenant boundaries.

- Alternatives for Cross-Tenant Connectivity:

 - **Azure ExpressRoute:** This provides private connectivity between your on-premises infrastructure and Azure, allowing you to establish connections between different tenants by connecting them to a common on-premises network.

 - **Azure VPN Gateway:** Create site-to-site VPN connections between your on-premises network and each tenant's Azure environment, enabling communication between the VNets.

 - **Azure Virtual Network Gateway:** Like site-to-site VPN, but uses Azure's infrastructure for the VPN gateway.

 - **Third-Party Network Virtualization Solutions:** Some third-party providers offer solutions that can help bridge connectivity across different tenants, but these options often come with additional costs and complexities.

Can we do VNET peering of VNETs in different regions or geography?

- Yes, you can peer VNETs across different regions

<https://azure.microsoft.com/en-us/blog/global-vnet-peering-now-generally-available/>

**Hub-spoke topology**

- In this hub and spoke are deployed in separate VNETs connected through peering.

- Segregated management: enables us to apply governance and principle of least privilege. It supports concept of Azure Landing Zone with separation of duties.

- Minimizes direct exposure of Azure resources to the public internet.

- Organizations often operate with regional hub-spoke topologies. Hub-spoke network topologies can be expanded in the future and provide workload isolation.

- It makes the architecture extensible. To accommodate new features or workloads, new spokes can be added instead of redesigning the network topology.

- Azure firewall and DNS can be shared across networks through hub-spoke topology

**How to design network architecture?**
Define policies and best practices for NSG.
Define policies and best practices for Azure Firewall.
Define policies and best practices for Application Gateway (WAF).

**What are the Network Security solutions in Azure?**



**Azure Network Segmentation**

- Azure VNET and subnet can be used for enterprise network segmentation.

- High risk/High value resources can be in isolated VNETs and subnets.

- NSGs can be used for network segmentation, it acts as access control list (ACL), by restricting and controlling the traffic by port, protocol, source, and destination ip address.

- NSG: On NSG follow default rules as "**Deny by default, permit by exception**".

- For complex application architecture use application security groups (ASGs) to simplify complex configuration. Instead of defining policy based on explicit IP addresses in network security groups, ASGs enable you to configure network security as a natural extension of an application's structure, allowing you to group virtual machines and define network security policies based on those groups.

<!-- -->

- Azure Policies:

 - Adaptive network hardening recommendations should be applied on internet facing virtual machines

 - All network ports should be restricted on network security groups associated to your virtual machine

 - Non-internet-facing virtual machines should be protected with network security groups

 - Subnets should be associated with a Network Security Group

 - Internet-facing virtual machines should be protected with Network Security Groups

VNet concepts and best practices: https://docs.microsoft.com/azure/virtual-network/concepts-and-best-practices

Subnet: https://docs.microsoft.com/azure/virtual-network/virtual-network-manage-subnet

NSG: https://docs.microsoft.com/azure/virtual-network/tutorial-filter-network-traffic

ASG: https://docs.microsoft.com/azure/virtual-network/network-security-groups-overview#application-security-groups

**Secure cloud services with network controls (Private Endpoints)**

- Secure cloud services by establishing a private access point for the resources. You should also disable or restrict access from public network when possible.

- Deploy private endpoints for all Azure resources that support the Private Link feature, to establish a private access point for the resources. You should also disable or restrict public network access to services where feasible.

- For certain services, you also have the option to deploy VNet integration for the service where you can restrict the VNET to establish a private access point for the service."

-  

- Understand Azure Private Link: <https://docs.microsoft.com/azure/private-link/private-link-overview>

- Security architecture: <https://docs.microsoft.com/azure/cloud-adoption-framework/organize/cloud-security-architecture>

**Deploy firewall at the edge of enterprise network**

- "Deploy a firewall to perform advanced filtering on network traffic to and from external networks. You can also use firewalls between internal segments to support a segmentation strategy. <u>If required, use custom routes for your subnet to override the system route when you need to force the network traffic to go through a network appliance for security control purpose.</u>

- At a minimum, block known bad IP addresses and high-risk protocols, such as remote management (for example, RDP and SSH) and intranet protocols (for example, SMB and Kerberos).

- Use Azure Firewall to provide fully stateful application layer traffic restriction (such as URL filtering) and/or central management over many enterprise segments or spokes (in a hub/spoke topology).

- If you have a complex network topology, such as a hub/spoke setup, you may need to **create user-defined routes (UDR)** to ensure the traffic goes through the desired route. For example, you have option to use an UDR to redirect egress internet traffic through a specific Azure Firewall or a network virtual appliance."

- **How to deploy Azure Firewall:**

- <https://docs.microsoft.com/azure/firewall/tutorial-firewall-deploy-portal>

- **Virtual network traffic routing:**

- <https://docs.microsoft.com/azure/virtual-network/virtual-networks-udr-overview>

<!-- -->

- **Management ports should be closed on your virtual machines**

- **Management ports of virtual machines should be protected with just-in-time network access control**

- **IP Forwarding on your virtual machine should be disabled**

- **\[Preview\]: All Internet traffic should be routed via your deployed Azure Firewall**

- **Virtual network design considerations and configuration options for Azure Active Directory Domain Services**

- <https://learn.microsoft.com/en-us/azure/active-directory-domain-services/network-considerations>

- **Secured Virtual Hubs and Hub Virtual Networks.**

- **NSG Led the security assessment of azure security services such as network security groups,**

- **Azure Firewall** **Led the security assessment of azure security services such as Azure Firewall**

 - Finding the most efficient way to implement firewall policies across Contoso's multiple Azure regions.

- **Stateful vs Stateless Firewalls**: <https://www.geeksforgeeks.org/stateless-vs-stateful-packet-filtering-firewalls/>



## Scenarios

 

Scenario-1: If Azure VM is in one spoke VNET, in one subscription. and I have configured diagnostics settings to send its resource logs to Log analytics workspace which is in Hub VNET in Second subscription under same tenant, and their Azure Firewall placed between these 2 VNET. Now issue is Log analytics workspace is not received the logs from VMs, what could be the reason, how do I troubleshoot it?

 

There could be several reasons why your Log Analytics workspace is not receiving logs from your Azure VM. Here's how to troubleshoot the issue:

**1. Connectivity Issues:**

- **Network Security Group (NSG) Rules:** Verify that the NSG rules on both the VM's VNet and the Azure Firewall allow outbound traffic to the Log Analytics workspace in the Hub VNet. The outbound traffic should be destined to port 443 (HTTPS).

- **Subnet Routing:** Ensure the VM's subnet has a route defined to reach the Hub VNet where the Log Analytics workspace resides. This route might point to the Azure Firewall as the next hop.

- **Azure Firewall Rules:** Check the Azure Firewall rules. You need a rule that allows traffic from the VM's VNet to the Log Analytics workspace (port 443) in the Hub VNet.

 

**2. Log Analytics Workspace Configuration:**

- **Diagnostics Settings:** Double-check the diagnostics settings on the VM. Ensure they are configured to send the desired logs (e.g., resource logs) to the correct Log Analytics workspace.

- **Workspace Connectivity:** Verify that the Log Analytics workspace itself is functional and accessible. You can test connectivity using tools like Log Analytics agent health checks or PowerShell cmdlets.

 

**3. VM Agent and Logs:**

- **Agent Status:** Check the health of the Log Analytics agent running on the VM. Ensure it's installed, running, and can communicate with the workspace. You can find agent health information in the VM extensions section of the Azure portal.

- **Log Collection:** If the agent is healthy, investigate why specific logs aren't being collected. Refer to the documented log types for the VM resource and ensure they are included in the diagnostics settings.

 

**Troubleshooting Steps:**

Here is a recommended approach for troubleshooting:

1. **Review NSG rules** on the VM's VNet and the Azure Firewall for outbound traffic to port 443.

2. **Verify Subnet routing** on the VM's subnet to ensure it can reach the Log Analytics workspace.

3. **Check Azure Firewall rules** for traffic from the VM's VNet to the Log Analytics workspace.

4. **Confirm diagnostics settings** on the VM are configured correctly for the desired logs and workspace.

5. **Validate Log Analytics workspace health** and connectivity.

6. **Verify Log Analytics agent status** on the VM and ensure it's functional.

7. **Review specific log types** for the VM resource and ensure they are included in diagnostics settings.

 

**Additional Resources:**

- Troubleshoot the Log Analytics VM extension in Azure Monitor: <https://learn.microsoft.com/en-us/azure/azure-monitor/agents/diagnostics-extension-overview>

- Log Analytics agent for Linux VMs: <https://learn.microsoft.com/en-us/azure/azure-monitor/agents/log-analytics-agent>

- Log Analytics agent for Windows VMs: <https://learn.microsoft.com/en-us/azure/azure-monitor/agents/agent-windows>

 

Scenario-2: If there is application is in Microsoft Azure VM, email server is in On-premises, there is Expressroute between on-premises and azure cloud, now applications want to send email through on Prem email servers to users, how will you ensure communication uses TLS1.2 encryption?

Here are the steps to ensure communication uses TLS 1.2 encryption when an application in a Microsoft Azure VM sends email through on-premises email servers with an ExpressRoute connection:

> **1. Enable TLS 1.2 on the Azure VM:** Use Group Policy Objects (GPOs) or registry edits to enable TLS 1.2 for Schannel on the Azure VM.
>
> **2. Enable TLS 1.2 on the on-premises email server:** The specific steps will vary depending on your email server software. Consult your server's documentation for enabling TLS 1.2.
>
> **3. (Optional) Disable insecure TLS versions on both the Azure VM and email server:** Disabling older, insecure TLS versions (e.g., TLS 1.0, TLS 1.1) can further enhance security. Refer to your Azure VM and email server documentation for guidance.
>
> **4. Test email communication:** After making these changes, test email functionality to ensure successful communication with TLS 1.2 encryption.

 

Scenario-3: If you want to copy data to azure cloud through sftp, how will you do it?

Azure Blob Storage now supports SFTP, allowing you to use an SFTP client to securely transfer files. Here's how to copy data to Azure cloud through SFTP:

1. **Enable SFTP support on your Azure Blob storage account.**

2. **Create a local user on your storage account and assign the appropriate permissions.**

3. **Use an SFTP client to connect to your Azure Blob storage using the SFTP server address and your local user credentials.**

4. **Once connected, you can upload or download files between your local machine and Azure Blob storage.**

 

Scenario-4: Client follows to regulatory compliances, now they are offboarding from the Azure Cloud environment. How do you convince client that there is not data of client is present on your Azure Cloud environment?

Here is how you can convince your client that their data is not present on your Azure Cloud environment when they are offboarding for regulatory compliance:

**Transparency and Documentation:**

- **Provide a detailed offboarding plan:** Outline the steps you'll take to remove their data. This includes deleting virtual machines, storage accounts, databases, and any other resources that may contain their data.

- **Data deletion confirmation:** Once deletion is complete, offer a written confirmation that their data has been removed from Azure.

> **Security Measures:**

- **Leverage Azure logging and auditing:** Demonstrate how Azure's logging features track all data access and deletion activities. You can offer to share relevant logs related to their account.

- **Data encryption at rest and in transit:** Reiterate your commitment to data security by highlighting Azure's robust encryption practices. Data is encrypted at rest within storage accounts and in transit when transferred between Azure services.

> **Compliance Certifications:**

- **Highlight relevant Azure compliance certifications:** Many industries have specific data security regulations. Show how Azure meets these regulations through certifications like SOC 2, HIPAA, and GDPR.

**Additional Options:**

- **Offer data transfer assistance:** If the client needs to migrate their data to another platform for compliance reasons, you can assist with the transfer process.

- **Suggest data anonymization:** Propose anonymizing their data before deletion if it can be helpful for future reference without violating regulations.

> **Communication is Key:**

- **Actively listen to their concerns:** Understand their specific regulatory requirements and address them directly.

- **Maintain open communication:** Offer regular updates throughout the offboarding process to keep them informed.

- **Provide clear and concise explanations:** Use non-technical terms whenever possible to ensure they understand the process.

> By following these steps and prioritizing transparency and security, you can build trust with your client during their offboarding process and assure them their data is handled according to their compliance needs.

## Enable TLS 1.2 on webapp hosted on Azure VM

Let us say we have web app hosted on windows servers in Azure VM, we want any communication happens on that web application from internet or on-premises must be on TLS1.2 how to ensure that it communicates only on TLS 1.2 version?

Ensuring TLS 1.2 Communication for Your Azure Web App

**Understanding the Challenge:** To enforce TLS 1.2 communication for your web app hosted on Azure VMs, you'll need to configure both the server and client-side environments to prioritize and, ideally, exclusively support TLS 1.2.

**<span class="mark">Server-Side Configuration (Azure VM)</span>**

1. **Operating System Level:**

 - **Windows Server:**

 - Ensure the operating system is patched with the latest updates to include TLS 1.2 support.

 - Use the regedit tool to modify registry settings for TLS protocol preferences. Refer to Microsoft documentation for specific registry keys and values.

 - Consider using group policies to manage these settings centrally.

 - **.NET Framework:**

 - If using .NET Framework, adjust the ServicePointManager.SecurityProtocol property in your application code to prioritize TLS 1.2.

 - Example: ServicePointManager.SecurityProtocol = SecurityProtocolType.Tls12 \| SecurityProtocolType.Tls11 \| SecurityProtocolType.Tls; \`\`\`

<!-- -->

2. **Web Server Configuration:**

 - **IIS:**

 - Configure IIS to require TLS 1.2 and disable older protocols. This can be done through the IIS Manager interface or using PowerShell cmdlets.

 - Ensure the SSL certificate supports TLS 1.2.

3. **Application Level:**

 - Review your application code and libraries for any hardcoded TLS protocol preferences. Ensure they are aligned with TLS 1.2.

**<span class="mark">Client-Side Configuration</span>**

1. **Browser Settings:**

 - Encourage users to update their browsers to the latest versions, which typically support TLS 1.2 by default.

 - Some browsers might require specific settings to be enabled.

2. **Application Clients:**

 - If your application has custom clients (e.g., desktop applications, mobile apps), ensure they are configured to support TLS 1.2. This might involve code changes or updates to libraries.

**<span class="mark">Additional Considerations</span>**

- **Testing:** Thoroughly test your web application with different browsers, operating systems, and clients to ensure compatibility and security.

- **Monitoring:** Implement monitoring to detect and address any issues related to TLS 1.2 enforcement.

- **Azure App Service:** If you are using Azure App Service, it often provides built-in options to configure minimum TLS version.

- **Load Balancers:** If using Azure Load Balancers, ensure they are configured to support TLS 1.2.

- **Certificate Management:** Use strong, up-to-date SSL certificates that support TLS 1.2.

**<span class="mark">Example PowerShell Script for IIS Configuration</span>**

PowerShell

\# Get a reference to the site

\$site = Get-Website -Name "YourWebsiteName"

\# Disable TLS 1.0 and TLS 1.1

\$binding = \$site.bindings \| Where-Object {\$\_.protocol -eq "https"}

\$binding.securityBinding.enabledProtocols = \[System.Net.SecurityProtocolType\]::Tls12

\$site.bindings = \$binding

\$site \| Set-Website

By following these guidelines and carefully configuring both server and client-side environments, you can effectively enforce TLS 1.2 communication for your Azure web application.

## Design Virtual Network

Design a secure virtual network for an application in Azure.

Secure Virtual Network Design for an Azure Application

Here is a secure virtual network design for an application deployed on Azure Virtual Machines (VMs):

**Network Components:**

- **Virtual Network (VNet):** Create a VNet to isolate your application resources from the public internet. This provides a private address space for your VMs and other resources.

- **Subnets:** Divide your VNet into subnets based on functionality. Here's a common approach:

 - **Public Subnet:** Place your web server VMs in a public subnet to allow inbound traffic from the internet for functionalities like accessing your website.

 - **Private Subnet:** Deploy your application logic VMs and database VMs in a private subnet. Restrict inbound traffic to this subnet for enhanced security. Only authorized resources, like a jump box VM with stricter access controls, should have access.

- **Network Security Groups (NSGs):** Associate NSGs with each subnet to control inbound and outbound traffic flow. Define granular access rules based on source IP address, port number, and protocol. Here's an example:

 - **Public Subnet NSG:** Allow inbound traffic on port 80 (HTTP) and 443 (HTTPS) for web server access. Block all other inbound traffic.

 - **Private Subnet NSG:** Deny all inbound traffic by default. Only allow specific inbound traffic from the public subnet (e.g., for database access) or from a jump box VM with restricted access for management purposes.

**Additional Security Measures:**

- **Azure Firewall/Web Application Firewall (WAF):** Deploy an Azure Firewall or WAF in front of your web server VMs in the public subnet. This provides an additional layer of security by filtering malicious traffic, preventing DDoS attacks, and blocking common web application vulnerabilities.

- **Just-In-Time (JIT) Access:** Configure Azure Security Center to enable JIT access for jump box VMs in the private subnet. This restricts RDP/SSH access and requires manual approval before access is granted, reducing the attack surface.

- **Bastion Host:** Consider deploying a Bastion host as a secure entry point to your virtual network. This eliminates the need to expose jump box VMs directly to the internet, further enhancing security.

**Best Practices:**

- **Use strong passwords and implement Multi-Factor Authentication (MFA) for all administrative accounts.**

- **Keep software on your VMs updated with the latest security patches.**

- **Monitor your virtual network for suspicious activity using Azure Security Center.**

- **Implement a backup and disaster recovery plan for your application.**

**Benefits of this Design:**

- **Isolation:** Separates application resources from the public internet, reducing the attack surface.

- **Granular Access Control:** NSGs provide fine-grained control over traffic flow, minimizing unauthorized access.

- **Layered Security:** Azure Firewall/WAF and JIT access offer additional protection for critical resources.

Remember, this is a general design, and specific configurations may vary depending on your application's unique needs.

## Network Security Architecture in Azure

- DDoS Protection
- Detect and disable insecure services and protocols
- Intrusion detection and prevention
- Network segmentation boundaries
- Only SSL connection should be enabled on Database servers
- PaaS Services public access should be disallowed
- PaaS Services should have firewall enabled
- PaaS Services should use secure connection (HTTPS)
- Perimeter protection with firewall
- Use private link for all PaaS Services
- VPN connections should use Azure Active Directory for authentication
- Web Application Firewall



## VM security

Configure update management

Create VM templates

Define privileged access device strategy

Deploy and configure Windows Defender

Deploy disk encryption

Deploy Privileged access workstations

Enable and secure remote access management

Enable Endpoint protection

Explore Microsoft Defender for Cloud recommendations

Secure Azure workload with Azure Security Benchmark

## Container security

Configure AKS networking

Configure Azure container instance security

Deploy AKS storage

Enable Azure container registry authentication

Explore Azure Container registry

Implement AKS architecture

Manage access to AKS through Azure RBAC

Review Azure Kubernetes services

Secure authentication to AKS with Active Directory

## Network Segmentation

**Azure Network Segmentation** involves dividing a virtual network into smaller isolated segments, known as subnets, to enhance security and control traffic flow.

Key Components

- **Virtual Networks (VNETs):** Logical isolation of network resources.

- **Subnets:** Divisions within a VNET for further segmentation.

- **Network Security Groups (NSGs):** Act as firewalls, controlling inbound and outbound traffic.

- **Application Security Groups (ASGs):** Group virtual machines based on application logic for simplified security policy management.

Core Concepts

- **Isolation:** Segmenting high-value resources into isolated VNETs and subnets.

- **Access control:** Using NSGs to define granular network security policies.

- **Security groups:** Simplifying security management with ASGs.

- **Default denies:** Implementing a "deny by default" principle for enhanced security.

In essence, Azure Network Segmentation provides a robust framework for protecting resources and controlling network traffic by creating isolated segments and implementing granular security policies.

Azure Policies for network segmentation

- \[Preview\]: All Internet traffic should be routed via your deployed Azure Firewall

- Adaptive network hardening recommendations should be applied on internet facing virtual machines

- All network ports should be restricted on network security groups associated to your virtual machine

- Internet-facing virtual machines should be protected with Network Security Groups

- IP Forwarding on your virtual machine should be disabled

- Management ports of virtual machines should be protected with just-in-time network access control

- Management ports should be closed on your virtual machines

- Non-internet-facing virtual machines should be protected with network security groups

- Subnets should be associated with a Network Security Group

VNet concepts and best practices:

<https://docs.microsoft.com/azure/virtual-network/concepts-and-best-practices>

Subnet:

<https://docs.microsoft.com/azure/virtual-network/virtual-network-manage-subnet>

NSG:

<https://docs.microsoft.com/azure/virtual-network/tutorial-filter-network-traffic>

ASG:

<https://docs.microsoft.com/azure/virtual-network/network-security-groups-overview#application-security-groups>

Security architecture:

<https://docs.microsoft.com/azure/cloud-adoption-framework/organize/cloud-security-architecture>

## Implement advanced network security

- secure the connectivity of hybrid networks

- create and configure Azure Firewall

- create and configure Azure Firewall Manager

- create and configure Azure Application Gateway

- create and configure Azure Front Door

- create and configure Web Application Firewall (WAF)

- configure a resource firewall, including storage account, Azure SQL, Azure Key Vault, or Azure App Service

- configure network isolation for Web Apps and Azure Functions

- implement Azure Service Endpoints

- implement Azure Private Endpoints, including integrating with other services

- implement Azure Private Links

- implement Azure DDoS Protection



## Network Routing

UDR

Route Tables

## Network Watcher

Network watcher monitors and diagnoses network issues by using scenario-based analysis.
