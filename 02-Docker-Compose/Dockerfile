FROM openjdk:11.0-jdk
COPY ./target/workshop-*.jar /app.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]