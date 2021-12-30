FROM openjdk:8-jdk-alpine
ARG JAR_FILE=build/libs/*.jar
COPY ${JAR_FILE} paas-ta-container-platform-pipeline-inspection-api.jar
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","-Dspring.profiles.active=prod","/paas-ta-container-platform-pipeline-inspection-api.jar"]
