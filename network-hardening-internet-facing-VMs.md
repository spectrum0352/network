#Adaptive network hardening on internet facing VMs

Adaptive Network Hardening provides a more granular recommendation based on the traffic it has analysed. 
This is add-on feature to NSG. For instance, we have VM in azure we use as Jump Box to administer Azure assets.
We can access jump box on RDP/3389, we allowed traffic from 10.0.0.0/24 subnet. 
Adaptive network hardening will analyse this traffic and make recommendations to reduce the scope of subnet.
