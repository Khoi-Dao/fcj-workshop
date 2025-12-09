---
title: "Week 2 Worklog"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---



### Week 2 Objectives:

* Understand the concept and structure of VPC (CIDR, Subnet, Route Table, ENI).
* Learn to configure firewalls in VPC (NACL, Security Group).
* Understand the concept of networking services: VPN, Direct Connect.
* Experience on Load Balancer
* Experience on creating and configuring core components: VPC, Subnet, Route Table, IGW, EBS, Elastic IP.
* Understand  about connection to EC2 using remote  via SSH
* Experience Hybrid DNS using Route 53 Resolver.
* Experience multiple VPCs using VPC Peering.
* Testing AWS Transit Gateway to manage  inter-VPC connections 

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn theory <br> - What is VPC and how to optimize cloud service usage  <br> - Learn about VPC: <br>&emsp; + Subnet, CIDR <br>&emsp; + Route table <br> &emsp; + ENI (Elastic Network Interface)s                                                                                                 | 09/15/2025 | 09/15/2025      |1. [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) <br>2. [YouTube - AWS VPC](https://www.youtube.com/watch?v=O9Ac_vGHquM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=25) |
| 3   | - Configure VPC firewalls: NACL, Security Group <br> - VPN, Direct Connect <br> - Load Balancer <br> - Extra Resources                                              | 09/14/2025 | 09/14/2025      | [YouTube - AWS Security](https://www.youtube.com/watch?v=O9Ac_vGHquM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=25) |
| 4   | - **Labs:** <br>&emsp; + VPC + Subnet <br>&emsp; + Route Table <br> &emsp; + IGW(Internet GateWay) <br> &emsp; + EBS <br> &emsp; + ... <br> - Remote SSH into EC2 <br> - Learn Elastic IP | 09/15/2025 | 09/15/2025      | [AWS Study Group - 000003 : Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 5   | - **Labs:** <br>&emsp; + Set up Hybrid DNS with Route 53 Resolver <br>&emsp;+ Set up VPC Peering                          | 09/16/2025 | 09/16/2025      | [AWS Study Group - 000010 : Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) <br> [AWS Study Group - 000019 : Setting up VPC Peering](https://000019.awsstudygroup.com/)|
| 6   | - **Labs:** <br>&emsp; + Continue on experiencing VPC Peering <br>&emsp;+ Set up AWS Transit Gateway                                                                                     | 09/17/2025 | 09/17/2025      | [AWS Study Group - 000020 : Set up AWS Transit Gateway](https://000020.awsstudygroup.com/) |


### Week 2 Result:

* Understood the fundamental of Amazon VPC, and its key components: CIDR blocks, subnets, route tables, and ENIs.
* Experienced the activity of securing VPCs using both Security Groups and Network ACLs, and understand their differences in scope and use cases.
* Explored AWS networking services : VPN and Direct Connect 
* Learnt Elastic Load Balancing and its role in distributing traffic for high availability.
* Did labs about VPC essentials: creating subnets, configuring route tables, attaching internet gateways, working with EBS, and managing Elastic IPs.
* Reinforced skills in accessing and managing EC2 instances securely via SSH.
* Tested and practiced connecting multiple VPCs through VPC Peering.
* Deployed AWS Transit Gateway to design and manage scalable multi-VPC architectures.
