# AWS setup for High Availability Scalability and Resiliency

1. Created VPC
2. Deployed servers in 2 AZs
3. Used Auto-Scaling Groups
4. Configured Application Load Balancer (ALB)
5. Configured NAT as well

Deployed servers only in private subnets for additional security. Servers recieve requests through Load Balancer. Servers connect to the internet using NAT Gateway. To improve resiliency, deployed NAT Gateways to both AZ's.

