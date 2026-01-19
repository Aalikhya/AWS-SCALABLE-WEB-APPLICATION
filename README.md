# AWS Scalable Web Application

## Overview
This project demonstrates a highly available, secure, and scalable web application architecture on AWS.

## Architecture
- Amazon CloudFront for HTTPS and global caching
- Application Load Balancer for traffic distribution
- Auto Scaling Group with EC2 instances in private subnets
- IAM Role and AWS Systems Manager (SSM) for secure instance access
- VPC with public and private subnets and NAT Gateway

## Features
- Auto scaling based on demand
- High availability across multiple Availability Zones
- Secure HTTPS access
- No SSH access (SSM-based management)
- Infrastructure automation using EC2 User Data

## Technologies Used
- AWS EC2
- Application Load Balancer
- Auto Scaling
- CloudFront
- IAM
- Systems Manager
- Amazon VPC

## Request Flow
User → CloudFront → Application Load Balancer → EC2 (Auto Scaling Group)

## How It Works
EC2 instances are automatically configured using a user data script that installs and configures the web server and deploys the application.

## Author
Aalikhya Soni