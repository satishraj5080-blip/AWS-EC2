AWS EC2 Ubuntu Server Deployment and Configuration
--------------------------------------------------------------------------------------------------------------
By Satish Pawar

Project Overview
This project demonstrates the deployment and configuration of an Ubuntu Server on AWS EC2. The objective was to gain hands-on experience with cloud computing, Linux server administration, networking, and secure remote access using SSH.
Technologies Used
•	Amazon Web Services AWS EC2 
•	Ubuntu Server Ubuntu Server 
•	SSH 
•	Linux Commands 
•	Security Groups 
•	VPC Networking 
Project Objectives
•	Launch an Ubuntu Server EC2 instance. 
•	Configure Security Groups. 
•	Create and manage SSH key pairs. 
•	Connect securely using SSH. 
•	Perform basic Linux administration tasks. 
•	Understand cloud infrastructure fundamentals. 
Project Architecture
Local Computer
       |
       | SSH (Port 22)
       |
       v
AWS EC2 Ubuntu Server
Implementation Steps
Step 1: Login to AWS Console
Logged into AWS Management Console.
Step 2: Launch EC2 Instance
•	Opened EC2 Dashboard. 
•	Clicked Launch Instance. 
•	Named instance: Ubuntu-Server. 
•	Selected Ubuntu Server AMI. 
•	Chose t2.micro instance type. 
Step 3: Create Key Pair
•	Generated a new key pair. 
•	Downloaded the .pem file securely. 
Step 4: Configure Security Group
Allowed:
•	SSH (Port 22) 
Step 5: Launch Instance
Successfully launched the Ubuntu Server instance.
Step 6: Connect Using SSH
Example command:
ssh -i ubuntu-key.pem ubuntu@<public-ip>
Step 7: Verify Server Access
Checked server details:
hostname
whoami
pwd
Step 8: Update Ubuntu Server
sudo apt update
sudo apt upgrade -y
Step 9: Install RDP Package (XRDP)
Installed XRDP for remote desktop access:
sudo apt update
sudo apt install xrdp -y
sudo systemctl enable xrdp
sudo systemctl start xrdp
Verified service:
sudo systemctl status xrdp
Step 10: Configure Security Group for RDP
Added inbound rule:
Type	Port
RDP	3389
Step 11: Connect via Remote Desktop
Used Windows Remote Desktop Connection and connected using:
Public IP Address
Ubuntu Username
Ubuntu Password
Skills Gained
•	AWS EC2 Administration 
•	Linux Server Administration 
•	Ubuntu Server Management 
•	SSH Configuration 
•	XRDP Installation 
•	Cloud Computing Fundamentals 
•	Security Group Configuration 
•	Remote Server Management 
Project Outcome
Successfully deployed an Ubuntu Server on AWS EC2, configured SSH access, installed XRDP, and enabled remote administration through Remote Desktop.

