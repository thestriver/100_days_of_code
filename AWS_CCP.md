<h2>Cloud Concepts</h2>

**AWS Cloud Value Framework**
a. Cost Savings - Total Cost of Ownership (TCO) reduction
b. Staff Productivity
c. Operational Resilience d. Business Agility

Six Advantages and Benefits of Cloud Computing

Types of Cloud Computing - SaaS , PaaS and IaaS

Cloud Computing Deployment Models - Cloud, Hybrid, On-Premise

---------------

<h2>AWS Global Infrastructure - (Technology) </h2>

Map Overview

Regions

Availability Zones - 25 Launched Regions (geographically distinct), 80 Availability Zones , 218+ Edge Locations
AZs are physically separated by a meaningful distance, many kilometers, from any other AZ, although all are within 100 km (60 miles) of each other. and **<10ms latency between AZs**  

Edge Locations - Owned by Trsuted partner/serve requests for Cloudfront and Route 53. Sometimes also used by S3 Transfer Acceleration and API Gateway. 
Reliable, **low latency** and high throughput network connectivity

GovCloud Regions - host sensitive Controlled Unclassified Information

---------------

Creating an AWS Account
Billing Preferences, Budgets and Alarms
Change IAM Users Sign-in Link
Activate MFA on Root Account
Create individual IAM user
Set a password policy

---------------
Hands On

Regions

**EC2(Elastic Compute Cloud) - Virtual servers in the cloud** : 
Amazon Machine Image (AMI) / IAM roles /storage - Free tier eligible customers can get up to 30 GB of EBS General Purpose (SSD) or Magnetic storage.

Sessions Manager

AMI

Auto Scaling GroupsAmazon:  EC2 Auto Scaling
helps maintain the availability of your applications
Auto Scaling groups are collections of Amazon EC2 instances that enable automatic scaling and fleet management features. These features help you maintain the health and availability of your applications.

Elastic Load Balancer:
3 types - Application, Network, Gateway load and Classic 

S3: Simple Storage Service - Scalable storage in the cloud

CloudFront - Global CDN(Content Distibution Network)

RDS - Relational Database Service

Lambda - Run code without thinking about provisioning or managing servers or clusters / runtime limit - 15 minutes

---------------

<h2>EC2 Pricing Models</h2>

<u>On-Demand(default)</u>: **no long term commitment / no upfront payment**

**for short-term,spikey or unpredictable workloads**

pay per hour or minute/
low-cost& flexible/
suitable for first time apps


<u>Reserved</u> :(reserved instances) for stable apps with predictable usage. Reduced Pricimg = Term x Class Offering x Payment Option

**commitment to 1 or 3 Year contract** &
payment options are **Upfront/Partial-upfront or no upfront**

**best option for longterm**

<u>Spot instances</u>: Biggest savings(90%)
Suitable for flexible apps with flexible start and end who use idle AWs servers given out on the spot.

**Instances can be cancelled at anytime by AWS and you don't get charged by them for a partial hour usage. You however get charged for an hour if you cancel a partial hour usage yourself**


<u>Dedicated Host Instances</u>: (Most expensive)
for users with strict licensing (e.g regulatory) option which comes in On-Demand or Reserved flavours.

**Multi-tenant(virtual isolation) vs Single tenant (physical isolation)**


---------------

<h2>Billing and Pricing</h2>

Free Services - N.B some of these free services are free but they can setup services that are paid e.g **CloudFormation**, Amplify. Beanstalk 

AWS Support Plans: **Four -Basic, Developer, Business and Enterprise**

Basic - email support only for billing and account at $0 per month

Developer - within 24 hr response email support with no third party support at $20/month

Business - within 24hr response email support with chat or phone third party support at $100/month

Enterprise - within 24hr response email support with chat or phone third party support and a personal conceirge and TAM  at $15000/month.

*Key response times*:
**System Impaired < 12hr / Production system impaired < 4hr / Production system down < 1hr / Enterprise critical system down response time of <15m.

AWS Marketplace

<u>AWS Trusted Advisor </u> - (advice on **saving money**, performance, fault tolerance). 7 for Free & developer , All for Business and Enterprise <br>
Cost Optimization - e.g  idle Load Balancers & Unassociated Elastic IP addresses <br>
Performance - High Utilization Amazon EC2 Instances
Security - MFA on Root Account, IAM Access Key rotations 
Fault Tolerance - Amazon RDS Backups
Service Limits - VPC 

Consolidated Billing - all charges consolidated into **one bill**
The **master account** can pay the expenses of member account and you can use the cost explorer to visualize the costs.

Consolidated Billing Volume Discounts

AWS Cost Explorer

AWS Budgets: first 2 budgets are free. subsequent are $0.02 per day / 20,000 budgets limit
Cost, usage and reservation budgets. Alerts support EC2, RDS, Redshift, ElasticCache etc. 

TCO Calculator

AWS Landing Zone - helps **Enterprises** quickly set up AWS multi-account architecture via *AWS AVM(Account Vending Machine)

Resource Groups and Tagging
 - *Tags* are words/phrases that act as metadata for organizing AWS *resources* while *Resource groups* are a collection of resources that share one or more tags. RG show details about metrics, alarms and Config setiings.

AWS QuickStart: 3 parts
 - 1. reference achictecture 2. CloudFormation Templates 3. Deployment guide

AWS Cost and Usage Report
- generate detailed spreadsheet that are placed in **S3** & can be queried as a database using **Athena** and/or visualized as graphs using **Quicksight** 

---------------
---------------
---------------

<h2>Technology Overview</h2>
AWS Organizations and Accounts: Service control policies gives you control permissions over all accounts in the organization.

AWS Networking

Database Services

Provisioning Services

Computing Services

Storage Services

Business Centric Services

Enterprise Integration

Logging Services

Know your Initialisms

---------------
---------------
---------------

<h2>AWS Security</h2>
Shared Responsibility Model
AWS Compliance programs
AWS Artifact
AWS Artifact Follow Along
Amazon Inspector
AWS WAF
AWS Shield
Penetration Testing
Guard Duty
Key Management Service
Amazon Macie
Security Groups vs NACLs
AWS VPN

---------------

Variation Study
Cloud* Service
*Connect Service
Elastic Transcoder vs Media Convert
SNS vs SQS
Inspector vs Trusted Advisor
ALB vs NLB vs CLB
SNS vs SES
Artifact vs Inspector