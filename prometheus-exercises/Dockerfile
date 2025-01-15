FROM openjdk:17-jdk-alpine
EXPOSE 8080 8081
RUN mkdir /opt/app
COPY build/libs/java-mysql-project-1.0-SNAPSHOT.jar /opt/app
WORKDIR /opt/app
CMD ["java", "-jar", "java-mysql-project-1.0-SNAPSHOT.jar"]
