# k8s

Create a aws-cli pod:
```bash
kubectl run aws-cli \
  --image=public.ecr.aws/aws-cli/aws-cli \
  --command -- sleep infinity
```
