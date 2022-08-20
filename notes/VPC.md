---
title: VPC
uuid: 241dd6e8-1078-11ed-a3fd-b244f95defbd
version: 194
created: Sun, 31 Jul 2022 02:26:12 +0000
---

- Vitrual Private Cloud

    - Default VPC is created

    - **Sider Range** 173.31.0.0/16 => 173.31 network address 0.0 is for machine

        - 16 => 65,536 possible machines

        - Might be too many

    - **Subnets** in the Sider Range

        - Each in a separate availability zone

    - **Routing** tables define how to move packets around 

        - Every VPC has default route table which considers everything in sider range, inside that VPC

---

    - **VPC Peering** is connection between two VPCs.

        - Each VPC should have their own peering, there is no bypassing of Peering

    - **Public Subnet** each pc will be assigned private + public IP

    - **IGW** internet gateway

    - **Bastian** allows SSH passthrough to an EC2 instance in private subnet (Now Session Manager is replacing bastian)

    - **NAT Gateway**  only allows one way traffic (means only allow responses to requests initiated from within the network)

        - Create private subnet which talks to NAT Gateway

    - **Security Groups** define who can have access to the servers. Either allow public access, or allow traffic from a particular security group.

    - **Direct connect** very fast connection from on-prem to AWS (lower bandwidth 50-500m or higher 1-10gb)

    - **VPC endpoint** allows communication between e.g. VPC and s3 from with-in the network rather than going to internet 