# Advanced-Networking-on-AWS
ANS-C01 Notes

# Exam Prerequisites

Before you take this exam, AWS recommends you have:

- Professional experience using AWS technology, AWS security best practices, AWS storage options and their underlying consistency models, and AWS networking nuances and how they relate to the integration of AWS services.
- Knowledge of advanced networking architectures and interconnectivity options [e.g., IP VPN, multiprotocol label switching (MPLS), virtual private network service (VPN)].
- Familiarity with the development of automation scripts and tools. This should include the design, implementation, and optimization of the following: Routing architectures (including static and dynamic); multi-region solutions for a global enterprise; highly available connectivity solutions (e.g., AWS Direct Connect, VPN).
- Knowledge of CIDR and sub-netting (IPv4 and IPv6); IPv6 transition challenges; and generic solutions for network security features, including AWS WAF, intrusion detection systems (IDS), intrusion prevention systems (IPS), DDoS protection, and economic denial of service/sustainability (EDoS).

# Domain 	% of Exam
Domain 1: Network Design 	30%  
Domain 2: Network Implementation 	26%  
Domain 3: Network Management and Operation 	20%  
Domain 4: Network Security, Compliance, and Governance 	24%  

### Domain 1: Network Design

1.1: Design a solution that incorporates edge network services to optimize user performance and traffic management for global architectures.  
• Design patterns for the usage of content distribution networks (for example, Amazon CloudFront)  
• Design patterns for global traffic management (for example, AWS Global Accelerator)  
• Integration patterns for content distribution networks and global traffic management with other services (for example, Elastic Load Balancing, Amazon API Gateway)  

1.2: Design DNS solutions that meet public, private, and hybrid requirements.  
• DNS protocol (for example, DNS records, timers, DNSSEC, DNS delegation, zones)  
• DNS logging and monitoring  
• Amazon Route 53 features (for example, alias records, traffic policies, resolvers, health checks)  
• Integration of Route 53 with other AWS networking services (for example, Amazon VPC)  
• Integration of Route 53 with hybrid, multi-account, and multi-Region options  
• Domain registration  

1.3: Design solutions that integrate load balancing to meet high availability, scalability, and security requirements.  
• How load balancing works at layer 3, layer 4, and layer 7 of the OSI model  
• Different types of load balancers and how they meet requirements for network design, high availability, and security  
• Connectivity patterns that apply to load balancing based on the use case (for example, internal load balancers, external load balancers)  
• Scaling factors for load balancers  
• Integrations of load balancers and other AWS services (for example, Global Accelerator, CloudFront, AWS WAF, Route 53, Amazon Elastic Kubernetes Service [Amazon EKS], AWS Certificate Manager [ACM])  
• Configuration options for load balancers (for example, proxy protocol, cross-zone load balancing, session affinity [sticky sessions], routing algorithms)  
• Configuration options for load balancer target groups (for example, TCP, GENEVE, IP compared with instance)  
• AWS Load Balancer Controller for Kubernetes clusters  
• Considerations for encryption and authentication with load balancers (for example, TLS termination, TLS passthrough)  

1.4: Define logging and monitoring requirements across AWS and hybrid networks.  
• Amazon CloudWatch metrics, agents, logs, alarms, dashboards, and insights in AWS architectures to provide visibility  
• AWS Transit Gateway Network Manager in architectures to provide visibility  
• VPC Reachability Analyzer in architectures to provide visibility  
• Flow logs and traffic mirroring in architecture to provide visibility  
• Access logging (for example, load balancers, CloudFront)  

1.5: Design a routing strategy and connectivity architecture between on-premises networks and the AWS Cloud.  
• Routing fundamentals (for example, dynamic compared with static, BGP)  
• Layer 1 and layer 2 concepts for physical interconnects (for example, VLAN, link aggregation group [LAG], optics, jumbo frames)  
• Encapsulation and encryption technologies (for example, Generic Routing Encapsulation [GRE], IPsec)  
• Resource sharing across AWS accounts  
• Overlay networks  

1.6: Design a routing strategy and connectivity architecture that include multiple AWS  
accounts, AWS Regions, and VPCs to support different connectivity patterns.  
• Different connectivity patterns and use cases (for example, VPC peering, Transit Gateway, AWS PrivateLink)  
• Capabilities and advantages of VPC sharing  
• IP subnets and solutions accounting for IP address overlaps  

### Domain 2: Network Implementation  
2.1: Implement routing and connectivity between on-premises networks and the AWS Cloud.  
• Routing protocols (for example, static, dynamic)  
• VPNs (for example, security, accelerated VPN)  
• Layer 1 and types of hardware to use (for example, Letter of Authorization [LOA] documents, colocation facilities, Direct Connect)  
• Layer 2 and layer 3 (for example, VLANs, IP addressing, gateways, routing, switching)  
• Traffic management and SD-WAN (for example, Transit Gateway Connect)  
• DNS (for example, conditional forwarding, hosted zones, resolvers)  
• Security appliances (for example, firewalls)  
• Load balancing (for example, layer 4 compared with layer 7, reverse proxies, layer 3)  
• Infrastructure automation  
• AWS Organizations and AWS Resource Access Manager (AWS RAM) (for example, multiaccount Transit Gateway, Direct Connect, Amazon VPC, Route 53)  
• Test connectivity (for example, Route Analyzer, Reachability Analyzer)  
• Networking services of VPCs  

2.2: Implement routing and connectivity across multiple AWS accounts, Regions, and VPCs to support different connectivity patterns.  

• Inter-VPC and multi-account connectivity (for example, VPC peering, Transit Gateway, VPN, third-party vendors, SD-WAN, multiprotocol label switching [MPLS])  
• Private application connectivity (for example, PrivateLink)  
• Methods of expanding AWS networking connectivity (for example, Organizations, AWS RAM)  
• Host and service name resolution for applications and clients (for example, DNS)  
• Infrastructure automation  
• Authentication and authorization (for example, SAML, Active Directory)  
• Security (for example, security groups, network ACLs, AWS Network Firewall)  
• Test connectivity (for example, Route Analyzer, Reachability Analyzer, tooling)  

2.3: Implement complex hybrid and multi-account DNS architectures.  
• When to use private hosted zones and public hosted zones  
• Methods to alter traffic management (for example, based on latency, geography, weighting)  
• DNS delegation and forwarding (for example, conditional forwarding)  
• Different DNS record types (for example, A, AAAA, TXT, pointer records, alias records)  
• DNSSEC  
• How to share DNS services between accounts (for example, AWS RAM)  
• Requirements and implementation options for outbound and inbound endpoints  

2.4: Automate and configure network infrastructure.  
• Infrastructure as code (IaC) (for example, AWS Cloud Development Kit [AWS CDK], AWS CloudFormation, AWS CLI, AWS SDK, APIs)  
• Event-driven network automation  
• Common problems of using hardcoded instructions in IaC templates when provisioning cloud networking resources  

### Domain 3: Network Management and Operations

3.1: Maintain routing and connectivity on AWS and hybrid networks  

• Industry-standard routing protocols that are used in AWS hybrid networks (for example, BGP over Direct Connect)  
• Connectivity methods for AWS and hybrid networks (for example, Direct Connect gateway, Transit Gateway, VIFs)  
• How limits and quotas affect AWS networking services (for example, bandwidth limits, route limits)  
• Available private and public access methods for custom services (for example, PrivateLink, VPC peering)  
• Available inter-Regional and intra-Regional communication patterns  

3.2: Monitor and analyze network traffic to troubleshoot and optimize connectivity patterns.  

• Network performance metrics and reachability constraints (for example, routing, packet size)  
• Appropriate logs and metrics to assess network performance and reachability issues (for example, packet loss)  
• Tools to collect and analyze logs and metrics (for example, CloudWatch, VPC Flow Logs, VPC Traffic Mirroring)  
• Tools to analyze routing patterns and issues (for example, Reachability Analyzer, Transit Gateway Network Manager)  

3.3: Optimize AWS networks for performance, reliability, and cost-effectiveness.  

• Situations in which a VPC peer or a transit gateway are appropriate  
• Different methods to reduce bandwidth utilization (for example, unicast compared with multicast, CloudFront)  
• Cost-effective connectivity options for data transfer between a VPC and on-premises environments  
• Different types of network interfaces on AWS  
• High-availability features in Route 53 (for example, DNS load balancing using health checks with latency and weighted record sets)  

• Availability of options from Route 53 that provide reliability  
• Load balancing and traffic distribution patterns  
• VPC subnet optimization  
• Frame size optimization for bandwidth across different connection types  

### Domain 4: Network Security, Compliance, and Governance  
4.1: Implement and maintain network features to meet security and compliance needs and requirements.  
• Different threat models based on application architecture  
• Common security threats  
• Mechanisms to secure different application flows  
• AWS network architecture that meets security and compliance requirements  

4.2: Validate and audit security by using network monitoring and logging services.  
• Network monitoring and logging services that are available in AWS (for example, CloudWatch, AWS CloudTrail, VPC Traffic Mirroring, VPC Flow Logs, Transit Gateway Network Manager)  
• Alert mechanisms (for example, CloudWatch alarms)  
• Log creation in different AWS services (for example, VPC flow logs, load balancer access logs, CloudFront access logs)  
• Log delivery mechanisms (for example, Amazon Kinesis, Route 53, CloudWatch)  
• Mechanisms to audit network security configurations (for example, security groups, AWS Firewall Manager, AWS Trusted Advisor)  

4.3: Implement and maintain confidentiality of data and communications of the network.  
• Network encryption options that are available on AWS  
• VPN connectivity over Direct Connect  
• Encryption methods for data in transit (for example, IPsec)  
• Network encryption under the AWS shared responsibility model  
• Security methods for DNS communications (for example, DNSSEC)  


###  List of Topics :

### Load Balancers


   •  Configuring Load Balancers (Know Load Balancer Target groups including Cross Zone Load Balancing (the target group attributes selection for Cross-zone load balancing must be set as on)and Registering Targets)  
   •  ALB Listeners are processes that check for connection requests, using the protocol and port that you configure  
   •  ALB Target Groups are definitely an area to review for this exam. They are used to route requests to one or more registered registered targets. These are very useful in configuring ALBs  
   • Learn how to set up encryption end to end for a Load Balancer, configuring the certificates, listeners and target groups  
   •  For Sticky Sessions, one must update the Target Group attributes and set the Stickiness type to select a Load balancer generated cookie  
   •  Study that when wanting to use a unique random session key to provide additional safeguards against the eavesdropping of encrypted data for a Load Balancer, this will involve the Perfect Forward Secrecy  
   •  With respect to Network Load Balancer or a Application Load Balancer, a security policy update involves the their listeners. This might involve creating an ALB https listener or an NLB TLS listener  
   •  Understand the actual use of Gateway Load Balancers which enable you to deploy, scale, and manage virtual appliances, such as firewalls, intrusion detection and prevention systems, and deep packet inspection systems  
    • Path-based and host-based routing capabilities can only be handled by Application Load Balancers (not Network Load Balancers)  
    •  A load balancer should be configured to use TCP so the SSL/TLS connection can be passed through and terminated to the underlying EC2 instances. This ensures end to end encryption  
    • SSL/TLS automatically terminates  
    

### Transit Gateways

   • Understand the steps on how to share resources using RAM across different accounts for a Transit Gateway  
   • Understand Multicast Groups, especially with respect to IGMP(Internet Group Management Protocol) Multicast and static (API-based) sources. IGMP Multicast groups utilize UDP only and can be managed dynamically managed and members can send and receive data. Static groups utilize TCP and UDP but members can only receive traffic. If you are (Also see AWS re:Invent 2020: Using AWS Transit Gateway for your multicast workloads )  
   • Remember non-nitro instance cannot be a Multicast sender  
   • Know some of the Transit Gateway design best practices including that traffic might drop on a network if you have a Transit Gateway and a network appliance in the same subnet(or one of the Transit Gateway attachments).  
   • You should know that Transit VPC is never a good choice as Transit Gateway is a managed service that scales elastically  
   • BGP Routing can be helpful in configuring a global network with Direct Connect and Transit Gateway.  
   See https://aws.amazon.com/blogs/networking-and-content-delivery/building-a-global-network-using-aws-transit-gateway-inter-region-peering/
  

### Network Analysis Services:

   • Reachability Analyzer is a configuration analysis tool that enables you to perform connectivity testing between a source resource and a destination resource in your virtual private clouds (VPCs). If the destination is not reachable, Reachability Analyzer identifies the blocking component. The source and destination resources must be in the same Region. (supports only resources with an IPv4 address). Transit gateway Connect attachments are not supported. Reachability Analyzer can find paths through at most two transit gateway route tables. To analyze paths through additional transit gateway route tables, use Route Analyzer.  
   •  The Reachability Analyzer can also be used in automating connectivity checks that are triggered by security group changes. See Automating connectivity assessments with VPC Reachability Analyzer   
   • Route Analyzer can perform an analysis of the routes in your transit gateway route tables. The source and destination must be transit gateway attachments. The Route Analyzer analyzes the routing path between a specified source and destination, and returns information about the connectivity between components. (IPv4 or IPv6). The Route Analyzer analyzes routes in transit gateway route tables only. It does not analyze routes in VPC route tables or in your customer gateway devices.  
  •  Network Access Analyzer identifies unintended network access to your resources on AWS. You can use it to specify your network access requirements and identify potential network paths that do not meet your specified requirements. Possibly ensuring that production and development VPCs are isolated or which resources can be accessed by internet gateways.  
  • Transit Gateway Network Analyzer provides a single global view of your private network.  

### Miscellaneous Topics:

  • AWS Global Accelerator is a networking service that provides static public IPs to act as a fixed entry point helping those devices that do not have access to dns resolution
  • The Route 53 Resolver DNS Firewall has some configurations such as firewall-fail-open Route53 configuration to know the concept of favoring availability over security  
  • Know that access to SQS from ECS or EC2 does not require any networking tasks such as route table configuration but simply the right IAM role, interface endpoint and security group  
  • If you had an application (with a complex networking design) which was going into production in a matter of days and it needed to be integrated with a new webservice. It might be connecting to the web service via an interface VPC endpoint  
  • Possibly you might have a customer that has a Direct Connect connection to Region A and Region B. There might be a Transit Gateway A in Region A that the on-premises location has access to and a VPC B in Region B connected to a Transit Gateway B. There could be a Direct Connect Gateway. Explore the ways to connect the on-premises location to VPC B. One could connect Transit Gateway A to Transit Gateway B or one could connect the customer’s Direct Connect Gateway to Transit Gateway B directly for connectivity to VPC B.  
  • Understand that one way to capture traffic between Kubernetes Nodes could be to have the node flow log data sent to S3 and have the data queried with Athena. See Using VPC Flow Logs to capture and query EKS network communications  
  • Flow logs delivered to OpenSearch (Real time application monitoring) with Kinesis Firehose is faster than Flow Logs simply to S3. See Stream VPC flow logs to Amazon OpenSearch Service via Amazon Kinesis Data Firehose  
  • Review Monitoring Direct Connect with CloudWatch for monitoring performance issues with respect to both the Direct Connect physical connection and virtual interfaces  
 • AWS Direct Connect Connection metrics:  
- ConnectionPpsEgress — measures the packet rate for outbound data from the AWS side of the connection ) (Packets per second)  
- ConnectionPpsIngress — measures the packet rate for inbound data to the AWS side of the connection (Packets per second)  
- ConnectionBpsEgress — measures the bitrate(bits/second) for outbound data (Bits per second)  
- ConnectionBpsIngress — measures the bitrate(bits/second) for inbound data (Bits per second)  
• AWS Direct Connect virtual interface metrics:  
- VirtualInterfaceBpsEgress, VirtualInterfaceBpsIngress, VirtualInterfacePpsEgress, VirtualInterfacePpsIngress  

• AWS Network Firewall is a stateful, managed, network firewall and intrusion detection and prevention service for your virtual private cloud(VPC).   
Network Firewall can perform deep packet inspection on traffic entering or leaving your VPC  
• Route 53 Resolver DNS Firewall provides protection for outbound DNS requests from your VPC and help prevent DNS exfiltration of your data.  
• Look into NAT gateway troubleshooting , including if the connection drops after 350 seconds, you can initiate more traffic over the connection or enable the TCP keepalive on the instance with a value less than 350 seconds. Might be useful for long running database queries.  
• When Configuring a Transit VIF(Virtual Interface) to enable IPv6 you go under Additional settings, choose IPV6 and the peer IPv6 addresses are automatically assigned from Amazon’s pool of IPv6 addresses.  
• When enabling outbound IPv6 traffic using an egress-only internet gateway you will:  
    - Create the egress-only internet gateway  
    - Create a custom route table (adding a route that sends traffic to the gateway and then associate it with your subnet)  
• Review configuring a public VIF for IPv6  
• PrivateLink can be used when creating a Network Load Balancer for the application in your VPC, create a VPC endpoint service configuration pointing to that load balancer. The service consumer will create an interface endpoint to the service.  
• Review VPC Flow logs at a high level  
• If you also want a breakdown on the different areas to study for the exam you should have a look at 10 study areas for the AWS Certified Advanced Networking — Specialty exam .  

### Practice questions  

Practice questions that involve the following topics can be given less focus in my opinion with respect to the current exam content. They may have been relevant previously but I don’t think so now. However, one could place the caveat that this material can still be beneficial if still on the AWS Certified Advanced Networking — Specialty (ANS-C01) Exam Guide They do provide content that is probably part of the networking specialty but maybe not as important now. These include questions involving:  

    • MED vs AS PATH VPN preferences  
    • WaveLength Zones or Outposts  
    • DNS addressing, TimeSync Service or ENA Linux Kernel Drivers  
    • Port hours or Data Transfer Out  
    • Squid Proxy  
    • Match Viewer  
    • Url of retrieving Metadata http://169.254.169.254/latest/  
    • email-smtp.ap-southeast-2.amazonaws.com:587  
    • Transparent Data Encryption(TDE)  
    • MINIMUM_IP_TARGET  
    • Fragmented TCP Packets  
    • Domain Name System Security Extensions (DNSSEC)  
    • Nat Gateway charges  
    • Network Time Protocol (NTP)/Amazon Time Sync Service  
    • Cloud Map  
    • Bidirectional Forwarding Detection (BFD)  

As well, one could take note that some distractor or eliminatory words can be utilized to try and eliminate options from consideration to improve your chances of selecting the right response. These include:  

    • cloud-init  
    • VPC Proxy (proxy in general)  
    • Transit VPC  
    • OPworks Chef  
    • Mention of VPN usually  
    • Cron job  

### VPC 

### Extension of existing VPC by using a Secondary CIDR blocks
To extend the IPv4 address range of your VPC, see Associating a secondary IPv4 CIDR block with your VPC. Make sure that you follow the CIDR block association restrictions.

https://aws.amazon.com/premiumsupport/knowledge-center/vpc-ip-address-range/

- Associating a secondary IPv4 CIDR block with your VPC [https://docs.aws.amazon.com/vpc/latest/userguide/working-with-vpcs.html#add-ipv4-cidr]

- CIDR block association restrictions [https://docs.aws.amazon.com/vpc/latest/userguide/configure-your-vpc.html#add-cidr-block-restrictions]



### Security Groups vs NACLs 

- Security Group : stateful
- Network ACL : stateless 

### VPC Flow Logs

### DHCP Option Sets 

### VPC Peering and its limitations 

### VPC Peering vs Transit Gateway 
UseCases

### Placement Groups 

- Cluster Placement Groups 
- Partiion Placement Groups 

### VPC Endpoints 

- Gateway VPC Endpoints 
- Interface VPC Endpoints 

### Private Link 

### VPC Network Access Analyzer 

### VPC Network access analyzer vs Reachability Analyzer

### Transit Gateway 
usecases 

### Transit Gateway integration with Direct Connect Gateway 

### NAT Gateways vs NAT Instances 

### VPN (Virtual Private Network) vs Direct Connect (DX)

### DX Virtual Interfaces 
- Private VIF 
- Public VIF 
- Transit VIF 

### Direct Connect Gateway 

### Active/Active vs Active/Passive Scenarios (Direct Connect)

### MACsec Encryption (Layer2)

### BGP Attributes 

### Route 53

- Route53 Resolver DNS Firewall 

### CloudFront 

- Lamda@Edge UseCases

### Global Accelerator 

### ELB , NLB , ALB 
usecases

### GWLB and GWLB Endpoints 


### AWS GuardDuty 

### AWS Shield 

### AWS WAF 

### AWS Network Firewall 

### AWS Inspector 

### AWS CloudFormation 

### AWS Config 


### Summary 



References:
ANS-C01

https://aws.amazon.com/certification/certified-advanced-networking-specialty/

Sample Exam Questions:

https://d1.awsstatic.com/training-and-certification/docs-advnetworking-spec/AWS-Certified-Advanced-Networking-Specialty_Sample-Questions.pdf

Practice Questions Test:

https://explore.skillbuilder.aws/learn/course/external/view/elearning/12676/aws-certified-advanced-networking-specialty-official-practice-question-set-ans-c01-english?ans=sec&sec=prep
