#Overview #EC2 #Containers
# 🎁 What are Containers?
> [!analogy]
> Think of containers like pizza boxes:
> - Each box contains separate application/service
> - Can be stacked on single server or distributed
> - Creates organization, separation, and security

# 📋 Container Benefits
- **Increased Portability**
  - Deploy across multiple OS and hardware platforms
- **Operational Consistency**
  - Same deployment behavior everywhere
- **Greater Efficiency**
  - Rapid deployment, patching, and scaling
- **Development Acceleration**
  - Faster dev, test, and production cycles
- **Resource Efficiency**
  - Less system resources than traditional VMs
  - No OS images included

## 🎯 When to Use Containers
> [!tip]
> Consider containers for:
> - Lift and shift to cloud
> - Application refactoring for cloud-native
> - Microservices architecture
> - CI/CD streamlining
> - Repetitive tasks (ETL, batch jobs)

# AWS Container Services

## 📦 Elastic Container Registry (ECR)
> [!analogy]
> Like storing recipes for pizza
>  Store, share, and deploy container software

## 👨‍🍳 ECS vs EKS (The Head Chefs)
**Common Features:**
- Both are container orchestration services
- Fully managed
- Can run with:
  - EC2
  - Fargate
  - Outposts
  - Anywhere (hybrid solutions)

### Key Differences:

| ECS                                   | EKS                               |
| ------------------------------------- | --------------------------------- |
| Built with Fargate                    | Uses Kubernetes (open-source)     |
| Supports Docker & Docker Composed CLI | Supports Kubernetes               |
| -                                     | Supports Local Zones & Wavelength |

> [!note]
> Choice between ECS and EKS often depends on team expertise with Docker vs Kubernetes

---
*Notes Last Updated: 2025-02-14 14:30*