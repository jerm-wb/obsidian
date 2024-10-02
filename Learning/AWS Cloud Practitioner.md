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

# Introducing Cloud Computing and Deployment Models
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

	h