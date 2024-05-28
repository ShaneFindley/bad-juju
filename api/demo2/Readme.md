# Build the Docker image
docker build -t my-spring-boot-app .

# Run the Docker container
docker run -p 8080:8080 my-spring-boot-app