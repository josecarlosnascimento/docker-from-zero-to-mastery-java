FROM openjdk:11-jdk-slim
VOLUME /tmp
ADD app/target/docker-from-zero-to-mastery-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8080
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java", "-Djava.securiry.edg=file:/dev/./urandom","-jar", "/app.jar"]