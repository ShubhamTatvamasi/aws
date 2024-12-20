# code build


Trigger all builds:
```bash
region=us-east-2

projects=$(aws codebuild list-projects --query "projects" --output text --region $region)

for project in $projects; do
  echo "Starting build for project: $project"
  aws codebuild start-build --project-name "$project" --region $region
done

```

