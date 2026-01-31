# EC2 Pricing Considerations

EC2 Pricing
Your Amazon EC2 usage is calculated by either the hour or the second based on
the size of the instance, operating system, and the AWS Region where the
instances are launched.
Each partial instance-hour consumed is billed per-second for instances launched
in Linux, Windows, or Windows with SQL Enterprise, SQL Standard, or SQL
Web instances.

<div align="center">
<img src="images/image1.png" alt="IAM Policies" width="80%">
</div>

## Pricing for Instance in Stopped State

If the EC2 instance is in stopped state, you will not get billed for it.
Many organizations automatically stop their EC2 during weekends and start on
Monday.
Note: EC2 can also have backend storage which will be charged even if EC2 is
stopped.
AWS Free Tier includes 30 GB of storage
