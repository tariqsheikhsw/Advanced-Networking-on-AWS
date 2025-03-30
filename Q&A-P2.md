### ANS-C01 Q&A Part2

# Static Vs Dynamic Routing

### Dynamic Routing

Type of routing to use in Site-to-Site VPN if your Customer Gateway device supports Border Gateway Protocol (BGP)

### Static Routing

Type of routing to configure in Site-to-Site VPN if your Customer Gateway device does NOT support Border Gateway Protocol (BGP)


# Symmetric vs Asymmetric Routing

For Customer Gateway devices that support Asymmetric Routing, AWS does NOT recommend using AS PATH Prepending

For Customer Gateway devices that support Asymmetric Routing, not implementing the AS PATH Prepending method ensures that the multi-exit discriminator (MED) value, that AWS sets on a tunnel, is used to determine tunnel priority.

# BGP Attributes 

### Multi-Exit Discriminator (MED)

What optional BGP attribute, that AWS sets on a tunnel during VPN tunnel endpoint updates, is used to determine tunnel priority.

The Internet-routable IP address for your Customer Gateway must be static and can be behind a device performing network address translation (NAT).

# VPN 

In your VPN connection, you can use an existing public Border Gateway Protocol (BGP) Autonomous System Number (ASN) assigned to your network, with the exception of:

7224 – Reserved in all Regions
9059 – Reserved in the eu-west-1 Region
10124 – Reserved in the ap-northeast-1 Region
17943 – Reserved in the ap-southeast-1 Region

# Virtual Private Gateway vs Transit Gateway vs Customer Gateway vs Cloud WAN 

### Virtual Private Gateway

is the VPN concentrator on the Amazon side of the site-to-site VPN connection.

### Customer Gateway

A resource that you create in AWS that represents the physical or software device residing on your on-premises network (your side of the VPN connection)

# Application Load Balancer vs Network Load Balancer

### Application Load Balancer

What type of AWS Load Balancer will the AWS Load Balancer Controller provision to the Amazon EKS cluster if you create a Kubernetes Ingress?

### Network Load Balancer

The AWS Load Balancer Controller will provision. what type of load balancer cluster if you create a Kubernetes service of type LoadBalancer?

