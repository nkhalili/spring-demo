# Spring 2.0 Demo

## YML Profiles

Rename application.properties to application.yml and add your configuration:

```yaml
spring:
  profiles: dev
server:
  port: 8081
---
spring:
  profiles: test
server:
  port: 8000
```

Build and Run your app (set your env variable):

```shell script
mvn clean package
java -jar -Dspring.profiles.active=dev target/spring2demo-0.0.1.jar
```

