#Overview #Serverless
# 🌐 What is Serverless?
> [!info]
> A cloud-native development model where:
> - Developers build/run apps without managing servers
> - Servers exist but are abstracted away
> - Focus is purely on code and business logic

# 🔄 AWS Serverless Services

## Lambda
> [!definition]
> Serverless compute service for running code without server management

**Key Features:**
- Supports multiple languages (Python, Rust, Ruby, etc.)
- Automatic scaling
- Function-based architecture

### Use Cases for Lambda:
1. **Real-time File Processing**
   ```mermaid
   graph LR
   A[S3 Upload] --> B[Lambda] --> C[DynamoDB]
   ```

2. **Email Notifications**
   ```mermaid
   graph LR
   A[CodeCommit Changes] --> B[CloudWatch] --> C[Lambda] --> D[SNS] --> E[Email]
   ```

3. **Backend Business Logic**
   ```mermaid
   graph LR
   A[Alexa Skill] --> B[Lambda] --> C[DynamoDB] --> D[Lambda] --> E[Alexa Response]
   ```

## Fargate
> [!definition]
> Pay-as-you-go auto-scaling compute engine for containers

**Key Features:**
- Container-based
- Define memory and compute resources
- Isolated tasks (no shared resources)
- Launch type in ECS

### Use Cases for Fargate:
1. **Message-Driven Workloads**
   - Long-polling SQS messages
   - Processing > 15 minutes
   - DynamoDB storage

2. **Event-Driven & Scheduled Workloads**
   Example: Code Scanning Flow
   ```mermaid
   graph LR
   A[CodeCommit PR] --> B[Lambda] --> C[Fargate Task] --> D[SNS/Email]
   ```

# 🔑 Key Differences
> [!important]
> Lambda vs Fargate:
> - Lambda: Short, redundant tasks (<15 mins)
> - Fargate: Longer-running container tasks

# 📝 Exam Tips
> [!tip]
> Remember:
> 1. **Lambda Responsibilities**
>    - You: Code only
>    - AWS: Servers, environment, language support
> 
> 2. **Fargate**
>    - Considered serverless
>    - Used for container management
>    - Part of ECS ecosystem

# 💡 Selection Guide
>[!tip]
>- Need quick functions? → Lambda
>- Need longer processes? → Fargate
>- Need container management? → Fargate
>- Need simple code execution? → Lambda

---
*Notes Last Updated: 2025-02-14 14:39*