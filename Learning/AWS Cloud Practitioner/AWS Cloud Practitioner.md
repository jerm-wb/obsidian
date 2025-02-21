# Table of Contents
%% Begin Waypoint %%
- [[Course Notes - 01 - Getting your head in the cloud]]
- [[Course Notes - 02 - Cloud computing and deployment models]]
- [[Course Notes - 03 - Exploring regions and availability zones]]
- [[Course Notes - 04 - Reviewing edge locations and local zones]]
- [[Course Notes - 05 - Introducing the Frameworks]]
- [[Course Notes - 06 - AWS Management Console and accessing AWS]]
- [[Course Notes - 07 - Compute]]
- [[Course Notes - 08 - EC2 Connection Methods & Demo]]
- [[Course Notes - 09 - Containers]]
- [[Course Notes - 10 - Serverless services in AWS]]
- [[Course Notes - 11 - Serverless services pricing & features]]
- [[Course Notes - 12 - Introducing additional compute services]]
- [[Course Notes - 13 - Exam Tips - Compute technology and service]]

%% End Waypoint %%

```dataview
TABLE 
length(rows.file.tags) as "Usage Count"
FROM "wb/Learning/AWS Cloud Practitioner"
FLATTEN file.tags as tags
GROUP BY tags
SORT length(rows.file.tags) desc
```
