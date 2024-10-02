```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 2 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
(disregard this, it's a table of contents when viewed in Obsidian)
# Getting your head in the Cloud
## What is the cloud?
- Decentralized server architecture
- Data centers divided into slices using virtualization
	- Virtualization cost is gauged like an electric meter
		- On-demand
		- Pay-as-you-go
## What is cloud computing?
- Using the internet to deliver computing services
	- Rather than an internal data center or local machine
## Types of services AWS offers	
*For more information, go to [Overview of Amazon Web Services ](https://docs.aws.amazon.com/pdfs/whitepapers/latest/aws-overview/aws-overview.pdf)*
- Compute
- Storage
- Networking
- Database
- Developing
- Migration
- Artificial Intelligence
- Auditing
- Security
- Pricing
## Exam Tips
- Learn the different service categories
- Read the whitepaper linked above

# Cloud Computing and Deployment Models
## CapEx vs. OpEx
- Capital Expenditures
	- Upfront purchases towards fixed assets
		- E.g. datacenter, office building, company vehicle
- Operating Expenses
	- Funds used to run day-to-day operations
		- E.g. salaries, office supply cost, fuel for company vehicle

## Cloud Computing Advantages
- Global environment in minutes
- No data center spending
- Leverage economies of scale
- Deployment speed and agility
- Elastic capacity allows you to only use what you need
#### High availability
- Designed to operate continuously without failure for a long time
- Avoid loss of services by managing failures
#### Elasticity
- Can provision only what you need
- Grow and shrink based on demand
#### Agility
- All the new services facilitates quicker innovation
#### Durability
- Services can go longer without corruption

## Cloud Computing Models
### Infrastructure as a Service
- Building blocks that the end user can choose to put together how they please
- E.g. monthly subscription to a hosting site
### Software as a Service
- Using a complete application on demand that is offered to users
- E.g. email service
### Platform as a Service
- Help develops software using web-based tools
- E.g. storefront generators

## Cloud Deployment Models
### Private Cloud
- All resources are *on premises*
- Offers more security, but has less of the cool stuff from before
### Public Cloud
- AWS, Azure, etc.
- Offers less security, but has all of the cool stuff from before
### Hybrid Cloud
- Sensitive data is on premises, securely connected to Public Cloud
- Good tradeoff of Public and Private clouds

## Exam Tips
- Understand the six advantages of the cloud
- Understand cloud benefits and terminologies
- Know the computing models (IaaS, SaaS, PaaS)
- Know the deployment models (Private, Hybrid, Public)

# Exploring Regions and Availability Zones
## AWS Regions
- A physical location, grouped by geographical locations
- Regions are isolated from each other
	- Resources are not shared between the regions and would need to be replicated manually across them
## Availability Zones
- **Official Definition**: One or more discrete data centers with redundant power, networking, and connectivity in an AWS region
- AWS Regions consist of multiple availability zones
- Each availability zone has one or more data center
### Characteristics of Availability Zones
- Housed separately, but connected through low-latency links
- If one AZ goes out, the rest are *not* affected
- Allows for high availability if an app is deployed on multiple AZs
## Exam Tips
- Region is global and is made up of two or more AZs
- An AZ is made up of multiple data centers
- Multi-AZ deployments provide high availability
# Reviewing Edge Locations and Local Zones
## Latency
- In layman's terms: the amount of time a website takes to load
- More accurately: the time that passes between a users request and the resulting response
- Low latency > High latency
## Local Zones
- Place AWS services closer to end-users
- Facilitates lower latency
- Extensions of AWS Regions
## Edge Locations
- Aren't used to launch resources, but instead cache content for quicker viewing
- Delivered by Cloudfront
- More edge locations than AZs, due to use of the AWS backbone network
## Exam Tips
- An edge location ensures low latency by placing content closer to users
- A local zone is an extension of a region which is closer to end-users
# Introducing the Frameworks
## Cloud Adoption Framework Overview
### Perspectives and Foundational Capabilities
#### Security
- Focuses on compliance and assurance
- Governance, security assurance, and application security
- Protection of infrastructure and data
- Identity and access management
- Incident response and threat detection
#### Business
- Focuses on strategy and outcomes
- Strategy, product innovation
- Data science, monetization
#### Platform
- Focuses on architecture and engineering
- Continuous Integration/Continuous Delivery
- Modern App Development
- Provisioning and Orchestration
#### Operations
- Focuses on successful workload delivery
- Manages event (AIOps), incident and problem, change and release, performance and capacity, configuration, patches, availability and continuity, and application
-  Observability is high priority
#### Governance
- Focuses on transformational risks and maximizing organizational benefits
- Manages program and project benefits, risk, financial, and portfolio
- Governs data and curation
#### People 
- Focuses on people and business
- Transformation of leadership and workforce
- Organization of design and alignment
- Cloud fluency, change acceleration, culture evolution
### Cloud Transformation Domains
#### Technology
- Migrate and modernize legacy infrastructure
#### Process
- Digitize, automate, and optimize your business
#### Organization
- Reimagine orchestration
#### Product
- Reimagine business model by creating new products/services
### Cloud Transformation Journey Phases
#### Envision
- Benefits to business outcomes
#### Align
- Gaps across perspectives
#### Launch
- Delivering pilot transformations and their value
#### Scaling
- Expand sustainable initiatives
### Image Overview
![[Pasted image 20241002144646.png]]
## Well-Architected Framework Overview
### Six Pillars
#### Security
- Focuses on protection of data, systems, and any assets used by your workload
- E.g. using CloudTrail to log all actions performed in your account
#### Cost Optimization
- Focuses on the ongoing process of maintaining costs in the cloud
- Use S3 Intelligent-Tiering to automatically move data
#### Performance Efficiency
- Focuses on the ability to use computing resources efficiently to meet requirements
- Use Lambda to run code with zero administration
#### Operational Excellence
- Focusing on creating applications that successfully support your workload
- Use CodeCommit for code and template version control
#### Reliability
- Focuses on architecting a workload to be consistent and able to recover quickly
- Use Multi-AZ deployments of RDS databases
#### Sustainability
- Focuses on environmental impacts like energy efficiency and consumption
- Use EC2 Auto Scaling to ensure maximum utilization
### General Design Principles
- Stop guessing your capacity needs by collecting usage data
- Test systems at production scale
- Consider evolutionary architectures
- Automate with architectural experimentation in mind
- Drive architectures using data by leveraging usage information
- Improve through game-days (drills)
## Exam Tips
- Understand the CAF perspectives and the Cloud Transformation Journey Phases
- Understand the Well-Architected Framework pillars, design principles, and how they apply in the real world

# AWS Management Console and accessing AWS
## Root User
- Initially created when you set up the account
- Can delete the account and all resources inside the account
- Should *NOT* be used for day to day tasks
## CLI
- Allows you to access resources through a terminal window
- Sometimes new features are in CLI first
- Allows programmatic access
## Programmatic Access
- Multiple ways to achieve programmatic access
	- CLI
	- Application code
	- SDKs (access from programming languages)
## Exam Tips
- The root user should be protected by MFA, and is more powerful than *any* other user
- CLI and SDKs are available options
# Compute: The Bigger Picture
