# Elastic Block Store (EBS)

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="10%">
</div>

## Simple Use-Case: External Hard Disk

External Hard Disk can be attached to the Workstation and detached whenever
required (portable)
Depending on the use-case, you can buy external storage of different
configuration based on size, performance and others.

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="50%">
</div>

## Understanding the Basics

Elastic Block Store (Amazon EBS) is a scalable, high-performance block-storage
service designed for Amazon EC2.
These volumes can be attached and detached from EC2 instance.

<div align="center">
<img src="images/image3.png" alt="IAM Policies" width="50%">
</div>

## EBS is Network Storage

EBS volumes are attached to EC2 instance through Network.
There can be latency that might be involved.

<div align="center">
<img src="images/image4.png" alt="IAM Policies" width="50%">
</div>

## Availability Zone Specific

You create an EBS volume in a specific Availability Zone, and then attach it to an
instance in that same Availability Zone.
Cross Availability Zone based attachment is not supported.

<div align="center">
<img src="images/image5.png" alt="IAM Policies" width="50%">
</div>

## EC2 and EBS Attachment

One EC2 instance can be attached with multiple set of EBS volumes of different
sizes.

<div align="center">
<img src="images/image6.png" alt="IAM Policies" width="50%">
</div>
