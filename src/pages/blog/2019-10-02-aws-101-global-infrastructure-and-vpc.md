---
templateKey: blog-post
title: 'AWS 101: Global Infrastructure and VPC'
date: '2019-10-02 14:45'
featuredpost: true
featuredimage: /img/tutorials.png
tags:
  - AWS
  - AWS101
---
## AWS Region
* An AWS Region is a geographical location. Every region is physically isolated from and independent of every other region in terms of location, power, water supply, etc.
* Inside each region, there are two or more availability zones with each AZ hosted in separate data centers from another zone.
* The level of region isolation is critical for workloads with compliance and data sovereignty requirements where guarantees must be made that user data does not leave a particular geographic region. 
* The presence of AWS regions worldwide is also important for workloads that are latency-sensitive and need to be located near users in a particular geographic area.
* When you create certain resources in a region, you will be asked to choose a zone in which to host that resource.

## AWS availability zones
* An availability zone is a **_logical data center_** in a region.
* logical because there can be multiple data center in 1 AZ.
* In each AZ, all data centers are connected to each other over redundant low-latency private network links. 
* Likewise, all AZ in a region communicate with each other over redundant private network links. These intra and inter-zone links are heavily used for data replication by a number of AWS services including storage and managed databases.
* AZ is an important and foundational concept for building a highly available, fault-tolerant application using AWS.
