# aws

Title | Link
---|---
AWS Pricing Calculator | https://calculator.aws
Amazon EC2 Instance Comparison | https://ec2instances.info
Max Pods per instance type | https://github.com/awslabs/amazon-eks-ami/blob/master/files/eni-max-pods.txt
AWS CLI Docs | https://awscli.amazonaws.com/v2/documentation/api/latest/index.html

Configure Keys:
```bash
aws configure
```

Test aws key access:
```bash
aws iam get-user
```

Check availability zones for a region:
```bash
aws ec2 describe-availability-zones \
  --region us-west-1 \
  --query 'AvailabilityZones[*].ZoneName' \
  --output table
```

