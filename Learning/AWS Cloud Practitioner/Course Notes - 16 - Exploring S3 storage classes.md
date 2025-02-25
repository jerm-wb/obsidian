# Standard
- Primary storage used for frequently accessed data
- High throughput, low latency
# Intelligent-Tiering
- Dynamic storage used for data with unpredictable access patterns
- Automatically moves data between two access queues
- Designed for savings in storage cost without performance impact
# Infrequent Access
- Deeper storage used for data that is accessed less frequently but needs to be gotten quickly when needed
- Has a retrieval fee
## One Zone-Infrequent Access
- Infrequent access set up in only one Availability Zone, used for secondary backups or data that is easily reproducable
- More cost-effective than multi-zone options
# Glacier
## Instant Retrieval
- Even deeper storage designed to be used with archival data
- Low cost storage for long-life data
- Rarely accessed
## Flexible Retrieval
- Designed for archive data that is retrieved 1-2 times per year
- Lower cost
## Deep archive
- Deepest archival service, used for data that is basically never retrieved
- Lowest archival cost of all
# 💡 Exam Tips
> [!important]
> Remember:
> - Know the difference of retrieval times and fee differences between classes 
> - Know if there are one or more availability zones for data storage


---
*Notes Last Updated: 2025-02-25 11:47*