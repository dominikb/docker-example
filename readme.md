# Docker Example

1. Clone the repository

```sh
git clone git@github.com:dominikb/docker-example.git
```

2. Build the Docker Image
```sh
cd docker-example
docker build --tag my-nginx .
docker run --rm -d --name my-nginx-container -p 1234:80 my-nginx

# Verify it is running
docker container ls
```

3. Visit the Website [http://localhost:1234]()

4. Stop the container and remove artifacts
```sh
docker stop my-nginx-container
docker image rm my-nginx
```