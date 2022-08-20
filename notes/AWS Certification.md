---
title: AWS Certification
uuid: c750cd88-095d-11ed-be7e-7eb08a2c5cd0
version: 179
created: Fri, 22 Jul 2022 01:29:51 +0000
tags:
- aws
---

- [S3](S3.md) 

    - 

- Snowball, Snowball Edge, Snowmobile => Are Physical devices used to transfer data in and out of S3

    - [ ] Cheetsheet - Screenshot [^1] 

[VPC](VPC.md) 

- IAM

    - Core Components

        - Users

        - Groups

        - Roles

            - Policies

                - Managed Policies, managed by AWS, read only, you can't edit them

                - Customer managed policies, you create them

                - Inline policies, one time temporary policies

    - Use cases 

        - Policies assigned to roles, role assigned to group

        - Policies assigned to roles, role assigned to user

        - Policies assigned to user (inline)

        - Multiple policies can be assigned to one role

        - Role assigned to resources

    - Three types of role policies 

    - User MFA, Programmatic keys

- [Amazon Cognito](Amazon%20Cognito.md) 

- DNS 

    - Domain name server, converts domain name to an IP address

    - IP address can be IPv4 or IPv6

    - A (Address) Record info about a domain and which IP it points to

    - CNAME canonical names are domain name to another domain name records

- Route 53 is AWS DNS

    - Traffic flow : visual editor 

    - Routing policies

        - Simple routing policy : record set point to one or multiple IPs, multiple ips it will pick random IP for each routing

        - Weighted routing policy : split traffic based on weight assigned

        - Latency based routing : 

        - Failover routing policy

- AMI - Amazon Machine images

    - Template to configure new instances

- Auto scaling groups

    - Launches or shuts down EC2 instances based on demand

---
[^1]: Screenshot

    ![](images/c750cd88-095d-11ed-be7e-7eb08a2c5cd0/cd5583c9-2b79-4f27-b568-018ea1f6bab4.png)