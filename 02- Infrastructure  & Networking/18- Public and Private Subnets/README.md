# Public and Private Subnets

## Public Subnet

Public subnet is a subnet that is associated with an Internet Gateway.
This subnet is recommended if you want to run a public-facing web application.
Overall Security Risk: High

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="80%">
</div>

## Private Subnet

Private subnets are the ones that do not have an Internet Gateway attached to it.
No New connections from the Internet can reach to the EC2 instances within the private
subnet.

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="80%">
</div>

## Benefits of Private Subnet

Since internet connectivity is not present, it is much more difficult by an attacker to attack
the system in private subnet directly.

<div align="center">
<img src="images/image3.png" alt="IAM Policies" width="80%">
</div>

## Important Note

Even though the EC2 instance are in private subnet, the local level communication between
EC2 in public and private will still work using private IPs.

<div align="center">
<img src="images/image4.png" alt="IAM Policies" width="80%">
</div>

## The Network Architecture

<div align="center">
<img src="images/image5.png" alt="IAM Policies" width="80%">
</div>

## Public Subnet Configuration

Following is true for Public Subnet:

1. Internet Gateway is Attached to VPC
2. Route Table has route towards Internet Gateway.

<div align="center">
<img src="images/image6.png" alt="IAM Policies" width="80%">
</div>

## Private Subnet Configuration

Following is true for Private Subnet:
Route Table does not have a route towards Internet Gateway.

<div align="center">
<img src="images/image7.png" alt="IAM Policies" width="80%">
</div>

## Steps to Configure Public and Private Subnet

There will be 2 route tables: One for Public Subnet and Second for Private Subnet.

<div align="center">
<img src="images/image8.png" alt="IAM Policies" width="80%">
</div>
