## Network security

MDC needs to collect data for at least 30 days to provide recommendations for adaptive network hardening.
Adaptive network hardening provides recommendations to further harden the NSG rules.
While remediating the recommendation for Adaptive network hardening, we need to enforce rules, those enforced rules are added in NSG (may be attached to subnet/NIC) which is protecting the VM.
All Internet traffic should be routed via your deployed Azure Firewall
All network ports should be restricted on network security groups associated to your VMs
API Management services should use a VNET
App Configuration should use private link
Authorized IP ranges should be defined on Kubernetes Services
Azure Cache for Redis should reside within a VNET
Azure Cosmos DB accounts should have firewall rules
Azure DDoS Protection Standard should be enabled
Azure Defender for DNS should be enabled
Azure Event Grid domains should use private link
Azure Event Grid topics should use private link
Azure Key Vault should disable public network access
Azure Machine Learning workspaces should use private link
Azure SignalR Service should use private link
Azure Spring Cloud should use network injection
Cognitive Services accounts should disable public network access
Cognitive Services accounts should restrict network access
Container registries should not allow unrestricted network access
Container registries should use private link
Internet-facing VMss should be protected with Network Security Groups"
IP Forwarding on your VMs should be disabled
Latest TLS version should be used in your API App
Latest TLS version should be used in your Function App
Latest TLS version should be used in your Web App
Management ports of VMss should be protected with just-in-time network access control
Management ports should be closed on your VMss
Non-internet-facing VMss should be protected with network security groups
Private endpoint connections on Azure SQL Database should be enabled
Private endpoint should be configured for Key Vault
Private endpoint should be enabled for MariaDB servers
Private endpoint should be enabled for MySQL servers
Private endpoint should be enabled for PostgreSQL servers
Public network access on Azure SQL Database should be disabled
Public network access should be disabled for MariaDB servers"
Public network access should be disabled for MySQL servers
Public network access should be disabled for PostgreSQL servers
Storage account public access should be disallowed
Storage accounts should restrict network access
Storage accounts should restrict network access using VNET rules
Storage accounts should use private link
Subnets should be associated with a Network Security Group
VM Image Builder templates should use private link
Web Application Firewall (WAF) should be enabled for Application Gateway
Web Application Firewall (WAF) should be enabled for Azure Front Door Service
