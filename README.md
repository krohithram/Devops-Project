# About the Project
- Multi Tier Web Application Stack
- Re-Architect Services for AWS Cloud
- Architecture to boost agility or impove business continuity.

## Scenario
- Project services running on Physical/Virtual/Cloud machines EC2.
- Various of services like Nginx, Tomcat, Mysql, RabbitMQ & Memcached.

## Problem
- Operational Overhead
- Uptime & Scaling
- Manual Process

## Solution
- Cloud Setup - PAAS & SAAS 

- AWS Services

- Beanstalk - VM for Tomcat, Nginx LB Replacement, Automation for VM scaling
- S3/EFS - Storage for Artifact
- RDS - For Database PAAS to replace Mysql on VM
- Elastic Cache - To replace Memcached
- Active MQ - To replace RabbitMQ
- Route53 - For DNS
- Cloudfront - For Content Delivery Network

- EC2 Instances, ELB, Autoscaling, S3, RDS, Elastic Cache, Active MQ, Route53 Cloudfront

## Flow of Execution

- Create Key Pair for Beanstalk Instances Login.
- Create Security Group for Elastic Cache, RDS & Active MQ.
- Create Services RDS, Amazon Elastic Cache & Amazon Active MQ.
- Create Elastic Beanstalk Environment.
- Update SG of Backend to allow traffic from Bean-SG.
- Update SG of Backend to allow internal traffic.

- Launch EC2 Instance for DB Initializing
- Login to the instance and Initialize RDS DB
- Change health check on Beanstalk to "/login"
- Add 443 hhtps Listiner to ELB
- Build Artifact with Backend Information
- Deploy Artifact to Beanstalk
- Create CDN with SSL Cert
- Update Entries in GoDaddy DNS Zones
- Test the URL.


