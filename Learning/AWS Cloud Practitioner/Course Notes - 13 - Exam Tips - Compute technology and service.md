#EC2 #Serverless 
#  EC2 Pricing Options
- On Demand
- Spot Instances
	- Cheapest if start and stop times don't matter
- Dedicated Hosts
	- Not the same as Dedicated instances!
- Reserved Instances
	- Time commitment for 1-3 years
- Savings Plans
	- Time commitment for 1-3 years
# Real-World Uses for EC2
- Deploying highly available applications
- Databases you need full control over
# Scaling Types and Benefits
## Horizontal (Scaling Out)
- High availability
- Done across multiple AZs
## Vertical (Scaling Up)
- Increases resources on individual instances
- Less complex but limited by hardware capacity
# Load Balancer Types
- Classic Load Balancer
- Gateway Load Balancer
- Application Load Balancer (ALB)
  - Uses HTTP/HTTPS protocols
  - Best for web applications
- Network Load Balancer (NLB)
  - Offers extreme performance
  - Static IPs with TCP, UDP, and TLS protocols
# EC2 Connection Methods
- Console
- Instance Connect
- SSH (requires key pair)
- Systems Manager
# Container Services
## ECS (Elastic Container Service)
- Supports Docker
- Owned and managed by AWS
## EKS (Elastic Kubernetes Service)
- Fully managed by AWS
- Supports Kubernetes (open source)
## When to use containers
- Lift and shift migrations
- Microservices architecture
- CI/CD deployments
- Refactoring applications
#  Serverless Services
## Lambda
- You're only responsible for your code
- AWS manages servers, environment, and language support
- Always free tier: 1 million requests free per month
- 15-minute timeout limit
- Can be triggered by events
## Fargate
- Considered serverless
- Used to manage containers
- No upfront costs
- Pay only for what you use (vCPUs, memory, storage)
# Additional Compute Services
- Outposts: Hybrid deployment with local data residency
- Lightsail: Quick launch for small projects (test environments, WordPress)
- Batch: Processes larger workloads into smaller batches
- Wavelength: Allows users to access applications within 5G mobile networks
# 💡 Exam Tips
> [!important]
> Remember:
> - Spot instances are cheapest but have unpredictable start/stop times
> - Horizontal scaling provides high availability across multiple AZs
> - Lambda has a 15-minute timeout and 1M free requests/month
> - For containers, think microservices and CI/CD pipelines
> - Fargate is serverless container management (pay-per-use)

---
*Notes Last Updated:  2025-02-21 14:50*