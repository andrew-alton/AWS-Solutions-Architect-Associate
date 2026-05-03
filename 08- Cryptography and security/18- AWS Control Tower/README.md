## Challenges with Multi-Account Environments
Most of the organizations follow a multi-account based architecture.
When the amount of AWS account increases, it leads to own set of challenges.

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="25%">
</div>

## Challenge 1 - Identity Management

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="25%">
</div>

## Solution 1 - Single Sign On

Single sign-on (SSO) is an authentication method that enables users to securely authenticate with
multiple applications and websites by using just one set of credentials.

<div align="center">
<img src="images/image3.png" alt="IAM Policies" width="25%">
</div>

## Challenge 2 - Security Hardening

<div align="center">
<img src="images/image4.png" alt="IAM Policies" width="25%">
</div>

## Solution 2 - Security Automation

AWS CloudFormation StackSets allows you to create, update, or delete stacks across multiple
accounts and Regions with a single operation

<div align="center">
<img src="images/image5.png" alt="IAM Policies" width="25%">
</div>

## Challenge 3 - Centralized Console

We need to have a centralized console that shows details of all AWS accounts, their security
compliance level, and other information

<div align="center">
<img src="images/image6.png" alt="IAM Policies" width="25%">
</div>

## AWS Control Tower
AWS Control Tower offers a straightforward way to set up and govern an AWS
multi-account environment, following the best practices.


<div align="center">
<img src="images/image7.png" alt="IAM Policies" width="25%">
</div>

## Centralized Logging

A comprehensive log management and analysis strategy is mission critical in an organization.
It enables the organizations to understand the relationship between operational, security,
and change management events and maintain a comprehensive understanding of their
infrastructure.

<div align="center">
<img src="images/image8.png" alt="IAM Policies" width="25%">
</div>