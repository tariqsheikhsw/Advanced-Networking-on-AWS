### ANS-C01 Q/A

# VGW and IGW 

IGW : Internet  
VGW : VPN Consolidation (S2S VPNs aggregation) : Branch Office

# Using TGW instead of VGW (limitations) 
VGW vs TGW 
- A VGW is used to connect an Amazon VPC to a remote network, typically an on-premises network, via VPN or Direct Connect
- A TGW is used to connect multiple VPCs and on-premises networks via a centralized hub, creating a star (hub-and-spoke) network topology.

# Summarization , SuperNetting 
Route Aggregation 

# Can VGWs used to peer VPCs ?
Public internet , not recommended 
Transit Gateway or VPC peering recommended 

# Connect 2 VPCs in 2 different Regions 
VPC peering , Transit Gateway 

# VGW is mandatory for DX connection ?
No
DX with VGW/DXGW/TGW
- Direct Connect with Virtual Private Gateway (VGW)
- Direct Connect with Direct Connect Gateway
- Direct Connect with Transit Gateway (TGW)






