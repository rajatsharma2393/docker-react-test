This is a simple React App to get started with Docker.

#Build and tag the Docker image:
docker build -t sample:dev .

#Then, spin up the container once the build is done:
docker run -v \${PWD}:/app -v /app/node_modules -p 3001:3000 --rm sample:dev
