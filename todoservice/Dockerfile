
FROM java:8-alpine
VOLUME /todoservice
ADD target/todoservice-0.0.1-SNAPSHOT.jar app.jar
RUN sh -c 'touch app.jar'
EXPOSE 8080
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-Dspring.profiles.active=docker","-jar","/app.jar"]
