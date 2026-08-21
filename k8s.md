# k8s

Create a aws-cli pod:
```bash
kubectl -n default run aws-cli \
  --image=public.ecr.aws/aws-cli/aws-cli \
  --command -- sleep infinity
```
