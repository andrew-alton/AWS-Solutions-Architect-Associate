# Bucket Policy Document

## Policy 1 - Public Read Access

```

{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"PublicRead",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject"],
      "Resource":["arn:aws:s3:::demo-bucket/*"]
    }
  ]
}

```

## Policy 2 - Allow Only HTTPS

```
{
  "Id": "ExamplePolicy",
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "AllowSSLRequests",
      "Action": "s3:GetObject",
      "Effect": "Allow",
      "Resource": [
        "arn:aws:s3:::mykplabs-policy/*"
      ],
      "Condition": {
        "Bool": {
          "aws:SecureTransport": "true"
        }
      },
      "Principal": "*"
    }
  ]
}
```
