# AWS-EC2-Instance-Setup
# Project Overview
This repository provides a step-by-step guide to creating, configuring, and managing an AWS EC2 instance. It covers everything from launching an instance, configuring security settings, connecting via Remote Desktop Protocol (RDP), and terminating the instance after use. This project also demonstrates how to use SSH keys for secure access and manage instance security with network and firewall rules.

# Key Steps and Features
1. Create AWS Account

- If you don't have an AWS account, sign up for the AWS Free Tier.
2. Navigate to EC2 Dashboard

- Once logged into AWS, use the EC2 Dashboard to start setting up your instance. EC2 (Elastic Compute Cloud) provides scalable computing capacity in the cloud.
3. Launch a New EC2 Instance

- From the EC2 dashboard, select "Launch Instance" and begin the setup process for your virtual machine.
4. Choose Amazon Machine Image (AMI)

- Select an Amazon Machine Image (AMI) based on your needs. The free-tier AMIs include:
- Amazon Linux 2 AMI (Free-tier eligible)
- Ubuntu Server
- Windows Server
- For this guide, we select Amazon Linux 2 AMI.
5. Select Instance Type

- Choose the t2.micro instance type (1 vCPU, 1 GB RAM) to remain in the free tier.
- Click Next: Configure Instance Details.
6. Configure Network Settings and Security

- Ensure auto-assign Public IP is enabled to allow public internet access.
- Set up a security group:
- Allow inbound traffic for RDP (port 3389), SSH (port 22), HTTP (port 80) if you plan to use it as a web server.
- You can restrict IP ranges for additional security, allowing only trusted IPs.
7. Create SSH Key Pair

- Set up a key pair for secure access to the EC2 instance. The private key will be required to SSH into the instance.
- Download the .pem file and store it securely. You will need this to access your instance later.
8. Launch and Connect to Instance

- After reviewing the instance configuration, click Launch.
- Use Microsoft Remote Desktop (RDP) to connect to Windows instances, or SSH for Linux-based instances.
9. Configure Remote Desktop Access (for Windows)

- Once the instance is running, download the RDP file from the AWS console and use it to access your instance.
- If using Windows, retrieve the password by decrypting it with your .pem key.
10. Terminate or Stop the Instance

- After completing your tasks, either stop the instance to save costs or terminate it to remove it entirely. Stopping retains your data, while terminating deletes it.

# How to Run
# Prerequisites:

1. AWS account
- SSH client or Remote Desktop Connection (depending on the instance type)
- Basic understanding of networking and cloud concepts
2. Instructions:

- Follow the step-by-step guide in instance_setup.md to configure and launch your instance.
3. Termination:

- To avoid unnecessary charges, remember to stop or terminate your instance after use.

![Screenshot 2024-09-29 at 11 13 01 AM](https://github.com/user-attachments/assets/e457e12f-2f47-4c5e-8453-b3c70a2ef0a5)
![Screenshot 2024-09-29 at 11 13 17 AM](https://github.com/user-attachments/assets/e747ec78-b0d2-4273-b055-92ac40f183c6)
![Screenshot 2024-09-29 at 11 13 26 AM](https://github.com/user-attachments/assets/11f6c031-8cd0-4749-91cf-0c27c97f6d55)
![Screenshot 2024-09-29 at 11 13 36 AM](https://github.com/user-attachments/assets/9492e3a3-5f9e-45c4-a980-997466468a63)
![Screenshot 2024-09-29 at 11 13 41 AM](https://github.com/user-attachments/assets/0afcc89c-bf7c-455e-b031-31dd7da6e9b6)
![Screenshot 2024-09-29 at 11 13 47 AM](https://github.com/user-attachments/assets/15f1cd02-0f91-4290-b412-74d3a76b81b5)
![Screenshot 2024-09-29 at 11 13 56 AM](https://github.com/user-attachments/assets/0acc68f2-7d8b-4b2f-84f2-d1914599c812)
![Screenshot 2024-09-29 at 11 14 04 AM](https://github.com/user-attachments/assets/27ca3496-d62f-47bc-af28-91c51d906d70)
![Screenshot 2024-09-29 at 11 14 11 AM](https://github.com/user-attachments/assets/1b381f26-354a-4dbb-9f54-65498e520bb5)
![Screenshot 2024-09-29 at 11 14 18 AM](https://github.com/user-attachments/assets/34ff9cc1-49e5-4d1e-842b-3a5324fd0eec)
![Screenshot 2024-09-29 at 11 14 25 AM](https://github.com/user-attachments/assets/0945c4e8-1b5b-4eab-a152-ccf40192ee0e)
![Screenshot 2024-09-29 at 11 14 31 AM](https://github.com/user-attachments/assets/62cf8878-0663-4b4e-936a-e2437f64da96)
![Screenshot 2024-09-29 at 11 14 36 AM](https://github.com/user-attachments/assets/a949dab1-0aa8-4225-a135-f1bc8cf1eafb)
![Screenshot 2024-09-29 at 11 14 41 AM](https://github.com/user-attachments/assets/8ac73c12-a864-42df-924d-9cfae87cda3a)
