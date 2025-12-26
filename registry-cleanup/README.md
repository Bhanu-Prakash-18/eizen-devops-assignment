# Task 6 – Container Registry Cleanup

Container registries such as Amazon ECR can accumulate unused images over time.

## Cleanup Strategy
- Identify dangling or untagged images
- Remove them periodically

## Example (AWS ECR)
```bash
aws ecr list-images \
  --repository-name my-repo \
  --filter tagStatus=UNTAGGED

aws ecr batch-delete-image \
  --repository-name my-repo \
  --image-ids imageDigest=sha256:xxxx


