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

# Two VPCs connected by VPC peering and VGW , which one takes preference
preference for routing traffic depends on the specific route tables configured in the VPCs

# VGW is transitive ?
by default, no . can be done though ( BGP Route Reflector : to break the rules)

# VGW supports 
IKE and IKEv2 (both)

# S3 Gateway Endpoint , Interface EndPoint 
Interface EndPoint : Private link, VPN , DX etc. 

# VGW connecting to multiple on-prem sites ?
Each VPN connection or Direct Connect connection is associated with the same VGW in AWS.
- Branch Office 1: Connects to AWS via VPN Connection 1.
- Branch Office 2: Connects to AWS via VPN Connection 2.
- HQ Office: Connects to AWS via Direct Connect Connection 1.

   
# Jumbo Frame , Regular MTU 1500 
- Jumbo Frames : can use b/w vpcs in same region or ec2 instances
- Jumbo Frames : can't just if going to internet
- TCP/UDP : is controlled by Application, JF is agnostic of TCP/UDP traffic (retransmissions)
- Broadcast limit : 1000 (EC2 or machines) per subnet
- We don't use JF for voice/video traffic (RTP) etc.


# VXLAN
- Layer3 (used to encapsulate Layer2 packets)
- Underlay
- VXLAN extends Layer 2 networks over Layer 3 infrastructure, making it a technology that functions at both the Data Link and Network layers of the OSI model.

# Crypto 
- Public key / Private Key
- Confidentiality / Integrity (difference in public private key used for encrypt or decrypt etc.)
- Confidentiality : Public key encrypts , Private key decrypts
- Integrity : Private key encrypts, Public key decrypts

# SD-WAN (CISCO)
- Orchestration Layer/Control Plane
- Control Plane: vSmart
- Data Plane: vEdge/cEdge Routers
- Management Plane: vManage

# AWS Transit Gateway
- VPCs are not transitive (VPC peering) , unless you use Transit Gateway or CloudHub
- VGW : one vpc , edge router (VPN, DX)
- TGW : multiple vpcs across regions, edge case also 
- TGW (hub and spoke) vs VPC Peering (fully meshed)
- TGW (think of BGP Route Reflector)
- Transit Gateway Connect is a powerful feature for organizations looking to integrate their on-premises SD-WAN solutions with AWS
- CloudWAN
- Use Cases: Use Transit Gateway Connect if your primary goal is to extend SD-WAN capabilities into AWS. Choose CloudWAN if you need a unified management solution for a diverse and complex network spanning multiple environments.
- AWS Transit Gateway is a regional resource.
- Peer 2 transit gateways in 2 VPCs (Peer Connection) 


# Multicast Routing & Network ACL (NACL)
- Multicast over GRE tunnel (b/w AWS and Azure Cloud etc.)

# VPN 
- Transit Gateway with Global Accelerator (not with VGW)
- Major VPN provider , can use single core only (system with 128 cores) - Application works better with high cpu limit // (May be in past need to check support)
- IPSec vs TLS
- VGW only has S2S VPN support
- FQDN/IP

# DX 
- Cloud on RAMP : SASE solution
- CloudOnRAMP vs DX
- can we have 2 direct connect gateways in 2 regions : YES
- DX gateway is Global resource
- TGW infront of DXGW


# MISC
- Transit Gateway Connection

  

