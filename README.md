# Contanarized-Web-App-Deploy
It touches on the essential pillars of modern infrastructure: Containerization (Docker), Cloud Registry (ECR), Orchestration (ECS), and CI/CD (GitHub Actions).

# Login to ECR: Use the AWS CLI to authenticate Docker with AWS.
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 115966687062.dkr.ecr.us-east-1.amazonaws.com


# Tag and Push:
# Tag your Docker image to match your ECR repository name.
 1. docker tag ecs-demo-app:latest 115966687062.dkr.ecr.us-east-1.amazonaws.com/ecs-demo-app:latest

 2. docker push 115966687062.dkr.ecr.us-east-1.amazonaws.com/ecs-demo-repo:latest

# Summary
Docker: containerized a simpele Hello from AWS ECS Fargate!

ECR: managed cloud artifacts.

ECS/Fargate:run containers without managing servers.

CI/CD: linked code changes to infrastructure updates



