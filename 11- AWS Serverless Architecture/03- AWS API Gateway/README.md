
<div align="center">
<img src="images/image7.png"  width="10%">
</div>

# API Gateway

APIs act as the "front door" for applications to access data, business logic, or
functionality from your backend services.

Hence API should be able to be highly available and handle thousands of
requests.

<div align="center">
<img src="images/image1.png"  width="75%">
</div>

Amazon API Gateway is a fully managed service that makes it easy for
developers to create, publish, maintain, monitor, and secure APIs at any scale.

<div align="center">
<img src="images/image2.png"  width="75%">
</div>

# API Gateway Practical

1- Create HTTP API

2- API will invoke a backend Lambda function.

<div align="center">
<img src="images/image8.png"  width="75%">
</div>

Depending on where the majority of your API traffic originates from, you can
create a appropriate API Gateway endpoint type.

![My Image](images/image3.png)

An edge-optimized API endpoint is best for geographically distributed clients.
API requests are routed to the nearest CloudFront Point of Presence (POP).
This is the default endpoint type for API Gateway REST APIs.

![My Image](images/image4.png)

A regional API endpoint is intended for clients in the same region.
When a client running on an EC2 instance calls an API in the same region, or
when an API is intended to serve a small number of clients with high demands,
a regional API reduces connection overhead.

![My Image](images/image5.png)

A private API endpoint is an API endpoint that can only be accessed from your
Amazon Virtual Private Cloud (VPC) using an interface VPC endpoint.

![My Image](images/image6.png)
