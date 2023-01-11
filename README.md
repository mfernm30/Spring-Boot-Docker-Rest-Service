# spring-boot-docker-rest-service
This is a simple spring boot API rest service running in a docker container.

## Running app locally
Compile project with maven with commands or compile it with IntelliJ.
```
./mvnw clean package
```
Execute the app.
```
java -jar .\target\spring-boot-docker-rest-service-0.0.1-SNAPSHOT.jar
```

## Running app in Docker
Creating container with docker.
```
docker build -t dockerhub_username/spring-boot-docker-rest-service .
```
Run the app within the container.
```
docker run -p 8080:8080 dockerhub_username/spring-boot-docker-rest-service
```

## Further information

This project is based on this tutorials: 
  - [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/).
  - [Spring Boot with Docker](https://spring.io/guides/gs/spring-boot-docker/)

This project was made with Oracle OpenJDK version 1.8.0_351.
