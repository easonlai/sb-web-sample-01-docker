# Sample Java Web App in Spring Boot framework with Containerization
Readme update 1.1

## Build with Maven
```shell
mvn package
```

## Run locally
```shell
java -jar target/gs-spring-boot-docker-0.1.0.jar
```

## Test web app locally
```shell
http://localhost:8080
```

## Containerize
1. Build a docker image using `Dockerfile`:
   ```
   docker build -t sb-web-sample-01-docker .
   ```
2. Run docker image locally
   ```
   docker run --rm -p 8080:8080 sb-web-sample-01-docker
   ```
3. Then you can access the web app at http://localhost:8080 in browser.

Or you can pull this sample from my Docker Hub.
https://cloud.docker.com/u/easonlai/repository/docker/easonlai/sb-web-sample-01-docker
