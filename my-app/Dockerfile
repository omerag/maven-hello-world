FROM maven:3.8.6-jdk-11-alpine as builder
COPY my-app app
RUN mvn package -f pom.xml



FROM openjdk:11-jdk-slim
COPY --from=builder app/target/my-app-*.*.*.jar app/hello.jar
CMD java -cp app/hello.jar com.mycompany.app.App
