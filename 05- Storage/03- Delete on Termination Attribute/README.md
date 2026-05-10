# Delete on Termination Attribute

## Revising the Basics

Since EBS and EC2 are separate set of entities, they can live independently of
each other.

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="80%">
</div>

## Basics of Deletion Attribute

When an instance terminates, the value of the DeleteOnTermination attribute
for each attached EBS volume determines whether to preserve or delete the
volume.

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="80%">
</div>
