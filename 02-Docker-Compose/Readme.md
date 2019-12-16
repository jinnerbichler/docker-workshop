**Build Spring Boot Project**:

```shell script
mvn clean package -DskipTests
```

**Build Docker Image**:

```shell script
docker build -t jinnerbichler/workshop02 .
```

**Run Containers**:

```shell script
docker-compose up --build
```