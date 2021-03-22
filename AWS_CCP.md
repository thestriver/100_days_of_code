**Cloud Concepts**

What is Cloud Computing?
Six Advantages and Benefits of Cloud Computing
Types of Cloud Computing - SaaS , PaaS and IaaS
Cloud Computing Deployment Models - Cloud, Hybrid, On-Premise

---------------

**AWS Global Infrastructure** - (Technology)

Map Overview

Regions

Availability Zones - 25 Launched Regions (geographically distinct), 80 Availability Zones , 218+ Edge Locations
AZs are physically separated by a meaningful distance, many kilometers, from any other AZ, although all are within 100 km (60 miles) of each other. and **<10ms latency between AZs**  

Edge Locations - Owned by Trsuted partner/serve requests for Cloudfront and Route 53. Sometimes also used by S3 Transfer Acceleration and API Gateway. 
Reliable, **low latency** and high throughput network connectivity

GovCloud Regions - host sensitive Controlled Unclassified Information

---------------
Getting Started
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

EC2 Pricing Models

<u>On-Demand(default)</u>: **no long term commitment / no upfront payment**

**for short-term,spikey or unpredictable workloads**

pay per hour or minute/
low-cost& flexible/
suitable for first time apps


<u>Reserved</u> :(reserved instances) for stable apps with predictable usage 
**commitment to 1 or 3 Year contract** &
payment options are **Upfront/Partial-upfront or no upfront**

best option for longterm

<u>Spot instances</u>: Biggest savings(90%)
Suitable for flexible apps with flexible start and end who use idle AWs servers given out on the spot.

**Instances can be cancelled at anytime by AWS and you don't get charged by them for a partial hour usage. You however get charged for an hour if you cancel a partial hour usage yourself**


Dedicated

EC2 Pricing CheatSheet

---------------
️Billing and Pricing
Free Services
AWS Support Plans
Follow Along - Lets create a support case
AWS Marketplace
Follow Along - Marketplace subscription
AWS Trusted Advisor
Follow Along Trusted Advisor
Consolidated Billing
Consolidated Billing Volume Discounts
AWS Cost Explorer
AWS Cost Explorer Follow Along
AWS Budgets
AWS Budgets Follow Along
TCO Calculator
TCO Calculator Follow Along
AWS Landing Zone
Resource Groups and Tagging
Resource Groups Follow Along
AWS QuickStart
AWS Cost and Usage Report
Cost and Usage Follow Along

---------------

Technology Overview
AWS Organizations and Accounts
AWS Organizations Follow Along
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
AWS Security
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