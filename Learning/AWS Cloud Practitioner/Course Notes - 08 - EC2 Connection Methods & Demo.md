#EC2 #Overview 
# Connection Methods
- **AWS Management Console**
  - Browser-based configuration and management
  
- **EC2 Instance Connect (EIC)**
  - Uses IAM policies to control SSH access
  - Eliminates need for SSH key management
  
- **SSH/RDP Connection**
  - SSH → Linux instances
  - RDP → Windows instances
  - Requires key pair (public + private keys)
  - Connect from local machine using private key
  
- **Session Manager (Systems Manager)**
  - Manage instances via browser or AWS CLI

# Creating EC2 Instance

## Instance Configuration
1. Name: Web App
2. AMI: Amazon Linux (free tier)
3. Create new key pair: "NewKeyPair"
   > ⚠️ Key pair can only be downloaded at creation time

## Setup Steps
1. Access EC2 dashboard
2. Launch new instance
3. Configure settings:
   - Title: Web App
   - AMI: Amazon Linux (free tier)
   - Architecture: Default
   - Instance Type: Free tier eligible
   - Network: Allow SSH from anywhere (for demo)
   - Storage: Default configuration

## Connection Test
1. Wait for instance status: Running
2. Use Instance Connect
3. Verify connection using list command

# 📝 Exam Tips
> [!important]
> - Know all methods to connect to EC2 from local machine:
>   - Management Console
>   - Instance Connect
>   - SSH/RDP
>   - Systems Manager
> 
> - Remember Linux connection options:
>   - Instance Connect
>   - SSH
>   - Systems Manager
> 
> - Windows instances use RDP only

# 🔑 Key Points
- Different connection methods serve different purposes
- Security considerations important for production
- Free tier options available for testing
- Instance Connect simplifies SSH access 
---
*Notes Last Updated: 2025-02-14 14:28*