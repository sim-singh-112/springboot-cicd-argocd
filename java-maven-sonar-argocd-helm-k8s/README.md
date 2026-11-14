# Java Maven SonarQube ArgoCD Kubernetes

End-to-end CI/CD project using:
- Java Spring Boot
- Jenkins
- Maven
- SonarQube
- Docker
- Kubernetes
- Argo CD

Our CI/CD workflow:

1. GitHub
   Developer pushes new Java code.
   
3. Jenkins
   Detects the code change and starts the pipeline.
   
5. Maven
   Compiles Java code, downloads dependencies and runs tests.
   
7. SonarQube
   Checks code quality, bugs and code vulnerabilities.
   
9. Docker
   Creates a Docker image and pushes it to Docker Hub.
   
11. Shell script
   Updates the image tag in the Kubernetes deployment YAML and pushes the change to Git.

13. Argo CD
   Detects the updated manifest and synchronizes the deployment.

15. Kubernetes
   Runs your Spring Boot application in Pods.
