# IAM Policies - JSON policy document structure

## Understanding the Basics

It is important for us to be able to understand to read and write JSON policies
effectively

<img src="images/image1.png"  width="75%">
</div>

### Basic about JSON Policy

Most policies are stored in AWS as JSON documents.
These include:

- Identity-based policies
- Resource-based policies
- Service Control Policies
- Session policies

## Understanding the Basic Structure

As illustrated in the following figure, a JSON policy document includes these
elements:

<img src="images/image2.png"  width="75%">
</div>

## Comparison - Policy to Structure

<img src="images/image3.png"  width="75%">
</div>

| Elements              | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| Version               | Specify the version of the policy language that you want to use. AWS recommends that you use the latest `2012-10-17` version. |
| Statement             | Use this main policy element as a container for the following elements.    |
| Sid (Optional)        | Include an optional statement ID to differentiate between your statements. |
| Effect                | Use `Allow` or `Deny` to indicate whether the policy allows or denies access. |
| Principal             | Not required for IAM policies attached to a user or role. For resource-based policies, you must specify the account, user, role, or federated user to allow or deny access. |
| Action                | Include a list of actions that the policy allows or denies.                |
| Resource              | If you create an IAM permissions policy, you must specify a list of resources to which the actions apply. |
| Condition (Optional)  | Specify the circumstances under which the policy grants permission.        |

## Importance of ARNs

Amazon Resource Names (ARNs) uniquely identify AWS resources.

<img src="images/image4.png"  width="75%">
</div>

### example

<img src="images/image5.png"  width="75%">
</div>

### Reference Policy 1

Allows full RDS database access within a specific Region

<img src="images/image6.png"  width="75%">
</div>

### Reference Policy 2

This policy restricts access to actions that occur between April 1, 2020 and June
30, 2020 (UTC), inclusive

<img src="images/image7.png"  width="75%">
</div>

### Reference Policy 3

Allow ALL actions on EC2 except Stop and Terminate IF if the user is not
authenticated using multi-factor authentication (MFA)

<img src="images/image8.png"  width="75%">
</div>
