FROM maven:3.5-jdk-8-alpine as builder
COPY my-app app
RUN mvn package -f pom.xml



FROM openjdk:8-jdk-slim
COPY --from=builder app/target/my-app-*.*.*.jar app/hello.jar
CMD java -cp app/hello.jar com.mycompany.app.App
