# NAT Gateway

Allow Outbound Internet Connectivity

# Challenge with Instance in Private Subnet

Since there is no Internet connectivity in Private subnet, the EC2 instance and application inside
it will not be able to perform any kind of patch updates, download new softwares etc.

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="80%">
</div>

## Overview of NAT Gateways

NAT Gateway allows instances in the private subnet to initiate a new connection towards the
Internet.
New connections from Internet cannot be established to instances in Private subnet.

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="80%">
</div>

# Working of NAT Gateway

<div align="center">
<img src="images/image3.png" alt="IAM Policies" width="80%">
</div>

## Example 2 - NAT Gateway

<div align="center">
<img src="images/image4.png" alt="IAM Policies" width="80%">
</div>
