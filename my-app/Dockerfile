FROM openjdk:11-jdk-slim
COPY my-app/target/my-app-*.*.*.jar app/hello.jar
RUN ls && pwd && ls app
CMD java -cp my-app/target/hello.jar com.mycompany.app.App