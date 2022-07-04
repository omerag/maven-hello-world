FROM openjdk:11-jdk-slim
COPY target/*.jar app/
RUN ls app
CMD java -cp target/classes com.mycompany.app.App