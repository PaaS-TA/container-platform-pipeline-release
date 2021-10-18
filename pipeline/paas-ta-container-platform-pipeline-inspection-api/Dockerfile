FROM openjdk:8-jdk-alpine
ARG JAR_FILE=build/libs/*.jar
COPY ${JAR_FILE} container-platform-pipeline-inspection-api.jar
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","-Dspring.profiles.active=prod","/container-platform-pipeline-inspection-api.jar"]
