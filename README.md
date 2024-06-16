#create your springboot web app
1. create the jar file
2. write docker file 

#base docker image
FROM openjdk:17-jdk-alpine
LABEL maintainer="adewale"
ADD target/springboot-docker-demo-0.0.1-SNAPSHOT.jar springboot-docker-demo.jar
ENTRYPOINT ["java", "-jar", "springboot-docker-demo.jar"]

3. login to docker using terminal
4. docker image ls /// docker images
get the repository and tag of your application
5.create repository on docker online
run - docker tag springboot-docker-demo(repository):latest(tag) phemmy1212/springboot-docker-demo:latest
6. pushing the application to web docker
docker push phemmy1212/springboot-docker-demo:latest
7. docker pull phemmy1212/springboot-docker-demo:latest











