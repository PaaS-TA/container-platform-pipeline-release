FROM openjdk:8-jdk-alpine
ARG JAR_FILE=build/libs/*.war
COPY ${JAR_FILE} paas-ta-container-platform-pipeline-ui.war
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","-Dspring.config.location=application.yml","-Dspring.profiles.active=prod","/paas-ta-container-platform-pipeline-ui.war"]