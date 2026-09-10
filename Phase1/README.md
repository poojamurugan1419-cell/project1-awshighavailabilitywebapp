project-1
# AWS High Availability Web Application

## Project Overview

Built a highly available web application using AWS.

## AWS Services Used

- VPC
- EC2
- Application Load Balancer
- Target Group
- Security Groups
- Internet Gateway
- CloudWatch
- S3

## Architecture
            INTERNET
                     |
                     v
              Application LB
                     |
             ┌───────┴───────┐
             |               |
             v               v
         EC2 #1           EC2 #2
         Nginx             Nginx
             |               |
        AZ-1/Subnet 1   AZ-2/Subnet 2
             \               /
              \             /
                 VPC
              10.0.0.0/16


## Implementation

1. Created VPC
2. Created two public subnets
3. Created Internet Gateway
4. Created route table
5. Created security group
6. Launched EC2 instances
7. Installed Nginx
8. Created Target Group
9. Created Application Load Balancer
10. Configured CloudWatch

## Testing

- EC2 1 healthy
- EC2 2 healthy
- ALB health checks successful
- Website accessible through ALB

## What I Learned

- VPC networking
- Public subnet
- Route tables
- Security groups
- EC2
- Load balancing
- Health checks
- High availability
- CloudWatch monitoring
