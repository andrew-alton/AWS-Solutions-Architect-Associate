# VPC Peering

"Let’s Route"

## VPC Peering

VPC peering is a network connection between two VPC that enables the communication
between instances of both the VPC.

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="80%">
</div>

## Architecture - 1

- First VPC - 172.31.0.0/16
- Secondary VPC - 10.77.0.0/16

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="80%">
</div>

## Architecture - 2

<div align="center">
<img src="images/image3.png" alt="IAM Policies" width="80%">
</div>

## Things to Remember

- VPC Peering is now possible between regions.
- VPC Peering does not act like a Transit VPC

<div align="center">
<img src="images/image4.png" alt="IAM Policies" width="80%">
</div>

## Unsupported VPC Peering Configurations - 1

You cannot create a VPC peering connection between VPCs with matching or
overlapping IPv4 CIDR blocks.

<div align="center">
<img src="images/image5.png" alt="IAM Policies" width="80%">
</div>

## Unsupported VPC Peering Configurations - 2

You have a VPC peering connection between VPC A and VPC B (pcx-aaaabbbb), and
between VPC A and VPC C (pcx-aaaacccc).
There is no VPC peering connection between VPC B and VPC C. You cannot route
packets directly from VPC B to VPC C through VPC A.

<div align="center">
<img src="images/image6.png" alt="IAM Policies" width="80%">
</div>
