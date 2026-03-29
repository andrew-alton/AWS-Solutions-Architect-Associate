# EBS Encryption

## Basics of Disk Level Encryption

Disk Level encryption involves encrypting all the files that are part of the
storage device.
Multiple Set of Technologies: BitLocker, Apple FileVault and others

<div align="center">
<img src="images/image2.png" alt="IAM Policies" width="80%">
</div>

## EBS Encryption

Amazon EBS encryption uses AWS KMS keys when creating encrypted
volumes and snapshots.
For an encrypted EBS volume that is attached to a supported instance type, the
following types of data are encrypted:

1. Data at rest inside the volume
2. All data moving between the volume and the instance
3. All snapshots created from the volume
4. All volumes created from those snapshots

## Points to Note

Enabling EBS Encryption has minimal effect on latency.
Encryption and decryption are handled transparently, and they require no
additional action from you or your applications.
Amazon EBS encrypts your volume using industry-standard AES-256 data
encryption
