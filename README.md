# mv-spring-boot-docker
Dockerize Spring Boot "initial" example

https://spring.io/guides/gs/spring-boot/

Modified pom.xml so you can build the project and create a Docker image out of it.

Step 1: docker package docker:build

To check if the docker image has been created, execute in the terminal:
docker images

You will see a similar entry like below:
REPOSITORY                   TAG                 IMAGE ID            CREATED             SIZE
spring-boot-example          latest              e7748cfac0b1        20 minutes ago      683.4 MB

Step 2: Run the image
docker run -p 8080:8080 spring-boot-example

Step 3: Access using the browser
http://localhost:8080/
