# Secure Spring-Boot Application using Keycloak

Using `keycloak-spring-boot-2-adapter`

* Keycloak Service version old 1.12: http://127.0.0.1:8080/auth
* Keycloak Service version 1.17++: http://127.0.0.1:8080/admin
* REALM: keylcoak deam
* client: spring-boot-mvc-app


# Configure in the application.properties

```
keycloak.realm = keycloak-demo
keycloak.auth-server-url = http://127.0.0.1:8080/admin
keycloak.resource = spring-boot-mvc-app
keycloak.principal-attribute=preferred_username
keycloak.public-client=true


spring.main.allow-bean-definition-overriding=true
server.port=8081
```


# Build & Run
`mvn clean spring-boot:run`