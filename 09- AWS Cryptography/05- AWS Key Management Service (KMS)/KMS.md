# AWS Documeantion

<https://docs.aws.amazon.com/cli/latest/userguide/cli_kms_code_examples.html>

## encrypt

The following code example shows how to use encrypt.(Windows)

```
aws kms encrypt \
    --key-id 1234abcd-12ab-34cd-56ef-1234567890ab \ #ID of of key created in AWS
    --plaintext fileb://ExamplePlaintextFile \
    --output text \
    --query CiphertextBlob > C:\Temp\ExampleEncryptedFile.base64

certutil -decode C:\Temp\ExampleEncryptedFile.base64 C:\Temp\ExampleEncryptedFile

```
