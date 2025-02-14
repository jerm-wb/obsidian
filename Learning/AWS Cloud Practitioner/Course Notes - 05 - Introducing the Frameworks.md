 #Architecture #Overview
# Cloud Adoption Framework Overview
## Perspectives and Foundational Capabilities
### Security
- Focuses on compliance and assurance
- Governance, security assurance, and application security
- Protection of infrastructure and data
- Identity and access management
- Incident response and threat detection
### Business
- Focuses on strategy and outcomes
- Strategy, product innovation
- Data science, monetization
### Platform
- Focuses on architecture and engineering
- Continuous Integration/Continuous Delivery
- Modern App Development
- Provisioning and Orchestration
### Operations
- Focuses on successful workload delivery
- Manages event (AIOps), incident and problem, change and release, performance and capacity, configuration, patches, availability and continuity, and application
-  Observability is high priority
### Governance
- Focuses on transformational risks and maximizing organizational benefits
- Manages program and project benefits, risk, financial, and portfolio
- Governs data and curation
### People 
- Focuses on people and business
- Transformation of leadership and workforce
- Organization of design and alignment
- Cloud fluency, change acceleration, culture evolution
## Cloud Transformation Domains
### Technology
- Migrate and modernize legacy infrastructure
### Process
- Digitize, automate, and optimize your business
### Organization
- Reimagine orchestration
### Product
- Reimagine business model by creating new products/services
## Cloud Transformation Journey Phases
### Envision
- Benefits to business outcomes
### Align
- Gaps across perspectives
### Launch
- Delivering pilot transformations and their value
### Scaling
- Expand sustainable initiatives
## Image Overview
![[Pasted image 20241002144646.png]]
# Well-Architected Framework Overview
## Six Pillars
### Security
- Focuses on protection of data, systems, and any assets used by your workload
- E.g. using CloudTrail to log all actions performed in your account
### Cost Optimization
- Focuses on the ongoing process of maintaining costs in the cloud
- Use S3 Intelligent-Tiering to automatically move data
### Performance Efficiency
- Focuses on the ability to use computing resources efficiently to meet requirements
- Use Lambda to run code with zero administration
### Operational Excellence
- Focusing on creating applications that successfully support your workload
- Use CodeCommit for code and template version control
### Reliability
- Focuses on architecting a workload to be consistent and able to recover quickly
- Use Multi-AZ deployments of RDS databases
### Sustainability
- Focuses on environmental impacts like energy efficiency and consumption
- Use EC2 Auto Scaling to ensure maximum utilization
## General Design Principles
- Stop guessing your capacity needs by collecting usage data
- Test systems at production scale
- Consider evolutionary architectures
- Automate with architectural experimentation in mind
- Drive architectures using data by leveraging usage information
- Improve through game-days (drills)
## 💡 Exam Tips
> [!important]
> Remember:
> - Understand the CAF perspectives and the Cloud Transformation Journey Phases
> - Understand the Well-Architected Framework pillars, design principles, and how they apply in the real world

---
*Notes Last Updated: 2025-02-14 14:08*