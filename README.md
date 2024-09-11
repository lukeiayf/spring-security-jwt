<h1 align="center">
  Spring Security JWT
</h1>

This is an application made to test Spring Security & JWT practices as seen on [this vídeo](https://youtu.be/kEJ8a1w4a2Q).

## Tecnologies

- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)
- [Spring Security](https://spring.io/projects/spring-security)
- [Spring Data JDBC](https://spring.io/projects/spring-data-jdbc)
- [H2](https://www.h2database.com)

## How to run
- Clone git repo:
```
git clone https://github.com/lukeiayf/spring-security-jwt
```

- Build project
```
./mvnw clean package
```

- Run:
```
java -jar ./target/spring-security-jwt-0.0.1-SNAPSHOT.jar
```

- Test ( with [httppie](https://httpie.io) or Postman):
```
http -a username:password POST :8080/authenticate
JWT = <token>
http :8080/private -A bearer -a ${JWT}
```