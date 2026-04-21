# Gateway VPC Endpoints

## Gateway Endpoints Architecture

A gateway endpoint targets specific IP routes in VPC route table, in the form of a
prefix-list, used for traffic destined to DynamoDB or S3.

<div align="center">
<img src="images/image1.png" width="75%">
</div>

## Supported Services

Gateway VPC Endpoints supports only S3 and DynamoDB Service.

<div align="center">
<img src="images/image2.png" width="75%">
</div>

## Prefix list for Endpoint

This prefic list contain all the CIDR ranges related to S3 service for the region to automatically route the traffic via the Gateway endpoint.

<div align="center">
<img src="images/image3.png" width="75%">
</div>
