FROM maven:3.5.3-jdk-11 as builder

COPY . /usr/src/workshop03/
RUN mvn -f /usr/src/workshop03/pom.xml clean package -DskipTests

FROM openjdk:11.0-jdk
COPY --from=builder /usr/src/workshop03/target/workshop-*.jar /app.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]