**Build Spring Boot Project**:

```shell script
mvn clean package -DskipTests
```

**Build Docker Image**:

```shell script
docker build -t jinnerbichler/workshop01 .
```

**Run Container**:

```shell script
docker run -e "SPRING_PROFILES_ACTIVE=prod" -p 8080:8080 -t jinnerbichler/workshop01
```