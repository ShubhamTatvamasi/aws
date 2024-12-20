# secrets manager

Force delete secret:
```bash
ssh aws secretsmanager delete-secret \
  --secret-id github_ssh_key \
  --force-delete-without-recovery \
  --region us-east-2
```
