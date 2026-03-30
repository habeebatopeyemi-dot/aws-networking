1. I created a VPC and split it into two subnets in different availability zones

 Public Subnet: 10.0.0.0/24

 Private Subnet: 10.0.1.0/24

2. I deployed a NAT Gateway in the Public Subnet to allow the private instance to communicate with the internet.

   I updated the Private Route Table to point all internet traffic to the NAT Gateway.

3.  I configured security group to allow SSH traffic from specific IP ranges.

4. I implemented a stateless NACL, configured both inbound and outbound rules to allow traffic to flow correctly. 
