# Network Load Balancers

## Setting the Base

Not ALL applications support HTTP protocol.
Example: DNS servers, SMTP server, FTP servers, SSH servers etc.

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="75%">
</div>

## Requirement of Additional Load Balancer Type

There is a requirement of additional load balancer types that works for
non-HTTP based protocols.

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="75%">
</div>

## Setting the Base

A Network Load Balancer operates at the layer 4 (Transport Layer) of the OSI
model.
It can handle millions of requests per second.

<div align="center">
<img src="images/image3.png" alt="IAM Policies" width="75%">
</div>

## Supported Protocols

Network Load Balancer target groups support following protocols.

<div align="center">
<img src="images/image4.png" alt="IAM Policies" width="75%">
</div>

## Reference Screenshot - Supported Protocols for NLB

<div align="center">
<img src="images/image5.png" alt="IAM Policies" width="75%">
</div>

## Points to Note

For TCP traffic, the load balancer selects a target using a flow hash algorithm
based on the protocol, source IP address, source port, destination IP address,
destination port, and TCP sequence number.

For UDP traffic, the load balancer selects a target using a flow hash algorithm
based on the protocol, source IP address, source port, destination IP address,
and destination port.
