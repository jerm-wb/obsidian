#Architecture #Billing #EC2
## Introduction to EC2
Foundational service that manages virtual instances
- Stands for Elastic Cloud Compute
	- Elastic in this context means that the EC2 instance can grow and shrink as necessary
- Virtual servers in the cloud, running on a physical server in a datacenter
- Provisions Amazon Machine Images (AMIs)
- Can also deploy applications to an EC2 instance over multiple AZs
- Has six families of instances
	- General Purpose
	- Compute Optimized
	- Memory Optimized
	- Accelerated Computing
	- Storage Optimized
	- High Performance Computing Optimized
### Pricing
#### On Demand
- Fixed price billed by the *second*
- Use for workloads that cannot be predicted or interrupted
- For developing applications, or if workload won't last longer than a year
- Capacity reservations will hold capacity *whether or not* you run an instance
#### Spot
- Take advantage of unused EC2 capacity
- Use for workloads where stop and start times don't matter and the workload could be interrupted
- Very low compute pricing, up to 90% cheaper than On Demand
#### Dedicated Host
- Physical server that is fully dedicated to our instances
- Use when you bring your own server-bound software license like Microsoft or Oracle
- Look into regulatory corporate compliance requirements on tenancy and sharing instance with another company, no sharing with other customers
- Dedicated Instance is the app running on the Dedicated Host
- Up to 70% off On Demand prices
#### Reserved Instance
- Commit to a *specific* instance type for 1 to 3 years
- Use when you have steady state usage and can commit
- You must pay upfront
- Application requires a capacity reservation
#### Savings Plans
- Commit to compute usage for 1 to 3 years
- Measures per *hour*
- Use when you need to lower you bill across multiple compute services, OS, instance types, Regions
- No capacity reservations 
## 💡 Exam Tips
> [!important]
> Remember:
> - Know the pricing options
> - Understand the real world usage of EC2 (deploying database or web app)

---
*Notes Last Updated: 2025-02-14 14:26*