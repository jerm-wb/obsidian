#Regions  #AvailabilityZones
# AWS Regions
- A physical location, grouped by geographical locations
- Regions are isolated from each other
	- Resources are not shared between the regions and would need to be replicated manually across them
# Availability Zones
- **Official Definition**: One or more discrete data centers with redundant power, networking, and connectivity in an AWS region
- AWS Regions consist of multiple availability zones
- Each availability zone has one or more data center
## Characteristics of Availability Zones
- Housed separately, but connected through low-latency links
- If one AZ goes out, the rest are *not* affected
- Allows for high availability if an app is deployed on multiple AZs## AWS Regions
- A physical location, grouped by geographical locations
- Regions are isolated from each other
	- Resources are not shared between the regions and would need to be replicated manually across them
# 💡 Exam Tips
> [!important]
> Remember:
>- Region is global and is made up of two or more AZs
>- An AZ is made up of multiple data centers
>- Multi-AZ deployments provide high availability

---
*Notes Last Updated: 2025-02-14 13:54*