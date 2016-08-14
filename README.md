# ExtendingSpringBootActuatorWithAngularJS

Internal Test to Extend the Spring Boot Actuator [sample](https://spring.io/guides/gs/actuator-service) with [Application initialization ](src/main/java/com/xtendsba/actuator/Application.java) and use the [AngularJS](https://angularjs.org) to explore the data that the [actuator endpoints](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#production-ready-endpoints) returns.

Also, added for CORS (Cross-Origin Resource Sharing) Filter.

## Deployment
In order to be able to deploy on [Heroku](https://www.heroku.com), server and management endpoints are kept on the same port (Heroku only supports one). You can update [application properties](src/main/resources/application.properties) in case you need to do two ports (you would also need to update the `managementURL` value in the angular [app](src/main/webapp/WEB-INF/js/actuate-app.js)).
