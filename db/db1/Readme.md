# Build the Docker image
docker build -t bad-juju-db-image .

# Run the Docker container
docker run --name bad-juju-db-container -p 5432:5432 -d bad-juju-db-image