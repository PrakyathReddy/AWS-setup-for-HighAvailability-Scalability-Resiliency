# AWS setup for High Availability Scalability and Resiliency

1. Created VPC
2. Deployed servers in 2 AZs
3. Used Auto-Scaling Groups
4. Configured Application Load Balancer (ALB)
5. Configured NAT as well

Deployed servers only in private subnets for additional security. Servers recieve requests through Load Balancer. Servers connect to the internet using NAT Gateway. To improve resiliency, deployed NAT Gateways to both AZ's.

![public-private-subnet-architecture](public-private-subnet-architecture.png)

Step 1: Create VPC. Make sure to select 1 NAT Gateway per AZ. 
![vpc](VPC-resources.png)
![vpc2](VPC.png)
VPC created with 4 subnets in 2 AZs and a NAT gateway in each AZ

Step 2: Create AutoScaling Group
