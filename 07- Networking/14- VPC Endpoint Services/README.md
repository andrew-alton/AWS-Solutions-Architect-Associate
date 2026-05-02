# VPC Endpoint Services

## Understanding the Basics

Organizations widely use many 3rd party solutions like Data Dog, New Relic etc
to create dashboards related to systems / application performance.
To create such dashboards, organization has to send appropriate metrics to 3rd
party servers.

<div align="center">
<img src="images/image1.png" width="75%">
</div>

## Understanding the Challenge

These system and applications metrics are generally sent via the Internet to 3rd
Party service provider servers.

<div align="center">
<img src="images/image2.png" width="75%">
</div>

## Better Solution - Internal Network

If both Consumers and Service Providers are hosted in AWS, these metrics can
be sent via AWS Private Network instead of the Internet.
This can provide many advantages related to cost, latency, and security.

<div align="center">
<img src="images/image3.png" width="75%">
</div>

## Possible Approach - VPC Peering

In this approach, the Consumer and Service Provider VPC can establish VPC
Peering and data can then be sent over Internal Network.

<div align="center">
<img src="images/image4.png" width="75%">
</div>

## VPC Peering is Not Practical

A Service provider can have thousands of customers.
There will be CIDR overlapping issues.

<div align="center">
<img src="images/image5.png" width="75%">
</div>

## Consumer Requirements

Consumer and Service Provider VPC should be able to communicate with each
other through AWS Internal Network without worrying about CIDR overlaps

## Introducing VPC Endpoint Services

Using Interface Endpoints, AWS allows connecting to the Service Provider VPC
The traffic flows through AWS Private Network.

<div align="center">
<img src="images/image6.png" width="75%">
</div>
