FROM openjdk:11-jdk-slim
COPY my-app/target/my-app-*.*.*.jar app/hello.jar
RUN ls && pwd && ls app
RUN java -cp app/hello.jar com.mycompany.app.App
CMD java -cp app/hello.jar com.mycompany.app.App
