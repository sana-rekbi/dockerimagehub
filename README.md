## Docker Workflow Automation

This project includes an automated process to build and push a Docker image for the Python application to Docker Hub whenever changes are pushed to the main branch.

### Workflow Explanation:
1. **Trigger on Main Branch Push**: The workflow is triggered on any push event to the main branch.
2. **Setup Docker Buildx**: It checks out the code and sets up Docker Buildx for advanced Docker builds.
3. **Docker Hub Login**: The workflow logs into Docker Hub to authorize image pushing.
4. **Docker Image Build and Push**: Finally, it builds the Docker image using the provided Dockerfile and pushes the image to Docker Hub under the specified username and repository.

### How to Use:
1. Make sure Docker is installed and configured.
2. Ensure your GitHub repository has the necessary secrets for Docker Hub authentication (`DOCKER_USERNAME` and `DOCKER_PASSWORD`).
3. Update the Dockerfile as needed for your project.

This automation ensures the latest version of the Python application is always ready for deployment as a Docker container.
