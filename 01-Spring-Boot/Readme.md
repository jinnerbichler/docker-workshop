**Build Spring Boot Project**:

```shell script
mvn clean package -DskipTests
```

**Build Docker Image**:

```shell script
docker build -t jinnerbichler/workshop01:v0.1.0 .
```

**List local Images**:

```shell script
docker images
```

**Run Container**:

```shell script
docker run --name workshop01 -p 8080:8080 -t jinnerbichler/workshop01:v0.1.0
```

in daemon mode:

```shell script
docker run --name workshop01 -d -p 8080:8080 -t jinnerbichler/workshop01:v0.1.0
```

**Push Image**:

```shell script
docker push jinnerbichler/workshop01:v0.1.0
```

**Show Container Diff**:

```shell script
docker diff workshop01
```
