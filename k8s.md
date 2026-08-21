# k8s

Create a aws-cli pod:
```bash
kubectl -n default run aws-cli \
  --image=public.ecr.aws/aws-cli/aws-cli \
  --command -- sleep infinity
```

Get inside pod:
```bash
kubectl -n default exec -it aws-cli -- bash
```

```
mkdir -p ~/.aws
```

```
cat << EOF > ~/.aws/config
[default]
region = us-east-1
endpoint_url = http://rook-ceph-rgw-ceph-objectstore.rook-ceph.svc.cluster.local
EOF
```


```
cat << EOF > ~/.aws/config
[default]
aws_access_key_id = 898384F352206C8BA82C
aws_secret_access_key = UMmJZtaQKcloqgfMmB8IgDjOK88Hu5E82lB3yRQR
EOF
```


---

```bash
kubectl -n rook-ceph port-forward svc/rook-ceph-mgr-dashboard 8443:8443
```


