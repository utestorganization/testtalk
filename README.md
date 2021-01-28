#### Version 1.0

# SCloud SLA 

**Last Updated** 19 Jan. 2021

This Service Level Agreement (this “SLA”) applies to the Service(s) that are used by the Customer ("you" or "your"), and is an integral part of your SCloud End User Licence Agreement (the “Customer Agreement”). Capitalized terms used in this SLA are as defined in the Customer Agreement unless otherwise stated in this SLA. Should there be any conflict or inconsistency between this SLA and the Customer Agreement, this SLA shall prevail to the extent of such conflict or inconsistency.

SCloud may modify the terms of this SLA from time to time in its sole and absolute discretion. The modified SLA will be uploaded on SCloud's website and will apply from the effective date stated therein. Your continued use of the Services following the effective date of the modified SLA represents your consent and agreement to the modified SLA, and acceptance of the terms therein. If you disagree with the modified SLA, you may cease using the Services, subject to the termination provisions in the Customer Agreement.

Except as set forth in the respective paragraphs relating to each Service below, or as otherwise stated in your Order Form, no service credits or other remedy (financial or otherwise) shall be provided to you due to the failure to meet a specified service level or standard for a specific Service.

## General Terms

### **1.** **Definitions**

- **“Service Cycle”** means a natural month.

- **“Total Time of Service Cycle”** means the total minutes during every Service Cycle.

- **“Service Unavailable”** will be defined for each Service in the Service Specific Terms thereafter. Service Unavailable does not include the situation that Cloud Service is unavailable due to the disclaimers described blow and disclaimers in the following service specific terms.

- **“Service Unavailable Duration”** means all the time when the Service is unavailable during a Service Cycle. If the duration is less than one month, it is still regarded as one month. Service Unavailable Duration cannot be calculated more than once. Every Service Unavailable Duration cannot be calculated again after the compensation being applied for.

- **“Service Availability”** means during a Service Cycle, the service available percentage per Service Cycle achieved by the Cloud Service given in this SLA.

- **“Monthly Service Fee”** means service fees paid by customers for the Services in a Service Cycle. For example, if the customer pays the service fee of several months at a time, the Monthly Service Fee is calculated as the total service fees paid divided by the total number of month.

  

### **2.** **Service Credit**

**Service Credit:** Service Credits are your sole and exclusive remedy for any performance or availability issues for any Service under the Agreement and this SLA. You may not unilaterally offset your Applicable Monthly Service Fees for any performance or availability issues.

Service Credits apply only to fees paid for the particular Service, Service Resource, or Service tier for which a Service Level has not been met. In cases where Service Levels apply to individual Service Resources or to separate Service tiers, Service Credits apply only to fees paid for the affected Service Resource or Service tier, as applicable. The Service Credits awarded in any billing month for a particular Service or Service Resource will not, under any circumstance, exceed your monthly service fees for that Service or Service Resource, as applicable, in the billing month.

If you purchased Services as part of a suite or other single offer, the Applicable Monthly Service Fees and Service Credit for each Service will be pro-rated.

If you purchased a Service from a reseller, you will receive a service credit directly from your reseller and the reseller will receive a Service Credit directly from us. The Service Credit will be based on the estimated retail price for the applicable Service, as determined by us in our reasonable discretion.



**Time limit for application:** you can apply for service credit in each Service Cycle after the bill are settled. The application must be filed within two (2) months after the end of the Service Cycle in which the incident that’s the subject of the claim occurred. Applications beyond the time limit will not be accepted. SCloud Cloud will make a reasonable assessment of all information provided to us and make a good faith decision on whether the service credit is owned.



### **3.** **Disclaimers**

This SLA does not apply to any performance and availability issues:

a. caused by force majeure;

b. that arise during the period when your Services are suspended or terminated according to the Customer Agreement;

c. caused by you or any third party;

d. caused by daily service maintenance;

e. that arise due to your failure to comply with the operation guidance of the Services;

f. caused by a serious problem of the network operator.



##  **Service-Specific Terms**

**General service levels for the Services**

| **Monthly Uptime Percentage** | **Monthly**    |
| ----------------------------- | -------------- |
| < 99.95%                      | 21m 54 s       |
| < 99.9%                       | 43m 49 s       |
| < 99%                         | 7h 18m 17 s    |
| < 95%                         | 1d 12h 31m 27s |



### **1. Cloud Server (HOST)**

Definitions

**Cloud Server Unavailability** means the Cloud Server (HOST) system log shows that SHOST was inaccessible for one (1) or more consecutive minutes because of errors or incidents caused by SCloud.

Disclaimers

These service levels do not apply to any performance or availability issues: 

1) Alteration, corruption, loss, or destruction of data kept by local disks, for example, the data of disk-intensive, ultra-high I/O and/or GPU-accelerated HOST stored in a local disk may be lost due to the damage of that disk.

2) Caused by your operations such as stopping or restarting HOST instances or detaching cloud disks on the console, through APIs, at the command-line interface (CLI), or by other means.

Service Availability

**Service Availability Rate in each Service Cycle calculation formula:**

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

**Service Availability Rate commitment:**

SCloud will use commercially and technically reasonable efforts to make the Service Availability Rate of Cloud Server Unavailability per Service Cycle no less than 99.95%; 

Service Credit

If SCloud fails to meet the commitment above on Compute Service availability rate, SCloud will provide you with with Service Credits in accordance with the rates below:



| **Monthly Uptime Percentage**           | **Service Credit**          |
| --------------------------------------- | --------------------------- |
| 99% ≤ Service Availability Rate <99.95% | 10% of Monthly Service Fee  |
| 95% ≤ Service Availability Rate <99%    | 15% of Monthly Service Fee  |
| Service Availability Rate <95%          | 100% of Monthly Service Fee |



### **2. Elastic IP (EIP)**

Definition

**Service Unavailability** means the Elastic IP (EIP) system log showing that all data packets in the outbound direction are discarded at the SCloud gateway for one (1) or more consecutive minutes due to the fault of SCloud Cloud.

Disclaimers

This SLA does not apply to any performance or availability issues:

1)   caused by hacker attacks on your applications, including but not limited to DDoS attacks.

2)   caused by a faulty backend server.

3)   caused by network operators.

Service Availability

Service Availability Rate in each Service Cycle is represented by the following formula:

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration)/Total Time of Service Duration * 100%

Service Availability Rate commitment:

SCloud will use commercially and technically reasonable efforts to make the Service Availability Rate of EIPs per Service Cycle no less than 99.95%

Service Credit

If SCloud fails to meet the above commitment, SCloud will provide you with Service Credits in accordance with the rates below:


 EIPs:

| **Monthly Uptime Percentage**            | **Service Credit**         |
| ---------------------------------------- | -------------------------- |
| 98% ≤ Service Availability Rate < 99.95% | 10% of Monthly Service Fee |
| Service Availability Rate < 98%          | 20% of Monthly Service Fee |



### **3. Content Delivery Network (CDN)**

Definitions

**Number of 5xx response errors in five minutes:** Number of 5xx errors returned by the domain name due to CDN system problems in five minutes.

**Number of failed requests due to node unavailability in five minutes:** If a node is unavailable, calculate the number of requests per five minutes based on the statistics of the first seven days, and then convert it to the number of failed requests due to node unavailability in five minutes.

Error in five minutes = (Number of 5xx response error in five minutes + Number of failed requests due to node unavailability in five minutes) / Total number of requests in five minutes of the domain name

**"Service Unavailability"** means the CDN system log shows that the error rate of CDN was greater than 0.05% within five (5) minutes for longer than consecutive 10 minutes because of SCloud Cloud.

Disclaimers

If you will have a sharp increase in CDN bandwidth usage (greater than or equal to 30% of the billed bandwidth for last month), you must submit a service ticket to inform SCloud at least three (3) business days in advance. Otherwise, SCloud will not be responsible for service unavailability resulting from this.

Service Availability

**Service Availability Rate in each Service Cycle calculation formula:**

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

**Service Availability Rate commitment:**

SCloud will use commercially and technically reasonable efforts to make the Service Availability Rate of CDN per Service Cycle not less than 99.9%.

Service Credit

If SCloud fails to meet the above commitment, SCloud will provide you with Service Credits in accordance with the rates below:

| **Monthly Uptime Percentage**        | **Service Credits** |
| ------------------------------------ | ------------------- |
| 99%≤Service Availability Rate <99.9% | 10%                 |
| Service Availability Rate <99%       | 15%                 |





### **4. Relational Database Service (RDS)**

Definition

**Service Unavailability** means the RDS system log shows that a DB instance was inaccessible for one (1) or more consecutive minutes because of SCloud.

Service Availability

**Service Availability Rate in each Service Cycle calculation formula:**

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

**Service Availability Rate commitment:**

SCloud will use commercially and technically reasonable efforts to make the Service Availability Rate of Primary/standby (1/2) DB instances per Service Cycle no less than 99.99%; and Primary/standby DB instances per Service Cycle no less than 99.95%;

Service Credit

If SCloud fails to meet the commitment above on RDS Service Availability Rate, SCloud will provide you with Service Credits in accordance with the rates below: 

| **Monthly Uptime Percentage**                      | **Service Credit**          |
| -------------------------------------------------- | --------------------------- |
| 99.0% ≤ Service Availability Rate <99.95%          | 10% of Monthly Service Fee  |
| Less than 99.0% but equal to or greater than 95.0% | 30% of Monthly Service Fee  |
| Less than 95.0%                                    | 100% of Monthly Service Fee |



### **6. Memcache (SMEM)**

Definition

Service Unavailability means the SMEM was inaccessible for one (1) or more consecutive minutes because of SCloud.

Service Availability

Service Availability Rate in each Service Cycle calculation formula:

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

Service Commitment

SCloud will use commercially reasonable efforts to make SMEM available with a Monthly Uptime Percentage of at least 99.95% (the "Service Commitment"). In the event a SMEM does not meet the Service Commitment, you will be eligible to receive a Service Credit as described below.

Service Credit

Service Credits are calculated as a percentage of the total charges paid by you for the affected SMEM for the monthly billing cycle in which the Service Commitment was not met, in accordance with the schedule below:

| **Monthly Uptime Percentage**                      | **Service Credit**          |
| -------------------------------------------------- | --------------------------- |
| 99.0% ≤ Service Availability Rate <99.95%          | 10% of Monthly Service Fee  |
| Less than 99.0% but equal to or greater than 95.0% | 30% of Monthly Service Fee  |
| Less than 95.0%                                    | 100% of Monthly Service Fee |



### **7. Storage Service** 

Definition

**Service Unavailability** means the UDISK system log shows that UDISK was inaccessible for five (5) or more consecutive minutes because of SCloud Cloud.

Service Availability

**Service Availability Rate in each Service Cycle calculation formula:**

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

Service Commitment

SCloud will use commercially reasonable efforts to make the Included Services each available for each SCloud region with a Monthly Uptime Percentage of at least 99.95%, in each case during any monthly billing cycle (the “Service Commitment”). In the event any of the Included Services do not meet the Service Commitment, you will be eligible to receive a Service Credit as described below.

Service Commitments and Service Credits

Service Credits are calculated as a percentage of the total charges paid by you for the applicable Included Service in the affected SCloud region for the monthly billing cycle that did not meet the Service Commitment in accordance with the schedule below.

| **Monthly Uptime Percentage**             | **Service Credit**         |
| ----------------------------------------- | -------------------------- |
| 95.0% ≤ Service Availability Rate <99.95% | 10% of Monthly Service Fee |
| Less than 95%                             | 20% of Monthly Service Fee |



### **8. Object Storage Service** 

Definition

**Service Unavailability** means the UF3 system log shows that UF3 was inaccessible for five (5) or more consecutive minutes because of SCloud Cloud.

Service Availability

**Service Availability Rate in each Service Cycle calculation formula:**

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

Service Availability Rate commitment: 

SCloud will use commercially and technically reasonable efforts to make the Service Availability Rate of data stored in UF3 storage per Service Cycle no less than 99.95%; and Cloud Archive/Infrequency Access Storage per Service Cycle no less than 99.9%.

Service Credit

If SCloud fails to meet the commitment above on Object Storage Service Availability Rate, SCloud will provide you with Service Credits in accordance with the rates below, according to different storage classes in different AZ deployment: 

**Data stored in UF3 Storage:** 

| **Monthly Uptime Percentage**          | **Service Credit**         |
| -------------------------------------- | -------------------------- |
| 99% ≤Service Availability Rate <99.95% | 10% of Monthly Service Fee |
| 95%≤Service Availability Rate <99%     | 15% of Monthly Service Fee |
| Service Availability Rate <95%         | 20% of Monthly Service Fee |



**Cloud Archive/Infrequency Access Storage:**

| **Monthly Uptime Percentage**        | **Service Credit**         |
| ------------------------------------ | -------------------------- |
| 95%≤Service Availability Rate <99.9% | 10% of Monthly Service Fee |
| Service Availability Rate <95%       | 15% of Monthly Service Fee |
|                                      |                            |



### **9. Advanced Anti-DDoS (AAD)**

Definition

**Service Unavailability** is the status that an AAD system was inaccessible and incapable of forwarding traffic for five (5) or more consecutive minutes. Duration of the inaccessibility and incapability that lasts shorter than five (5) minutes shall not be included.

Disclaimers

These service levels do not apply to any performance or availability issues: 

1) Due to security threats or fraud or illegal acts caused by you or your end users to the Services;

2) Issues in the back-end origin server, such as fully occupied bandwidth, exposed IP address, data center faults, and/or link jitter;

3) Black holes caused by attack traffic exceeding your purchased AAD capability.

Service Availability

**Service Availability Rate in each Service Cycle calculation formula:**

Service Availability Rate in each Service Cycle = (Total Time of Service Duration - Service Unavailable Duration) / Total Time of Service Duration * 100%

**Service Availability Rate commitment:**

SCloud will use commercially and technically reasonable efforts to make the Service Availability Rate of AAD per Service Cycle not less than 99.9%.

Service Credit

If SCloud fails to meet the above commitment, SCloud will provide you with Service Credits in accordance with the rates below:

| **Monthly Uptime Percentage**        | **Service Credits**        |
| ------------------------------------ | -------------------------- |
| 95%≤Service Availability Rate <99.9% | 10% of Monthly Service Fee |
| Less than 99.5%                      | 15% of Monthly Service Fee |
