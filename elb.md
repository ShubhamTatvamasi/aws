# ELB

List Target Group names:
```bash
aws elbv2 describe-target-groups --region us-east-1 --query "TargetGroups[].TargetGroupName" --output text | tr '\t' '\n'
```
