**Testcontainers** are Java libraries that provide lightweight, throwaway containers (e.g., databases, message queues) for integration testing. They use Docker to spin up real service instances during tests, ensuring realistic and isolated test environments.

**Secured variable** We use secured variables to protect sensitive data (like credentials) from being exposed in logs or code. They ensure credentials are only accessible within the GitHub Actions environment.

**needs: build-and-test-backend** ensures this job runs only if tests pass, enforcing that code is verified before Docker images are built and pushed.