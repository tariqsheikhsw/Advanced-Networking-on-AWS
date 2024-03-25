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

How to share DNS services between accounts (for example, AWS RAM)
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
