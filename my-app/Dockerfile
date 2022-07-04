FROM openjdk:11-jdk-slim
COPY my-app/target/*.jar app/
RUN ls app
CMD java -cp target/classes com.mycompany.app.App